# WG Securing Critical Projects

This charter describes operations as an [OSSF Technical Initiative](https://github.com/ossf/tac/blob/master/charters/).
The [Focus](#focus) section below describes what is in and out of scope,
and [Governance](#governance) section describes how our operations are consistent with OSSF policies with links to more detailed documents.

**Mission:** TODO

## Motivation

<img align="right" src="https://imgs.xkcd.com/comics/dependency.png">

Open Source Software has long suffered from a "tragedy of the commons" problem.
Organizations large and small make use of OSS every day, but many projects are struggling for the time, resources and attention they need.

This is a resource allocation problem - and we can help solve it together.
We need ways to connect critical projects we all rely on with organizations that can provide them with support.

Whether it is dedicated help from specialized experts or simply grant money or cloud credits, we recognize that no two
projects are the same, and support can come in many shapes.
We intend to work with upstream maintainers to understand what help and support they need, and then develop scalable processes to make
this help available.

## Focus

### Goals

To the best of our efforts, the goals of the working group are:

1. Identify projects critical to the open-source supply chain. 
2. Secure projects critical to the open-souce supply chain.
3. Provide tools and novel solutions for critical open-source projects. 

## Current WG projects

* [criticality_score](https://github.com/ossf/criticality_score) - this attempts to estimate criticality using the algorithm described in ["Quantifying Criticality" by Rob Pike](https://github.com/ossf/criticality_score/blob/main/Quantifying_criticality_algorithm.pdf); you can see the [Hacker News Discussion](https://news.ycombinator.com/item?id=25381397). A known challenge is that it emphasizes activity, and some critical projects aren't active.
* [Harvard research](https://www.coreinfrastructure.org/programs/census-program-ii/)
* [package-feeds](https://github.com/ossf/package-feeds) / [package-analysis](https://github.com/ossf/package-analysis)
* [allstar](https://github.com/ossf/allstar)

## Related work to quantitatively identify critical projects

* [*Vulnerabilities in the Core: Preliminary Report and Census II of Open Source Software*](https://www.coreinfrastructure.org/programs/census-program-ii/) by Frank Nagle, Jessica Wilkerson, James Dana, and Jennifer L. Hoffman, Linux Foundation & Harvard, February 2020.
* [Open Source Software Projects Needing Security Investments](https://www.coreinfrastructure.org/wp-content/uploads/sites/6/2018/04/pub_ida_lf_cii_070915.pdf) by David A. Wheeler & Samir Khakimov, June 19, 2015
* ["The Dark Reality of Open Source Through the Lens of Threat and Vulnerability Management" by Risksense](https://risksense.com/wp-content/uploads/2020/09/RiskSense-Spotlight-The-Dark-Reality-of-Open-Source.pdf), which identifies OSS with the most publicly-reported vulnerabilities reported as CVEs. Having more reported vulnerabilities does not mean that the software is necessarily more vulnerable; it often means that more people are looking for vulnerabilities & that there's a robust process for processing them. However, if so many people are searching for vulnerabilities in a product, that suggests it's an important (critical) project)
* OSTIF's list of critical projects
* [Core Infrastructure Initiative (CII) Open Source Software Census II Strategy](https://www.ida.org/research-and-publications/publications/all/c/co/core-infrastructure-initiative-cii-open-source-software-census-ii-strategy) by David A. Wheeler & Jason N. Dossett, October 2017
* [Report on the 2020 FOSS Contributor Survey](https://www.linuxfoundation.org/blog/2020/12/download-the-report-on-the-2020-foss-contributor-survey/) by Frank Nagle, David A. Wheeler, Hila Lifshitz-Assaf, Haylee Ham, and Jennifer L. Hoffman


## Operations

WG-Securing-Critical-Projects operations are consistent with standard operating guidelines
provided by the OSSF Technical Advisory Committee
[TAC](https://github.com/ossf/tac).

### Meetings

Meetings will all be published on the [OSSF Community Calendar](https://calendar.google.com/calendar/r?cid=s63voefhp5i9pfltb5q67ngpes@group.calendar.google.com).

### Communications

We have a public email list available here: https://lists.openssf.org/g/openssf-wg-securing-crit-prjs

You can also join us for day-to-day conversations on slack: https://openssf.slack.com/messages/wg_securing_critical_projects

#### Notes and Agendas

Meeting Notes and Agendas are available on [Google Drive](https://docs.google.com/document/d/1MIXxadtWsaROpFcJnBtYnQPoyzTCIDhd0IGV8PIV0mQ/edit). (Join the group above to edit.)

Meeting Recordings are available on Youtube at: https://www.youtube.com/playlist?list=PLVl2hFL_zAh-cAfx6y4k-fODfbHeQzb_O.

## Governance

This group is chaired by Amir Montazery (OSTIF) and Jeff Mendoza (Google).

Full details of process and roles are linked from [governance README](/governance).

## Identifying Critical Projects

[See information on identifying critical projects](https://github.com/Amir-Montazery/wg-securing-critical-projects/blob/main/Research-and-Publications/identifying-critical-projects.md)

