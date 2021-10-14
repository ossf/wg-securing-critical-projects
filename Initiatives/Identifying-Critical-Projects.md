# Identifying Critical Projects

Since its first meeting on August 27,2020, the Securing Critical Projects workgroup has encouraged participants, advocates, and the greater open source community to present and discuss research related to Security and Open Source Projects, Supply Chains, and ecosystems. As a result of that research and associated discussions, as well as proposed solutions to Secure Critical Projects, the workgroup curated this document; focused on identifying projects deemed "critical" to the open source ecosystem. 

# List of Identified Projects



# Resources, Data Points, and Supporting Documentation

Here are a few of the various papers and programs that attempt to quantitatively identify the most critical open source software (OSS) projects. The list below is just a sample of the many presentations done and discussions had. For a full overview of the working group presentations and discussions, join the workgroup and view the meeting notes. The workgroup is open to all 

* [*Vulnerabilities in the Core: Preliminary Report and Census II of Open Source Software*](https://www.coreinfrastructure.org/programs/census-program-ii/)
  by Frank Nagle, Jessica Wilkerson, James Dana, and Jennifer L. Hoffman, Linux Foundation & Harvard, February 2020.

This research has resulted in the release of a [preliminary report](https://www.coreinfrastructure.org/programs/census-program-ii/) that identified a list of top 10 most-used JavaScript packages as well as the top 10 most-used Non-JavaScript packages. 
  
* [Open Source Project Criticality Score program](https://github.com/ossf/criticality_score) - a program
  that scores a given OSS project using an algorithm described in
  ["Quantifying Criticality" by Rob Pike](https://github.com/ossf/criticality_score/blob/main/Quantifying_criticality_algorithm.pdf)
  (you can see the [Hacker News Discussion](https://news.ycombinator.com/item?id=25381397))

The Open Source Project Criticality Score has been used to generate a number of lists of open source projects that had the highest criticality scores. The [data generated](https://commondatastorage.googleapis.com/ossf-criticality-score/index.html)from the algorithm ranks the projects with the highest criticality scores by: All (all-time top 200), C top 200, C++ top 200, C# top 200, go top 200, java top 200, and many others. 

* [Core Infrastructure Initiative (CII) Open Source Software Census II Strategy](https://www.ida.org/research-and-publications/publications/all/c/co/core-infrastructure-initiative-cii-open-source-software-census-ii-strategy)
  by David A. Wheeler & Jason N. Dossett, October 2017
* [Open Source Software Projects Needing Security Investments](https://www.coreinfrastructure.org/wp-content/uploads/sites/6/2018/04/pub_ida_lf_cii_070915.pdf)
  by David A. Wheeler & Samir Khakimov, June 19, 2015

 

## Related Work

* [Report on the 2020 FOSS Contributor Survey](https://www.linuxfoundation.org/blog/2020/12/download-the-report-on-the-2020-foss-contributor-survey/),
  by Frank Nagle, David A. Wheeler, Hila Lifshitz-Assaf, Haylee Ham, and Jennifer L. Hoffman,
  The Linux Foundation & The Laboratory for Innovation Science at Harvard

## Proposed Solution: Managed Audit Program

OSTIF, the Open Source Technology Improvement Fund, Inc is an independent non-profit that specializes in facilitating security engagements for open source projects. Responsible for over 3,500 hours of independent review, 147 security fixes and improvements, and 26 Severe Bug Patches, OSTIF compiled a number of data points, including results from the Criticality Score and Census Program II referenced above, to generate a candidate list of 25 Critical Projects that could benefit from OSTIF's work. OSTIF [strategically partnered](https://www.linuxfoundation.org/press-release/new-collaboration-brings-increased-open-source-security-support-and-assurances-to-software-developers/) with Linux Foundation in January 2020 and contributes to the OpenSSF via the Securing Critical Projects and Identifying Security Threats working group.  

The Managed Audit Program was pitched to the Securing Critical Projects workgroup due to the relevance of OSTIF's work in improving the security of critical projects effectively. Via the OpenSSF TAC and Governing Board, OpenSSF approved a pilot grant to improve the security of **php symfony**, a critical and widely used web application framework in September 2021. OSTIF used this grant along with grants secured directly from organizations and foundations to launch the Managed Audit Program. 

More information on the Managed Audut Program can be found [here](https://docs.google.com/spreadsheets/d/1oytKuD7UCX6nDXWQMr6ZgYYgap_SH_JVBof5gNrgSxo/edit#gid=0)
