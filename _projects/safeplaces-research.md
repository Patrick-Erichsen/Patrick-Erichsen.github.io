---
title: 'COVID SafePlaces - Research'
subtitle: PathCheck Foundation, MIT Media Lab - Researcher, Signals Processing
description: Participated in research into novel approaches to privacy preserving digital contact tracing using Wifi Colocation.
featured_image: '/images/safeplaces-research/abstract.png'
date: 2020-10-03
---

![]({{site.baseurl}}/images/safeplaces-research/abstract.png)

<br />

<center>
	<div style="display: flex; justify-content: space-between;">
		<div style="flex: 33%;">
			<h4>Time Frame</h4>
			<ul style="list-style: none;">
				<li>July 2020 - August 2020</li>
				<li>(2 months)</li>
			</ul>
		</div>
		<div style="flex: 33%;">
			<h4>Roles (Volunteer)</h4>
			<ul style="list-style: none;">
				<li>Researcher</li>
			</ul>
		</div>
		<div style="flex: 33%">
            <h4>Outcome</h4>
            <ul style="list-style: none;">
				<li>
                   <a href="https://arxiv.org/pdf/2009.12699.pdf" class="button button--medium">View paper</a>
                </li>
			</ul>
        </div>
	</div>

	<p style="padding-top: 30px;">
		<a href="{{ site.baseurl }}/project/safeplaces-app-development">View mobile app contributions to SafePlaces</a>
	</p>
</center>

<hr />

In addition to the development of a flagship mobile app, the PathCheck foundation has a research arm led by members of the Camera Culture group at the  MIT Media Lab.

<span class="highlighted-text">After 4 months of helping to develop features on the mobile app, I joined the <b>Wifi Colocation group</b> to assist in research on novel approaches to digital contact tracing.</span>

## Introduction

<img style="padding-left: 10px" src="{{site.baseurl}}/images/safeplaces-research/device-diagram.png" width="50%" height="50%" align="right"/>

Privacy-preserving proximity inference is crucial to the success of a digital contact tracing solution.
The majority of mainstream solutions use either Bluetooth or GPS based colocation to achieve this.
However, a third option that is not as widely discussed is WiFi Colocation.

<span class="highlighted-text">In this paper, we investigate a hybrid implementation of three WiFi Colocation approaches described in Sapiezynski et. al, Das et al., and Carreras et. al.</span>

The hybrid implementation functions as follows:

- When a user is actively using WiFi, a deterministic if/else classifier infers proximity using features extracted from scans of nearby WiFi access points (APs)
- In the case where a user is not actively using WiFi, a duty-cycle that rotates the device between acting as a WiFi hotspot and a WiFi receiver will allow for proximity inference without interfacing with APs

## Process

### Researching Prior Art

Following the outbreak of COVID-19, a number of groups have explored ways to leverage WiFi signal processing to help enforce social distancing guidelines and improve digital contact tracing efforts. 

Wifi Colocation provides a number of distinct advantages over other approaches such as GPS/Bluetooth based colocation, particularly in terms of user privacy. <span class="highlighted-text">However, our team identified a handful of limitations to the state of the art when considering the application of Wifi Colocation in a practical context:</span>

- Implementations leveraging hotspot duty cycles will disconnect a user from their current Wifi connection, providing a poor user experience
- The iOS platform limits developer access to many of the APIs required to programatically interact with device hotspots

### Hybrid Implementation

The group determined that the two most relevant approaches that could be leveraged in a hybrid implementation were those outlined in <a href="https://arxiv.org/pdf/1610.04730.pdf" target="_blank">Sapiezynski et. al.</a> and <a href="https://www.researchgate.net/publication/241630493_Comm2Sense_Detecting_proximity_through_smartphones" target="_blank">Carreras et. al.</a>

<span class="highlighted-text">Combining the approaches in these two papers provides a number of distinct benefits in a practical context:</span>

- Provides a better user experience by falling back to access point based scanning if a user is connected to a Wifi network, which prevents the user from disconnecting from the network
- Wifi based colocation does not require direction interaction with participating parties, providing greater privacy to the user


## Contributions

In addition to helping author the final paper and participating in general discussions around research direction, my primary contributions were as follows.

### Proof Of Concept Android Code

Although the Android OS exposes APIs to programatically access the hotspot on a users device, there were no existing React Native bindings for these APIs. The SafePlaces application is written using the React Native framework, so I developed the required bindings to allow our developers to have simpler access to this logic.

### Recruiting Volunteers

The SafePlaces Slack community has well over 1,000 members from around the world, involved in the project in a variety of capacities.

I lead efforts to reach out to various members of the community to gather volunteer research participants to collect access point scans from Android devices to train our classification models on.

### Developing In-App Data Collection 

In order to collect access point scan information from the volunteers, I developed an additional screen that interacted with the React Native hotspot bindings that I authored to record RSSI values at varying distances.

<center>
	<figure>
		<img src="{{site.baseurl}}/images/safeplaces-research/data-collection.png" width="30%" height="30%" style="padding-bottom: 15px;">
		<figcaption>
			Data collection screen
		</figcaption>
	</figure>
</center>



