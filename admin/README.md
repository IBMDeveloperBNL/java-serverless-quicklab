# Administrator Guide

This document is meant as guide for someone intending to run this quicklab at a conference. This guide offers advice on how to setup and configure laptops to run this quicklab, solutionss to common problems, and general advice on how to make the running of this quicklab more smooth. 

For questions about this quicklab reach out to Billy Korando:

Email: william dot korando @ ibm dot com<br/>
Slack: @billy<br/>
Twitter: @BillyKorando<br/>

## Before You Run the Quicklab for the First Time

If you are planning on running this quicklab here are some of the things you should do: 

1. Run through the quicklab yourself... duh! (don't do this on your IBM account!)
2. Familiarize yourself with Serverless (also duh!)
3. Fork this repo, you will likely need to make some minor changes to fit this quicklab to the needs of your conference (See: [Before You Start the Conference Starts]())
3. Be a good teammate, if you run into an issue that isn't covered in this guide or see an opportunity for improvement update this guide or the workshop itself and submit a PR to Billy Korando. 


## Before You Start the Conference Starts

Be sure to run through these steps before starting the workshop!

1. Update IBM Cloud creation link with VCPI for workshop 
2. Whitelist IP 
3. Update the "hello world" value to the conference name

## Pre-Requisites

## Prerequisites: 

Here are the steps for configuring a Mac machine for this quicklab
  
1. Install Java 8+

	```
	brew cask install java
	```
2. [Install IBM Cloud CLI](https://github.com/IBM-Cloud/ibm-cloud-cli-release/releases/)
3. Install IBM Cloud Functions Plugin

	```
	ibmcloud plugin install cloud-functions
	```
4. Install git
	```
	brew install git
	```	 

## Common Problems

These are issues commonly encountered when running this lab:

### Pre-Existing IBM Account

<details>
  <summary>User has an Expired IBM Account</summary>
  If a user has an expired/lapsed IBM account it can be reactivated using a promo code. 
</details>


### Blank Region When Invoking Actions

<details>
  <summary>User attempts to invoke action, but gets response saying region is blank</summary>
  Sometimes an user, even if they run `target --cf` and select a region, will still run into issues when attempting to invoke actions. Steps to resolve:
  1. Run: `ibmcloud target -r REGION` see above for region list 
</details>

