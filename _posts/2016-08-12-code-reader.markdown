---
layout: post
title:  "Swift: Barcode Scanning"
date:   2016-08-12 10:58:31 +0800
categories: portfolio
---

This is an updated walkthrough on implementing a QR code or barcode scanner for iOS applications using Swift! When I was looking to use one,
my goal was to create a popup scanner, and so that's what we'll make today.

First, make sure that there is a ```UIView``` contained in the ```ViewController``` that will handle the scanning. Set some appropriate constraints
and place a label somewhere within the scanner view. We'll use this label to show what's being decoded.

At the top of your view controller's source code, import ```AVFoundation``` and add the ```AVCaptureMetadataOutputObjectsDelegate``` protocol to the controller. In ``viewDidLoad``
add the following code:

~~~
let captureDevice = AVCaptureDevice.defaultDeviceWithMediaType(AVMediaTypeVideo)

var input: AnyObject?
do {
    input = try AVCaptureDeviceInput(device: captureDevice)
} catch {
    let nsError = error as NSError
    print(nsError.localizedDescription)
    return
}
~~~

Note that to test out the scanning, the application has to be installed on a physical device otherwise a "Cannot Read" error will pop up. But let's break down what we just did:
we created a capture device that will automatically take in video data using the back camera by default, and then we set the input for that device to a local variable. Now that we
have the input images, we want to detect and decode barcodes. Define a class variable as ```captureSession```, that way we can start and stop from anywhere in the code. Then, continue to
add the following lines into ```viewDidLoad```.

~~~
captureSession = AVCaptureSession()
captureSession?.addInput(input as! AVCaptureInput)

let captureMetadataOutput = AVCaptureMetadataOutput()
captureSession?.addOutput(captureMetadataOutput)

captureMetadataOutput.setMetadataObjectsDelegate(self, queue: dispatch_get_main_queue())
captureMetadataOutput.metadataObjectTypes = [AVMetadataObjectTypeDataMatrixCode]
~~~

In the above code we created a capture session that will perform all the heavy-lifting of decoding, but we first need to specify the input and
output. The input will be metadata from the capture device that we defined earlier, but we have to further define the output. It's important at this step
to know what type of code you're using (whether it is QR, barcode, data matrix, etc). We set ```self``` to be the metadata delegate (this is why we implement 
the protocol), then the Apple documentation recommends using a serial queue which we can conveniently use the default queue from ```dispatch_get_main_queue()```.

If we want to see what the input is capturing, we need to add the following code (again, it's useful to create global variables):

~~~
videoPreviewLayer = AVCaptureVideoPreviewLayer(session: captureSession)
videoPreviewLayer?.videoGravity = AVLayerVideoGravityResizeAspectFill
videoPreviewLayer?.frame = scannerView.layer.bounds
scannerView.layer.addSublayer(videoPreviewLayer!)
self.view.bringSubviewToFront(scannerView)

scannerView.bringSubviewToFront(messageLabel)
~~~

The video preview layer will display inputs from the camera, and then we want to bring our subview and label to front. For the pop-up effect, we set
the ```.hidden``` property to ```false``` here. Finally, we can start capturing output with ```captureSession?.startRunning()```. To end, simply use ```// Start video capture.
captureSession?.stopRunning()```.

To process the output, we need to implement the following optional delegate method:

~~~
func captureOutput(captureOutput: AVCaptureOutput!, didOutputMetadataObjects metadataObjects: [AnyObject]!, fromConnection connection: AVCaptureConnection!) 
~~~

We'll first check to see if the metadata objects are present with:

~~~
if metadataObjects == nil || metadataObjects.count == 0 {
    messageLabel.text = "No QR code is detected"
    return
}
~~~

And finally, we can use the decoded text:

~~~
let metadataObj = metadataObjects[0] as! AVMetadataMachineReadableCodeObject

if metadataObj.type == AVMetadataObjectTypeDataMatrixCode {
    let barCodeObject = videoPreviewLayer?.transformedMetadataObjectForMetadataObject(metadataObj as AVMetadataMachineReadableCodeObject) as! AVMetadataMachineReadableCodeObject
    
    if metadataObj.stringValue != nil {
        messageLabel.text = metadataObj.stringValue
    }
}
~~~

To nicely animate the pop-out or pop-in scanning, the below code can be very useful:

~~~
captureSession?.stopRunning()
UIView.transitionWithView(scannerView, duration: 0.4, options: .TransitionCrossDissolve, animations: {
    self.scannerView.hidden = true // or false if you're making the view appear
    }, completion: nil)
~~~

Congrats! Now you have a nice pop-up scanner view that reads and displays barcodes! One final reminder: the application must be put onto a physical device to test out the barcode reading.