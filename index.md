---
title: Introduction to the Care Connect Get Unstructured Document API
keywords: homepage
tags: [overview]
sidebar: overview_sidebar
permalink: index.html
toc: false
summary: A brief introduction to he Get Unstructured Document API
---

# Introduction #

<!--
This is the Care Connect Get Unstructured Document RESTful FHIR STU3 ‘Read Only’ experimental API implementation guide. It is a component specification of the Care Connect API (CCAPI) suite. 
-->

The Get Unstructured Document RESTful FHIR STU3 'experimental' API implementation guide is a component of the Care Connect API (CCAPI) specification suite. 

This utility ‘Read Only’ API uses the ‘Get Binary Retrieval Pattern’ to support Consumer retrieval of non-structured documents such as a PDFs from remote Provider systems.

It is expected that this API will be piloted in early 2019 using the End Of Life FHIR STU3 content API.

## In Scope ##
This implementation guide defines the API requirements applicable to Provider systems sharing and Consumer systems retrieving ‘non-structured’ documents via a RESTful FHIR interface. The experimental API supports:
 - FHIR STU3 standard
 - Document retrieval (not discovery)
 - RESTful Pull interaction pattern
 - Simple READ ONLY functionality
 - Binary content restricted to any content that is not represented using FHIR resources (e.g. PDFs, PNGs, Work Documents etc).

For the experimental API the following assumptions apply:
 - It is assumed that Consumer systems will discover ‘non-structured’ document availability published by Provider systems using the NRLS or other federated services. 
 - Consumer systems MUST handle dynamic generation of binary content
 - Security & Access Control is no different to other NHS Digital FHIR APIs

## Out of Scope ##
The following is out of scope for the experimental API:
 - Advanced READ functionality
 - Creation of FHIR Binary resource (not part of retrieval API)
 - Binary registry/ repository pattern (i.e. NRLS/ IHE MHD profile)
 - Business error response codes
 - National Record Locator (NRLS) Phase 2 
 - Consumer system downstream processing capability/ expectations e.g. automated attachment/filing to the patient’s care record 
 - Security - options on where this is applied i.e. SSP, Provider/ Consumer endpoints
 - Integration with Spine
   - Authentication/ Authorisation
   - Access tokens & Audit (JWT)
 - The Spine Security Proxy (SSP)
   - certificates
   - data audit: such as clinical/ IG implications
   - transaction throttling
   - Consumer request options e.g. URL patterns
   - Request Headers e.g. traceID, system ASIDs, InteractionID etc


<!--

# Using this guide #

This guide has been created to support the adoption of the "your project here" profiles and FHIR resources. As such the site is structured around stakeholders including API users, developers and architects, who have an interest in implementing the "your project here"

Need to add include here....

-->
