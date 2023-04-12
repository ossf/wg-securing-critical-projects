# WG Securing Critical Projects

This charter describes operations as an [OSSF Technical Initiative](https://github.com/ossf/tac/blob/master/charters/).
The [Focus](#focus) section below describes what is in and out of scope,
and [Governance](#governance) section describes how our operations are consistent with OSSF policies with links to more detailed documents.

## Motivation

<table align="right">
  <tr><td><img align="right" src="https://imgs.xkcd.com/comics/dependency.png"></td></tr>
  <tr><td><a href="https://xkcd.com/2347">Source</a>. Randall Munroe. Licensed under <a href="https://creativecommons.org/licenses/by-nc/2.5/">CC BY-NC 2.5</a></td></tr>
</table>

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

1. Identify critical open source software (OSS) projects. 
2. Secure those projects.


## Current WG SIGs/Projects

* [Securing Critical Projects: List of Critical Open Source Projects, Components, and Frameworks](https://docs.google.com/spreadsheets/d/1ONZ4qeMq8xmeCHX03lIgIYE4MEXVfVL6oj05lbuXTDM/edit) - current version
    * Leads: Amir Montazery and Julia Ferraioli
    * Contributors: David Wheeler, Caleb Brown, Michael Scovetta, Georg Kunz
* [criticality_score](https://github.com/ossf/criticality_score) - this attempts to estimate criticality using the algorithm described in ["Quantifying Criticality" by Rob Pike](https://github.com/ossf/criticality_score/blob/main/Quantifying_criticality_algorithm.pdf); you can see the [Hacker News Discussion](https://news.ycombinator.com/item?id=25381397). A known challenge is that it emphasizes activity, and some critical projects aren't active.
    * Lead: Caleb Brown
* Harvard research - [Census II](https://www.linuxfoundation.org/research/census-ii-of-free-and-open-source-software-application-libraries) [Preliminary Census II](https://www.coreinfrastructure.org/programs/census-program-ii/)
* [package-feeds](https://github.com/ossf/package-feeds)
    * Lead: Caleb Brown
* [package-analysis](https://github.com/ossf/package-analysis)
    * Lead: Caleb Brown
* [allstar](https://github.com/ossf/allstar)
    * Lead: Jeff Mendoza

### Role Definitions

* Lead: Drives work forward
* Contributor: Available for taking work and completing

## How were critical OSS projects selected?

[Securing Critical Projects: List of Critical Open Source Projects, Components, and Frameworks](https://docs.google.com/spreadsheets/d/1ONZ4qeMq8xmeCHX03lIgIYE4MEXVfVL6oj05lbuXTDM/edit) is our current (in progress) list of critical OSS projects.

For our purposes, a critical OSS project is an OSS project that can have
an especially large impact if it has a significant unintentional vulnerability,
or if it is subverted in either its source repository or
distribution package(s).
There are literally millions of open source software (OSS) projects today,
making it difficult to create a focused list of "critical OSS projects".

The list of critical OSS projects was developed for the Great MFA Distribution
Project by the
[OpenSSF Securing Critical Projects Working Group (WG)](https://github.com/ossf/wg-securing-critical-projects).
This OpenSSF working group has been *specifically* working on this problem!

There are many ways to identify "critical" projects, so the
Securing Critical Projects WG combined the results of several different
analyses (the analyses are also called "Selection Criteria"),
The WG then used human group review of this combined set of top candidates
to create a final defensible list. The analyses ("selection criteria") for
identifying candidate critical OSS projects included:

* [OpenSSF Criticality Score](https://github.com/ossf/criticality_score): A top OpenSSF criticality score value. This metric prefers projects that are extremely active on specific forges. Such projects are likely to be important (at least to the participants). However, this is not a perfect measure; some projects will score low here and yet be very critical. Also, it currently only considers GitHub-hosted projects. As of 2021-11-23 the projects with the top scores are node, kubernetes, rust, and spark.
* [Census Program II](https://www.coreinfrastructure.org/programs/census-program-ii/): Harvard preliminary analysis, uses SCA & dependency data. This tends to emphasize lower-level libraries that are depended on, transitively, by many.
* OSTIF Managed Audit Program: Programs OSTIF has recommended for audit. These were selected earlier from research sources, focusing on securing the most critical projects. You can see the [OSTIF Managed Audit Program (MAP25)](https://docs.google.com/spreadsheets/d/1oytKuD7UCX6nDXWQMr6ZgYYgap_SH_JVBof5gNrgSxo/edit#gid=0)
* [Top Google Project](https://opensource.google/projects/list/featured):	Featured on Google Open Source page and widely adopted.
* [Top Microsoft Project](https://opensource.microsoft.com/projects/): Featured on Microsoft Open Source page and widely adopted.
* [Top Linux Foundation Project](https://www.linuxfoundation.org/projects/): 	Featured on Linux Foundation Project page and related to supply chains.
*  Secure Supply Chain Tool: Directly related to supply chain security (identified by WG)
* Survey Response: [Response to public survey](https://forms.gle/19PKPS17zkL5fTFUA)
* Language implementation: Identified by community as a widely-used language implementation
* Community Addition: Separately identified by the community as important.
* Previously subverted: If software has been previously attacked & it made headlines, it must be critical enough to attack.

Every method for identify critical OSS projects has its strengths and
weaknesses; we believe the combination of analysis combined with human review
is better than trying to do any one of them.
For example, high criticality score tends to emphasize very busy projects;
human review can remove projects that are busy but for whatever reason
are less critical.
Some projects are very important yet not active; by using other measures
(not just the OpenSSF criticality score) we can still identify them.

We have no doubt that other OSS projects will be added to the
critical OSS projects list over time. If you're interested in helping
to do that, please join the working group.

## Related work to quantitatively identify critical projects

* [*Vulnerabilities in the Core: Preliminary Report and Census II of Open Source Software*](https://www.coreinfrastructure.org/programs/census-program-ii/) by Frank Nagle, Jessica Wilkerson, James Dana, and Jennifer L. Hoffman, Linux Foundation & Harvard, February 2020.
* [Open Source Software Projects Needing Security Investments](https://www.coreinfrastructure.org/wp-content/uploads/sites/6/2018/04/pub_ida_lf_cii_070915.pdf) by David A. Wheeler & Samir Khakimov, June 19, 2015
* ["The Dark Reality of Open Source Through the Lens of Threat and Vulnerability Management" by Risksense](https://risksense.com/wp-content/uploads/2020/09/RiskSense-Spotlight-The-Dark-Reality-of-Open-Source.pdf), which identifies OSS with the most publicly-reported vulnerabilities reported as CVEs. Having more reported vulnerabilities does not mean that the software is necessarily more vulnerable; it often means that more people are looking for vulnerabilities & that there's a robust process for processing them. However, if so many people are searching for vulnerabilities in a product, that suggests it's an important (critical) project)
* OSTIF's list of critical projects for Managed Audit Program (link to more info [here.](https://docs.google.com/spreadsheets/d/1oytKuD7UCX6nDXWQMr6ZgYYgap_SH_JVBof5gNrgSxo/edit#gid=0)
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

This group is chaired by Amir Montazery (OSTIF) and Jeff Mendoza (Kusari).

Full details of process and roles are linked from [governance README](/governance).

## Identifying Critical Projects

[See information on identifying critical projects](https://github.com/ossf/wg-securing-critical-projects/tree/main/Initiatives/Identifying-Critical-Projects)

## Antitrust policy

Linux Foundation meetings involve participation by industry competitors, and it is the intention of the Linux Foundation to conduct all of its activities in accordance with applicable antitrust and competition laws. It is therefore extremely important that attendees adhere to meeting agendas, and be aware of, and not participate in, any activities that are prohibited under applicable US state, federal or foreign antitrust and competition laws.

Examples of types of actions that are prohibited at Linux Foundation meetings and in connection with Linux Foundation activities are described in the Linux Foundation Antitrust Policy available at <http://www.linuxfoundation.org/antitrust-policy>. If you have questions about these matters, please contact your company counsel, or if you are a member of the Linux Foundation, feel free to contact Andrew Updegrove of the firm of Gesmer Updegrove LLP, which provides legal counsel to the Linux Foundation.
