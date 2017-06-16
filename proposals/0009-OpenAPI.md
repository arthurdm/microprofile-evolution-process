# OpenAPI

* Proposal: [MP-0009](0009-OpenAPI.md)
* Authors: [Arthur De Magalhaes](https://github.com/arthurdm), [Tony Tam](https://github.com/fehguy)
* Status: **Awaiting review**

*During the review process, add the following fields as needed:*

* Decision Notes: [Discussion thread topic covering the  Rationale](https://groups.google.com/forum/#!topic/microprofile/CXq1h45_HOw)

## Introduction

The [OpenAPI Initiative](https://www.openapis.org/) is a consertium of various industry-leading companies that came together with a goal to standardize the documentation of RESTful APIs.  This standard is called [OpenAPI](https://github.com/OAI/OpenAPI-Specification/blob/OpenAPI.next/versions/3.0.md) and it is at version 3 to naturally succeed the contributing specification [Swagger v2](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/2.0.md).

This specification allows users to fully document their RESTful applications, including all request and response details.  It also allows encapsulating frameworks to optimize traffic routing, security and validation on behalf of the target application.

Mailinglist thread: [Discussion thread topic for that proposal](https://groups.google.com/forum/#!topic/microprofile/CXq1h45_HOw)

## Motivation

Describe the problems that this proposal seeks to address. If the
problem is that some common pattern is currently hard to express, show
how one can currently get a similar effect and describe its
drawbacks. If it's completely new functionality that cannot be
emulated, motivate why this new functionality would help Java EE developers to develop and operate microservice architectures.

## Proposed solution

Describe your solution to the problem. Provide examples and describe
how they work. Show how your solution is better than current
workarounds: is it cleaner, safer, or more efficient?

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
