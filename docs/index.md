---
layout: default
title: "Home"
nav_order: 1
description: "HCL Domino Application Reporting Tool"
has_children: true
---

[Download Latest Release](https://github.com/HCL-TECH-SOFTWARE/dominio_application_reporting_tool_DART/releases/latest){: .btn .btn-green }
[View on GitHub](https://github.com/HCL-TECH-SOFTWARE/dominio_application_reporting_tool_DART/){: .btn }

<h1> HCL Domino Application Reporting Tool (DART)</h1>

## Purpose
Here’s a typical scenario: Your organization has HCL Domino, and it “just runs”. Some of your Business Critical apps are running on HCL Domino. But you have a tonne of questions about the Domino environment and the custom Domino apps:

* What are they?
* How frequently are they being used?
* How complex are they?
* What should be done with them?

This is where HCL DART comes into the picture. 


<details close markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>
___
## How It Works

HCL DART is a fully self-contained Domino based application that can be placed into your environment, that will immediately begin analyzing your custom HCL Domino applications. It will report on which Domino applications are in use, how frequently they are being used, how much data is contained in each application, and determine the complexity of the design for each.

HCL DART is accessed through an easy to use, simple to understand web interface. There is no need for a HCL Notes Client to access the reports that are created.

HCL DART is built in such a way that it will begin providing reports and information about your HCL Domino environment within minutes, not days or weeks if done manually.

HCL DART assists organizations in determining what to do with their custom Domino applications

* Infrequent: If an application has no usage and is of little use in your business processes, HCL DART will indicate if the application can be archived for data retention purposes.

* Indispensable: If an application is heavily used, and it is determined that the design is highly complex, HCL DART will recommend that the application be kept on the Domino server. HCL DART will also perform a HCL Nomad Compatibility Check to see if there will be any problems running the application in an alternate environment (web browser, smartphone, or tablet)

* Improve: If an application is moderately used, has a medium to high complexity to its design, and is not used for “Mission Critical” events, then HCL DART will recommend keeping the application on the Domino platform, but also recommends “refreshing” the user experience. Using Domino Restyle to modernize the UI/UX in these applications will be presented as the best option

* Invest: If an application is heavily used and has medium complexity, HCL DART recommends that the application be replatformed to HCL VoltMX. HCL DART will include a set of Developer Tools to help “jumpstart” the transition into HCL VoltMX. HCL DART will enable these applications for use with the Domino REST APIs and provide a set of design artifacts to assist a non-Domino developer in understanding what is happening, allowing them to focus on the transition to the new platform instead of learning how to design an application in Domino.


<div style="visibility:hidden">
## Intro

{% include youtube.html id="zBPAdHMGzzo" %}
</div>

## Documentation
Learn how to use HCL DART with these topics:

* [Step-by-Step Deployment Instructions](instructions.md)
* [Understanding the Results](results.md)
* [Frequently Asked Questions](faqs.md)
* [Limitations](limitations.md)

## Compatibilty

see [System Requirements](requirements.md)


## Changes

Be sure to review the changes that are included in this release by opening the [CHANGE LOG](changelog.md)