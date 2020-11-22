---
title: 'COVID SafePlaces - App Development'
subtitle: PathCheck Foundation, MIT Media Lab - Volunteer UI Engineer
description: COVID SafePlaces is an open-source, privacy preserving mobile app for digital contact tracing based on research originally conducted by the MIT Media Lab Camera Culture group.
featured_image: '/images/safeplaces/app_landing.png'
date: 2020-10-04
---

![]({{site.baseurl}}/images/safeplaces/app_landing.png)

### COVID SafePlaces is an open-source, privacy preserving mobile app for digital contact tracing based on research originally conducted by the MIT Media Lab Camera Culture group.

<br />

<center>
	<div style="display: flex; justify-content: space-between;">
		<div style="flex: 33%;">
			<h4>Time Frame</h4>
			<ul style="list-style: none;">
				<li>March 2020 - July 2020</li>
				<li>(4 months)</li>
			</ul>
		</div>
		<div style="flex: 33%;">
			<h4>Roles (Volunteer)</h4>
			<ul style="list-style: none;">
				<li>UI Engineer</li>
				<li>Interaction Designer</li>
			</ul>
		</div>
		<div style="flex: 33%">
            <h4>Contributions</h4>
            <ul style="list-style: none;">
				<li>
                    <a href="https://github.com/Path-Check/covid-safe-paths/commits?author=Patrick-Erichsen" class="button button--medium">View  on GitHub</a>
                </li>
			</ul>
        </div>
	</div>

	<hr />

	<h2>In the news</h2>
	<div style="display: flex; justify-content: space-between;">
		<div style="flex: 50%;">
			<a href="https://www.wired.com/story/phones-track-spread-covid19-good-idea/" target="_blank">
				<figure>
					<img src="{{site.baseurl}}/images/safeplaces/in-the-news/wired.png" style="padding-bottom: 10px;">
					<figcaption>	
							Phones Could Track the Spread of Covid-19. <br /> Is It a Good Idea?
					</figcaption>
				</figure>
			</a>
		</div>
		<div style="flex: 50%;">
			<a href="https://www.technologyreview.com/2020/03/17/905257/coronavirus-infection-tests-app-pandemic-location-privacy/" target="_blank">
				<figure>
					<img src="{{site.baseurl}}/images/safeplaces/in-the-news/mit-tech-review.png" style="padding-bottom: 10px;">
					<figcaption>
						A new app would say if you’ve crossed paths <br /> with someone who is infected
					</figcaption>
				</figure>
			</a>
		</div>
	</div>

	<hr />
</center>

## Overview

Like millions of others, when COVID-19 brought life to a standstill in March, I felt helpless. Unlike the defining wars and crises of previous generations, this pandemic has no enemy to mobilize against or military effort to enlist in.

I knew that my skills as a UI Engineer could somehow be put to use, but I struggled to find where. After learning of SafePlaces through the Hyperledger Foundation newsletter, I immediately knew that this was an impactful project where I could make a difference.

<span class="highlighted-text">Once joining the team, I collaborated with a small group of core contributors on the React Native mobile app, building key features for the GPS-based contact tracing application.</span>

The app can be downloaded on both the [App Store](https://apps.apple.com/us/app/pathcheck-safeplaces/id1508266966) and the [Google Play Store](https://play.google.com/store/apps/details?id=org.pathcheck.covidSafePlaces&hl=en_US&gl=US).

## Problem

> “[Some of my patients] were more afraid of being blamed than dying of the virus" <br/><br/> -Lee Su-young, Psychiatrist at Myongji Hospital, South Korea [^2]

With a median smartphone usership rate of over 75% in advanced economies[^1], digital contact tracing represents a promising solution which can be utilized to quickly and accurately identify an infected individual’s contacts. <span class="highlighted-text">However, the same capabilities that enable digital contact tracing pose significant privacy concerns to individuals</span>. 

Mass surveillance, limited individual freedoms, and exposure of private details are all potential results of allowing government and public health officials to trace individuals' movements.

## Solution

<img style="padding-left: 10px" src="{{site.baseurl}}/images/safeplaces/users-with-server.png" width="25%" height="25%" align="right"/>

<span class="highlighted-text">SafePlaces addresses these concerns with a privacy-first implementation of both GPS and Bluetooth based digital contact tracing.</span>

PathCheck, the foundation behind the SafePlaces project, offers a white-label app with a multitude of plug-and-play capabilities that local governments and public health authorities can tailor to their needs. Location/Bluetooth data is stored on your own device, and only ever leaves your device with your permission.

## Joining The Project

Although I filled out a volunteer form to be onboarded, due to the emerging pandemic and hectic nature of an early stage startup, I never was put in contact with anyone from the project.

After exploring the codebase, I found a "`##TODO`" comment, [opened an issue on GitHub](https://github.com/Path-Check/covid-safe-paths/issues/375), and began working on my first feature.

## Contributions

The primary contributors to the app up to the point had been engineers and researchers from MIT, and as a result, the UX was lacking. <span class="highlighted-text">Alongside a dedicated team of volunteers, I worked on improving three key aspects of the project.</span>

### Onboarding

The onboarding process suffered not only from a confusing code path that was difficult to extend, but also failed to properly comfort the user and explain the key concepts of the app.

<center>
	<div style="display: flex; justify-content: space-between; padding-top: 15px; padding-bottom: 20px;">
		<div style="flex: 50%; padding-right: 10px">
			<img src="{{site.baseurl}}/images/icons/help.png">
			<h4>Vague / Technical Descriptions</h4>
			<ul style="list-style: none;">
				<li>
					Users expressed a sense of confusion and uncertainty during onboarding
				</li>
			</ul>
		</div>
		<div style="flex: 50%; padding-left: 10px">
            <img src="{{site.baseurl}}/images/icons/language.png">
			<h4>English Only</h4>
			<ul style="list-style: none;">
				<li>
					Although our initial deployment was for a non-English speaking region, the onboarding language strings were hard coded in English
				</li>
			</ul>
        </div>
	</div>
</center>

#### Improving Onboarding Flows To Put Users At Ease

<center>
	<figure>
		<img src="{{site.baseurl}}/images/safeplaces/reviews/doesnt-do-anything.png" alt="testimonial" width="50%" height="50%" style="padding-bottom: 15px">
		<figcaption>App Store Review</figcaption>
	</figure>
</center>

<span class="highlighted-text">Based on user interviews and initial feedback from the app store, our team determined that the biggest opportunities were to clarify technical jargon and calm users during onboarding</span>:

<div style="padding-left: 25px; padding-top: 10px">
	<ul>
		<li>
			Created Figma prototypes to indicate the state of requested device permissions
		</li>
		<li>
			Clarified and condensed descriptions to better fit on smaller, cheaper devices 
		</li>
		<li>
			Implemented translation logic for user locales
		</li>
	</ul>
</div>

<div class="gallery" data-columns="1" style="height: 30%; width: 30%; overflow: auto;">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_1.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_2.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_3.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_4.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_5.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_6.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_7.png">
	<img src="{{site.baseurl}}/images/safeplaces/onboarding/step_8.png">
</div>

### Health Authority Subscription

<center>
	<figure>
		<img src="{{site.baseurl}}/images/safeplaces/reviews/no-instructions.png" alt="testimonial" width="75%" style="padding-bottom: 15px">
		<figcaption>Google Play Store Review</figcaption>
	</figure>
</center>

One of the most critical features of the app is the subscription to a local health authority. 

The healthcare authority is where infected individuals' location/bluetooth logs are uploaded. If a user does not subscribe to a healthcare authority, they will not know if they have crossed paths with a COVID-19 positive individual.

#### Implementing HA Auto Subscribe

Early on, we decided as a team that users should have the ability to automatically subscribe to healthcare authorities in regions they have travelled to. To enable this, I implemented an auto subscription feature and added a step in the onboarding flow to let users opt-in to auto subscription.

<img style="padding-left: 10px" src="{{site.baseurl}}/images/safeplaces/ha/autosub.png" width="45%" height="75%" />

#### Updating The Healthcare Authority Subscription Screen

The original Healthcare Authority Subscription screen provided little context as to what "subscribing" entailed, and required a user to manually input a URL that they had to track down on their own.

<span class="highlighted-text">Based on user interviews and initial feedback from the app store, I helped design, prototype and implement a more explanatory and easy to use interface.</span>

<center>
	<div style="display: flex;">
		<div style="flex: 50%; padding-right: 20px;">
			<figure>
				<img src="{{site.baseurl}}/images/safeplaces/ha/old.png" alt="old" style="padding-bottom: 10px">
  				<figcaption>Previous Health Authority Subscription Screen</figcaption>
			</figure>
		</div>
		<div style="flex: 50%; padding-left: 20px;">
			<figure>				
				<img src="{{site.baseurl}}/images/safeplaces/ha/landing.png" height="50%" alt="new" style="padding-bottom: 10px">
  				<figcaption>Updated Health Authority Subscription Screen</figcaption>
			</figure>
		</div>
	</div>
</center>

### Community Management

After a few months on the project, and the departure of some of the early contributors, I held a fair amount of tribal knowledge around the history and direction of the codebase. As such, I began assisting with community management in a number of ways.

<center>
	<div style="display: flex; justify-content: space-between; padding-top: 30px; padding-bottom: 20px;">
		<div style="flex: 50%;">
			<h2>100+</h2>
			<ul style="list-style: none;">
				<li>
					Contributors on GitHub
				</li>
			</ul>
		</div>
		<div style="flex: 50%">
			<h2>35</h2>
			<ul style="list-style: none;">
				<li>
					Average commits per week
				</li>
			</ul>
        </div>
	</div>
</center>

#### Managing Pull Requests

I worked alongside the project management team to update our [CONTRIBUTING.md](https://github.com/Path-Check/covid-safe-paths/blob/develop/CONTRIBUTING.md) guidelines, keep our work visible to the broader open source community, and improve pull request quality with a simplified [PULL_REQUEST_TEMPLATE.md](https://github.com/Path-Check/covid-safe-paths/blob/develop/.github/PULL_REQUEST_TEMPLATE.md).

#### Rewriting A Confusing README

One of the most frequent problems with new volunteers was difficulties following the instructions in our `README` to set up and run the project on their devices. 

The information hierarchy was hard to parse, the instructions were out of date, and the original authors made implicit assumptions about how experienced readers were with mobile development.

<center>
	<div style="display: flex;">
		<div style="flex: 50%; padding-right: 20px;">
			<figure>
				<img src="{{site.baseurl}}/images/safeplaces/readme/old.png" alt="before">
  				<figcaption>Previous README</figcaption>
			</figure>
		</div>
		<div style="flex: 50%; padding-left: 20px;">
			<figure>
				<img src="{{site.baseurl}}/images/safeplaces/readme/new.png" alt="after">
  				<figcaption>Updated README</figcaption>
			</figure>
		</div>
	</div>
</center>

<span class="highlighted-text">The README has more content than shown above, but some of the key updates I made included:</span>

* Simpler, clearer information hierarchy written in an imperative tone
* Proper hyperlinks to relevant content, with a clear step to read our contribution guidelines
* Instructions for both Windows/macOS users
* Callouts to previously required steps/knowledge

## Reflection

### Helping Combat COVID-19

Although my contributions pale in comparison to the sacrifices made by millions of front line workers, helping to develop SafePlaces was the most impactful contribution I felt that I could make to address the COVID-19 pandemic.

<span class="highlighted-text">Working on a software project that has such a significant and tangible impact on end users has helped me to better understand the importance of user-centered design, and made me realize how much I enjoy tackling complex and ambiguous problems such as digital contact tracing.</span>

### Working On Open Source Software

<center>
	<figure>
		<img src="{{site.baseurl}}/images/safeplaces/contributor-graph.png" alt="contributor graph" width="75%" height="75%" style="padding-bottom: 15px;">
		<figcaption>Contributor graph during April 2020</figcaption>
	</figure>
</center>

Although my work on <a href="{{site.baseurl}}/project/consensource">ConsenSource</a> is also open-source (OS), this was my first OS project that I had volunteered on. It was also my first time working alongside contributors whom I had never met in person. 

Collaborating with a talented group of developers, designers, project managers, and other individuals from across the globe to tackle a shared mission was an incredible experience, and has motivated me to continue to contribute to OS projects in my career.

### First Mobile Development Project

Prior to working on SafePlaces, I had no experience developing mobile applications. Thankfully, the project was written in React Native, so I was able to get up to speed and begin making contributions relatively quickly thanks to my existing JavaScript/React background.

Mobile development is a platform I hope to continue to explore in future projects. I thoroughly enjoyed having to solve problems within the constraints of the platform, particularly when taking into account the range of devices that our users possess, from iPhone users in Jackson Hole, WY, to Android feature-phone users in nations such as Haiti.

[^1]: <a href="https://www.pewresearch.org/global/2019/02/05/smartphone-ownership-is-growing-rapidly-around-the-world-but-not-always-equally/pg_global-technology-use-2018_2019-02-05_0-01/" target="_blank">Pew Research: Smartphone ownership in advanced economies higher than in emerging</a>
[^2]: <a href="https://arxiv.org/pdf/2003.08567.pdf" target="_blank">Apps Gone Rogue: Maintaining Personal Privacy in an Epidemic</a>