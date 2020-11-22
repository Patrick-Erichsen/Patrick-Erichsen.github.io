---
title: 'ConsenSource'
subtitle: Target Corp - Lead UI Engineer
description: ConsenSource is an open-source blockchain platform designed to bring <i>transparency</i> and <i>trust</i> to the sourcing industry - making it easier to find and verify the certifications and audit histories of a factory.
featured_image: '/images/consensource/overview.png'
date: 2020-10-02
---

![]({{site.baseurl}}/images/consensource/overview.png)

### ConsenSource is an open-source blockchain platform designed to bring <i>transparency</i> and <i>trust</i> to the sourcing industry - making it easier to find and verify the certifications and audit histories of a factory.

<br />

<center>
	<div style="display: flex; justify-content: space-between;">
		<div style="flex: 33%;">
			<h4>Time Frame</h4>
			<p>August 2019 - Present</p>
		</div>
		<div style="flex: 33%;">
			<h4>Roles</h4>
			<ul style="list-style: none;">
				<li>Lead UI Engineer</li>
				<li>User Researcher</li>
			</ul>
		</div>
        <div style="flex: 33%">
            <h4>Contributions</h4>
            <ul style="list-style: none;">
				<li>
                    <a href="https://github.com/target/consensource-ui/commits?author=Patrick-Erichsen" class="button button--medium">View  on GitHub</a>
                </li>
			</ul>
        </div>
	</div>

	<hr />

	<h2>In the news</h2>
	<div style="display: flex; justify-content: space-between;">
		<div style="flex: 50%;">
			<a href="https://www.coindesk.com/retail-giant-target-is-working-on-a-blockchain-for-supply-chains" target="_blank">
				<figure>
					<img src="{{site.baseurl}}/images/consensource/in-the-news/coindesk.png" style="padding-bottom: 10px;">
					<figcaption>	
							Retail Giant Target Is Quietly Working on a Blockchain for Supply Chains
					</figcaption>
				</figure>
			</a>
		</div>
		<div style="flex: 50%;">
			<a href="https://www.forbes.com/sites/darrynpollock/2019/06/10/retail-giant-target-unmasks-its-blockchain-framework-aimed-at-supply-chain/?sh=6339ca602f2e" target="_blank">
				<figure>
					<img src="{{site.baseurl}}/images/consensource/in-the-news/forbes.png" style="padding-bottom: 10px;">
					<figcaption>
						Retail Giant Target Unmasks Its Blockchain Framework Aimed At Supply Chain
					</figcaption>
				</figure>
			</a>
		</div>
	</div>

	<hr />
</center>

## Overview

In 2018, Target began to investigate potential use cases for blockchain technology. Through an internal incubator program, a team of sourcing experts identified a growing need for increased transparency around the certification process of factories. 

<span class="highlighted-text">The ConsenSource platform emerged out of this work, with a mission to empower responsible sourcing through blockchain technology.</span>

## Problem

For many retailers, a common pain point in the sourcing process is the discovery and verification of the certification claims for a given factory. If a retailer wishes to only do business with factories that have a given certification, where can they find a filtered list of only the factories that are certified? <span class="highlighted-text">Furthermore, how can they trust that the certification is valid?</span>

In practice, each retailer ends up independently verifying these claims with the certifying body that performed the original audit. This process is time-consuming, expensive, and error prone. 

## Solution

<!-- <center style="padding-top: 25px; padding-bottom: 15px;">
	<video width="780" height="360" controls>
		<source src="{{site.baseurl}}/images/consensource/ConsenSource.mp4" type="video/mp4">
	</video>
</center> -->

ConsenSource is able to address these difficulties by leveraging a permissioned blockchain. Using a blockchain platform allows companies to share a single source of truth as to the certification status of a given factory, eliminating the need to reconcile data across dozens of sources. <span class="highlighted-text">Members of the ConsenSource network receive immediate, verifiably accurate information when certification data is updated.</span>

#### One Product, Four Users

Through interviews with both internal sourcing team members and external partners, our team identified four personas that can benefit from the ConsenSource platform. Each persona has a distinct set of benefits, and a distinct set of actions that they can perform to modify the distributed ledger.

##### Retailer Benefits

<img src="{{site.baseurl}}/images/consensource/retailer_landing.png">

##### Factory Benefits

<img src="{{site.baseurl}}/images/consensource/factory_landing.png">

##### Certifying Body Benefits

<img src="{{site.baseurl}}/images/consensource/cert_landing.png">

##### Standards Body Benefits

<img src="{{site.baseurl}}/images/consensource/std_landing.png">

## Contributions

As the lead UI Engineer on the team, my responsibilities on a given day can range from technical implementation of blockchain transaction serialization, to interviewing factory owners in Hong Kong or Dhaka to understand the problems they face with existing certification processes. 

Below are a few specific highlights of the work I have performed on ConsenSource.

#### Customer Interviews

Target has access to a wealth of sourcing and supply chain knowledge within the company. However, ConsenSource as a platform cannot be successful without engagement from all four of our user personas.

<span class="highlighted-text">To better understand the needs of these users, I have led a series of qualitative interviews to gather insight as to what pain points exist in the industry around the certification process of factories.</span>

#### Updating The Tech Stack

Much of the early UI work on the project was built as a proof-of-concept, rather than a consumer facing tool. As such, much of my early work on the team was focused around refactoring and enhancing the original interface to better suit our users needs.

<span class="highlighted-text">I led efforts to refactor the ConsenSource UI to use a modern tech stack, including TypeScript, React, and Material UI.</span>


#### Developing An Open-Source TypeScript Interface For Hyperledger Sawtooth

ConsenSource is built using the [Hyperledger Sawtooth](https://www.hyperledger.org/use/sawtooth) blockchain platform. When our team refactored the codebase to use TypeScript, the Sawtooth JavaScript SDK was one of the only packages in our project that did not have TypeScript support.

<span class="highlighted-text">To address this, a teammate and I developed a TypeScript interface for the Hyperledger Sawtooth SDK that is [available on NPM](https://www.npmjs.com/package/@types/sawtooth-sdk).</span>

