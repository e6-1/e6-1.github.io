---
layout: page
title: Resume
permalink: /resume/
---

<html>
	<head>
	
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, user-scalable=no, minimal-ui">
	
	<title>Ethan Petersen</title>
	<link href='http://fonts.googleapis.com/css?family=Merriweather:400,300,700' rel='stylesheet' type='text/css'>
	<link href='http://fonts.googleapis.com/css?family=Open+Sans:400,300,600' rel='stylesheet' type='text/css'>
	

	<style>
	body, html {
  padding-top:2.5em;
  margin:0;
  background-color:#fafafa;
}

.note {
  display:block;
  position: absolute;
  top:10px;
  left:10px;

  font-family: "Open Sans";
  font-size: 0.6em;
}

.new {
  background-color: #81C784;

  border: 1px solid #757575;
  padding: 1px;
  border-radius: 4px;

}

/* Header */

header {
  width:100%;
  vertical-align: middle;
  text-align: center;
 
}

.header-content {
  display: inline-block;
}

.pic {
  margin: 0 auto;
  margin-top:-2.5em;
  
  border-radius:10em;
  height:4em;
  width:4em;
  
  border: 2px solid #e0e0e0;
  transition : all 0.5s linear;
  
}

@-webkit-keyframes wiggle {
  0%   {
    transform: rotate(0deg);
  }
  25%  {
    transform: rotate(-30deg);
  }
  50%  {
    transform: rotate(15deg);
  }
  100% {
    transform: rotate(0deg);
  }
}

.pic:hover {
  /*Webkit fix*/
  -webkit-transform: translateZ(0);
  
  cursor:pointer;
  
  -webkit-animation: wiggle 0.7s cubic-bezier(0.6, -0.28, 0.735, 0.045);
}

.header-text {
  margin-top:0.5em;
  margin-left:1em;
}

header p {
  text-align:center;
  font-family: "Merriweather";
  
  margin:0;
  
  color: #212121;
}

.first-name {
   font-size: 1.05em;
}

.subtitle {
  font-family: "Merriweather";
  padding-top:.3em;
  font-size:0.55em;
  font-weight:500;
  color: #424242;
}

/* Information */

.paper {
  margin: 0 auto;
  margin-bottom:1em;
  
  background-color:white;
  width:100%;
  
  padding:0.5em 0 0.5em 0;
  
  border-top: 1px solid #e0e0e0;
  border-left: 1px solid #e0e0e0;
  border-right: 1px solid #e0e0e0;
  border-bottom: 3px solid #e0e0e0;
  border-radius:3px;
}

@media(max-width:992px) {
  .paper {
    width:80%;
  }
}

/* Content Part */

.content-wrapper {
  padding-right:7.25%;
}

.content {
  display:table;
  width:100%;
  
  padding-top:1.5em;
  
  /*border-top: 1px solid #eeeeee;*/
}

.content:last-child {
  margin-bottom: 2em;
}

body > div > article > div > section:last-child {
  padding-bottom:1.5em;
}

.row {
    display:table-row;
}
.row div {
    display:table-cell;
}

.content-cat {
  font-family: "Merriweather";
  font-variant:small-caps;
  font-weight:300;
  letter-spacing: 1px;
  
  color: #212121;
  
  font-size:0.975em;
  
  text-align:center;
  vertical-align:middle;

  padding-left:6.66%;
  width:30%;
}

.content-cat p {
  font-size:0.55em;
  font-weight:600;
  
  margin-bottom:0;
}

.content-text {
  border-left:1px solid #e0e0e0;
  transition: border 0.66s ease-in;
}

.big-text {
  vertical-align:top;
}

.content-text ul {
  padding:0;
  margin:0;
  margin-top:0.15em;
  
  width:85%;
  margin-left:1.5em;
}

.content-text ul:last-child {
  margin-bottom:0.5em;
}

.content-text ul li {
  font-family: "Open Sans";
  font-size:0.7em;
  
  display:inline-block;
  
}

.content-text ul li:first-child {
  width:35%;
  
  color: #424242;
  
  font-weight:600;
}

.content-text ul li a, div.content-text.work-listing.education-listing > p > strong > a {
  text-decoration: none;
  color: #0277bd;
}

.content-text ul li a:hover {
  color:#4fc3f7;
}

.work-listing p {
  font-family: "Open Sans";
  font-size:0.7em;
  
  color: #424242;
  
  margin-left:2em;
  margin-top:0.45em;
  margin-bottom: 0.45em;
}

div.content-text.work-listing.education-listing > p:nth-child(2) {
  margin-top:0.25em;
}

.work-listing .highlight {
  font-family: "Open Sans";
  font-size:0.7em;
  font-weight:400;
  
  color: #424242;
  
  margin-left:3.25em;
  padding-left:0.5em;
  
  border-left:1px solid #e0e0e0;
  
}

.education-listing > .heading {
  font-weight:600;
  
  margin-top:0.75em;
  margin-left:2em;
}

.education-listing > .highlight {
  margin-left:3.25em;
}

.highlight {
  transition: border .33s ease-in;
}

.profiles-listing ul li, .profiles-listing ul li:first-child {
  width:32%;
  font-weight: normal;
}

.work-content, .education-content {
  padding-top: .75em;
}

section.content.education-content > div > div.content-cat {
  vertical-align: top;
}

div.content-text.skills-listing > p {
  font-family: "Open Sans";
  font-size:0.7em;
  font-weight:400;

  margin-left: 2em;
  margin-top: 0.45em;
  margin-bottom: 0.45em;
}

div.content-text.skills-listing > p > {
  color:#212121;
}


	</style>

	<style media="print">
	
body, html {
  background-color: white;
  padding-top: 1.5em;
}

.paper {
  width:100%;
  border: 0;

  padding-top: 0;
}

header p {
  font-size: 1.3em;
}

.subtitle {
  font-size: 0.7em;
}

.header-pic {
  float:left;
}

.profiles {
  display:none;
}

.content {
  page-break-inside:avoid; 
  page-break-after:auto;
}

.header-text {
  float:left;
  margin-top: -1.6em;
}

.content-wrapper > .content:first-child {
  padding-top: 2em;
}

.content:last-child {
  padding-bottom: 0;
}

.content-cat {
  width:33%;
  color:black;
  text-align: left;
}

.content-cat p {
  font-size:0.6em;
  font-weight: 600;
}

header p, .content-text, .work-listing p, .content-text ul li:first-child, .work-listing .highlight, .content-text.skills-listing > ul > li > .highlight {
  color:black;
}

.content-text.skills-listing > ul > li span, .subtitle {
  color:#212121;
}

.content-text ul:last-child {
  margin-bottom: 0.25em;
}

.content-text ul li:first-child {
  width:50%;
}

.profiles-listing ul li:first-child {
  width:32%;
}

div.content-text.skills-listing > ul > li {
  width:33%;
}

.work-listing p {
  margin-bottom: 0.1em;
}

div.content-text.skills-listing > ul > li > p {
  margin-top: 0.4em;
  margin-bottom: 0.5em;
}

div.content-text.skills-listing > ul > li {
  padding-left: 1.5em;
}

div.content-text.skills-listing > ul > li:first-child {
  padding-left: 2em;
}

.note {
  display:none;
}

.content-text:hover {
  border-left:1px solid #eeeeee;
}

.content-text ul li a:hover {
  color:#4fc3f7;
}

.highlight:hover, .content-text.skills-listing > ul > li > .highlight:hover {
  border-left:1px solid #eeeeee;
}

.big-text {
  padding-top: 0;
}
	</style>
	
	</head>
	<body>
	
	<span class="note">Check out new print view! (<strong>Press Ctrl + P</strong>) (Not available in Live-Editor!)</span>

		<div class="resume-wrapper">
		  <article class="paper">
			    <header>
			      <div class="header-content">
			        <div class="header-text">
			          <p>
			            Ethan Petersen
			          </p>
			          <p class="subtitle">Programmer</p>
			        </div>
			      </div>
			    </header>
			    <div class="content-wrapper">
			    
			      <!-- CONTACT -->
			      <section class="content">
			        <div class="row">
			          <div class="content-cat">
			           Contact
			          </div>
			          <div class="content-text">

				            <ul>
				              <li>Email</li>
				              <li><a class="__cf_email__" href="/cdn-cgi/l/email-protection" data-cfemail="78081d0c1d0a0b1d17380a170b1d55100d14151916561d1c0d">[email&#160;protected]</a><script data-cfhash='f9e31' type="text/javascript">/* <![CDATA[ */!function(t,e,r,n,c,a,p){try{t=document.currentScript||function(){for(t=document.getElementsByTagName('script'),e=t.length;e--;)if(t[e].getAttribute('data-cfhash'))return t[e]}();if(t&&(c=t.previousSibling)){p=t.parentNode;if(a=c.getAttribute('data-cfemail')){for(e='',r='0x'+a.substr(0,2)|0,n=2;a.length-n;n+=2)e+='%'+('0'+('0x'+a.substr(n,2)^r).toString(16)).slice(-2);p.replaceChild(document.createTextNode(decodeURIComponent(e)),c)}p.removeChild(t)}}catch(u){}}()/* ]]> */</script></li>
				            </ul>

				            <ul>
				              <li>Phone</li>
				              <li>(815) 931-5217</li>
				            </ul>
			          </div>
			        </div>
			      </section>

			      <!-- LOCATION -->
					      <section class="content">
					        <div class="row">
					          <div class="content-cat">
					           Location
					          </div>
					          <div class="content-text">

						            <ul>
						              <li>Address</li>
						              <li>8181 Seale Ave</li>
						            </ul>

							            <ul>
							              <li>Postal Code & City</li>
							              <li>CA 94303 Palo Alto</li>
							            </ul>

						            <ul>
						              <li>Region</li>
						              <li>California</li>
						            </ul>

					          </div>
					        </div>
					      </section>

						
						<!-- LANGUAGE -->
			      <section class="content">
			        <div class="row">
			          <div class="content-cat">
			           Languages
			          </div>
			          <div class="content-text">

				            <ul>
											
				              	<li>English</li>

				              <li>Native speaker</li>

				            </ul>

			          </div>
			        </div>
			      </section>

			      <!-- PROFILES -->
				      <section class="content profiles">
				        <div class="row">
				          <div class="content-cat">
				           Profiles
				          </div>
				          <div class="content-text profiles-listing">
				            <ul>
					              	<li>
					              	<a href="https://www.linkedin.com/in/ethan-petersen-75122277" target="_blank">
							                	LinkedIn
							                </a>
							            </li>
					              	<li>
					              	<a href="https://twitter.com/cssema" target="_blank">
							                	Twitter
							                </a>
							            </li>
					              	<li>
					              	<a href="https://github.com/e6-1" target="_blank">
							                	Github
							                </a>
							            </li>
				            </ul>
				          </div>
				        </div>
				      </section>

								<section class="content">
			        <div class="row">
			          <div class="content-cat big-text">
											Work	Experience
			          
			            		<p>2016-03-07 till 2016-08-12</p>

			          </div>
			          <div class="content-text work-listing education-listing">
					            <p style="margin-top:2.4em;">
					            		<strong>Intern</strong> at <strong>Tesla Motors:</strong>
					            </p>

											<p>Within Tesla Motors lives Tesla Energy, a revolutionary venture in energy innovation.</p>

												<p class="highlight">Built web tools for sales engineers to simulate stationary storage performance and provide insight to market fits</p>
												<p class="highlight">Translated Matlab routines into Python/Cython scripts to forecast energy demand and accordingly optimize storage charge/discharge</p>

									
			          </div>
			        </div>
			      </section>
								<section class="content work-content">
			        <div class="row">
			          <div class="content-cat big-text">
			          
			            		<p>2015-07-21 till 2015-08-21</p>

			          </div>
			          <div class="content-text work-listing education-listing">
					            <p>
					            		<strong>Software Engineering Intern</strong> at <strong>Direct Supply:</strong>
					            </p>

											<p>An established innovator within the senior living industry, Direct Supply provides full life-cycle solutions for building, furnishing, and monitoring skilled-nursing facilities and assisted-living homes.</p>

												<p class="highlight">Improved software quality assurance through extensive unit testing</p>
												<p class="highlight">Learned best-practices in Agile software development</p>

									
			          </div>
			        </div>
			      </section>
								<section class="content work-content">
			        <div class="row">
			          <div class="content-cat big-text">
			          
			            		<p>2015-06-08 till 2015-07-17</p>

			          </div>
			          <div class="content-text work-listing education-listing">
					            <p>
					            		<strong>Research Intern</strong> at <strong>Pacific Undergraduate Research Experience:</strong>
					            </p>

											<p>Led by Dr. Luis Garcia-Puente and Dr. Rebecca Garcia, the PURE Math program began with two weeks of instruction in computational algebraic geometry, followed by three weeks of group research on an applied topic.</p>

												<p class="highlight">Collaborated with Ryan Kruse, Dane Miyata, Ihmar Aldana to produce original results pertaining to neural ideals</p>
												<p class="highlight">Developed algebro-geometric algorithms into open-source Python/Cython implementations</p>

									
			          </div>
			        </div>
			      </section>
								<section class="content work-content">
			        <div class="row">
			          <div class="content-cat big-text">
			          
			            		<p>2014-11-30 till 2015-02-20</p>

			          </div>
			          <div class="content-text work-listing education-listing">
					            <p>
					            		<strong>Software Engineering Intern</strong> at <strong>Rose-Hulman Ventures:</strong>
					            </p>

											<p>Consulted for Direct Supply to redesign a solution for tracking and logging inventory and contracts.</p>

												<p class="highlight">Cooperated with three other interns to build web pages and services in Outsystems to view and edit inventory items</p>
												<p class="highlight">Learned effective technical collaboration and communication with long-distance stakeholders</p>

									
			          </div>
			        </div>
			      </section>

				      <section class="content">
				        <div class="row">
				          <div class="content-cat big-text">
				          	RHIT Career Center
				          
				            		<p>2014-09-07 till 2016-02-22</p>

				          </div>
				          <div class="content-text work-listing">
										
					            <p>
					            	Assisted in set-up and management of quarterly career fairs on campus.
					            </p>

				          </div>
				        </div>
				      </section>
					

								<section class="content">
				        <div class="row">
				          <div class="content-cat big-text">

				            	Education

				            		<p>2014-09-07 till 2018-05-30</p>

				          </div>
				          <div class="content-text work-listing education-listing">
						            <p class="heading" style="margin-top:2.35em;">Rose-Hulman Institute of Technology</p>

				            		<p class="highlight">
													Bachelor:
				            		<i>Computer Science and Mathematics (3.74)</i>
				            		</p>

				          </div>
				        </div>
				      </section>

				      <section class="content">
				        <div class="row">
				          <div class="content-cat big-text">
				            	Awards

				            	<p>Best Student Project Travel Award</p>

				            	<p style="margin-top:0.25em;">2016-02-19</p>

				          </div>
				          <div class="content-text work-listing">

					         		<strong><p class="heading">Independent Project/Research Opportunities Program</p></strong>

				            	<p class="highlight">This award would pay for a student and faculty advisor to present at a conference: conference fees, air fare, hotels, meals, etc.</p>
				          </div>
				        </div>
				      </section>
				      <section class="content">
				        <div class="row">
				          <div class="content-cat big-text">

				            	<p>Goldwater Scholarship Nominee</p>

				            	<p style="margin-top:0.25em;">2016-03-30</p>

				          </div>
				          <div class="content-text work-listing">

					         		<strong><p class="heading">Rose-Hulman Institute of Technology</p></strong>

				            	<p class="highlight">Its goal is to provide a continuing source of highly qualified scientists, mathematicians, and engineers by awarding scholarships to college students who intend to pursue careers in these fields.</p>
				          </div>
				        </div>
				      </section>
				      <section class="content">
				        <div class="row">
				          <div class="content-cat big-text">

				            	<p>Theodore Paine Palmer Award</p>

				            	<p style="margin-top:0.25em;">2015-05-30</p>

				          </div>
				          <div class="content-text work-listing">

					         		<strong><p class="heading">Rose-Hulman Institute of Technology</p></strong>

				            	<p class="highlight">Awarded by vote of the mathematics faculty to a student or students who have demonstrated excellence in mathematics during the freshman year.</p>
				          </div>
				        </div>
				      </section>

			      <section class="content">
			        <div class="row">
			          <div class="content-cat">
			            Skills
			          </div>
			          <div class="content-text skills-listing">
			            	<p>
			            	<span class="name">
											<strong>
											Programming:

											</strong>
			            	</span>


												Python, Cython, Java, Hive, Pig, Sqoop, Oozie
			            	</p>
			            	<p>
			            	<span class="name">
											<strong>
											Econometrics:

											</strong>
			            	</span>


												Stochastic simulation, Event studies, Regression models
			            	</p>
			          </div>
			        </div>
			      </section>

			      <section class="content">
			        <div class="row">
			          <div class="content-cat">
			            Interests
			          </div>
			          <div class="content-text skills-listing">
			            	<p>
			            	<span class="name">
											<strong>
												Outdoors:
											</strong>
			            	</span>
												Hiking, Rafting, SCUBA Diving
			            	</p>
			          </div>
			        </div>
			      </section>

		    </div>
		      
		  </article>
		  
		</div>
	</body>
</html>

