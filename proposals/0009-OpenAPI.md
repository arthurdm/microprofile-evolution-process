# OpenAPI

* Proposal: [MP-0009](0009-OpenAPI.md)
* Authors: [Arthur De Magalhaes](https://github.com/arthurdm), [Tony Tam](https://github.com/fehguy)
* Status: **Awaiting review**

*During the review process, add the following fields as needed:*

* Decision Notes: [Discussion thread topic covering the  Rationale](https://groups.google.com/forum/#!topic/microprofile/CXq1h45_HOw)

## Introduction

The [OpenAPI Initiative](https://www.openapis.org/) is a consertium of various industry-leading companies that came together with a goal to standardize the documentation of RESTful APIs.  This specification is called [OpenAPI](https://github.com/OAI/OpenAPI-Specification/blob/OpenAPI.next/versions/3.0.md) (hereon OAS) and it is at version 3 to naturally succeed the contributing specification [Swagger v2](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/2.0.md).

The OAS allows users to fully document their RESTful applications, including all request and response details.  It also allows encapsulating frameworks to optimize traffic routing, security and validation on behalf of the target application.

Mailinglist thread: [Discussion thread topic for that proposal](https://groups.google.com/forum/#!topic/microprofile/CXq1h45_HOw)

## Motivation

The OAS is an essential part of a RESTful microservice but unfortunately the specification is language-agnostic, which means it does not expose a set of annotations or programming models for Java developers. One possible workaround would be to include a pre-generated OpenAPI document (YAML or JSON format) within the Java EE web application, however that does not provide a native programming model for Java developers.  Even 'where' to include a pre-generated OpenAPI document is not prescribed by the OAS.  

Thus, to avoid having dozens of different Java OAS programming models from different vendors, there needs to be a standard set of annotations and interfaces which form a consistent programming model that suits the various Java EE microservices architectures that expose RESTful APIs.


## Proposed solution

The [Swagger repositories](https://github.com/swagger-api) have been the 'de facto' standard for Java Swagger programming models, and they are building a correponding set of interfaces for OAS.  

## Detailed design (if applicable)

Describe the design of the solution in detail. If it involves new
syntax in the language, show the additions and changes to the Microprofile
grammar. If it's a new API, show the full API and its documentation
comments detailing what it does. The detail in this section should be
sufficient for someone who is *not* one of the authors to be able to
reasonably implement the feature.

## Impact on existing code (if applicable)

Describe the impact that this change will have on existing code. Will some
microprofile applications stop compiling due to this change? Will applications still
compile but produce different behavior than they used to? Is it
possible to migrate existing microprofile applications to use a new feature or API automatically?

## Alternatives considered

Describe alternative approaches to addressing the same problem, and
why you chose this approach instead.
