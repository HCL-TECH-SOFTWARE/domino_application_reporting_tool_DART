---
layout: default
title: "Requirements"
parent: "Home"
nav_order: 3
description: "System Requirements"
has_children: false
---

<h1>System Requirements</h1>
The following requirements must be met in order to run HCL DART.

<details close markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---

## Software

- Windows 7 or higher
- Notes Client version 12.0.2 or higher
- Domino Server version 12.0 or higher

## Access Rights

- READ access to the Domino Directory
- EDITOR access to the system databases<sup><a href="#systemapps">1</a></sub>
- Domino servers must have at least Designer access to the custom Domino applicaitons that reside on them
- Group membership in the "LocalDomainAdmins" Group or at least Editor access to the system databases<sup><a href="#systemapps">1</a></sup>

<sup id="systemapps">
1 - The list of applications the user needs access to are:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- names.nsf<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- log.nsf<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- catalog.nsf
</sup>

## Server Specific Requirements

* Main HCL DART server must be running Windows OS with HCL Domino V12.x
* Main HCL DART server must have the HTTP Task running with a properly obtained internet certificate
* If you intend on using the web interface in HCL DART, the main HCL Domino server must be running the HTTP task
* If you require usage information for web-based HCL Domino application, the "Domino Web Server Log" must be enabled and collecting informaiton on each HCL Domino server where the web-based applications are being accessed. For assistance setting up the Domino Web Server Log, please follow the steps in the [HCL Documentation](https://help.hcl-software.com/domino/12.0.0/admin/admn_thedominowebserverlogdomlognsf_c.html){:target="_blank2"}
* Domino Directory must have the following groups:
  * "LocalDomainServers" (with all Domino servers listed that HCL DART will be scanning)
  * "LocalDomainAdmins" (with all Domino Admins that will be accessing the HCL DART app)
  * Both Groups need to have the ability to Create new Databases and Replicas on the Domino servers

## Notes Client Specific Requirements

* The user needs Administration rights to all Domino servers that HCL DART will be scanning
* The user who is installing DART needs to have the ability to create new databases and replicas on ALL the Domino servers that will be scanned by HCL DART
* The user who is deploying/upgrading HCL DART needs the following “Programmability Restrictions” security rights to the Domino servers being scanned (configured on the Domino Server document’s “Security” tab):
  * Sign or run unrestricted methods and operations
  * Sign agents to run on behalf of someone else
  * Sign agents or XPages to run on behalf of the invoker
  * Sign or run restricted LotusScript/Java agents
