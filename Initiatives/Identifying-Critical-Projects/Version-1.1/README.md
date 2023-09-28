# Set of Critical Open Source Projects

_by the Open Source Security Foundation (OpenSSF) Securing Critical Projects
Working Group_

## Introduction

This document presents the “Critical Open Source Software Projects”, aka,
“Critical Projects”, as of 2023, which represents a point-in-time analysis from
2022-June 2023. This identifies a set of open source software (OSS) projects
that have been determined to be highly important by the Open Source Security
Foundation (OpenSSF) Securing Critical Projects Working Group through the
process described below. This set is intended as a starting point for
conversation about Open Source projects that are integral to the Internet,
whose health should be monitored, and who are potential candidates for
additional investment.

## Description, high level

The purpose of the “Set of Critical Projects'' is to help guide the open source
community in determining highly important open source projects that have been
identified through research and discussion as critical with the Securing
Critical Projects Working work group. These include projects under OSI-approved
licenses that have such extensive use that vulnerabilities (unintentional or
malicious) in that software could cause widespread problems, both in
significance or breadth.

This is _not_ a list, it is a set. This set is listed in alphabetical order by
project name; there is no implied ordering within the set. It was challenging
to determine what was or was not in the set; ranking between these projects
would have been even more difficult and was unnecessary for our purposes.

This set of projects are projects that the working group has deemed
critical. It is not a set of “top” or “most” critical projects. The working
group has not considered or evaluated all projects in existence. We have
strived to cast a wide net and incorporate a variety of sources for discovering
projects. Any omission of a project may be due to the project not being
considered, and is not an assertion that the project is not critical.

Please note that this is not a list of “OSS projects in trouble”. In fact,
being on this list is a sign of success, as it indicates that many are
depending on that project’s software.

## Set Creation Process

The overall process used in creating the set included two primary steps:

1. Find projects for consideration and gather data.
2. Evaluate projects in a working group meeting.

### Find

There are many ways to discover "critical" projects, so the Securing Critical
Projects WG combined the results of several different analyses (aka the
"Selection Criteria"). The analyses ("selection criteria") for identifying
candidate critical OSS projects included:

* [OpenSSF Criticality Score](https://github.com/ossf/criticality_score): A top
  OpenSSF criticality score value. This metric prefers projects that are
  extremely active. Such projects are likely to be important (at least to the
  participants). However, note that widely-used but less-active projects will
  score low here (a limitation [others have pointed
  out](https://ieeexplore.ieee.org/document/9463111)). Also, it currently only
  considers GitHub-hosted projects. Due to the nature of the score, we used it
  to discover and identify projects for consideration, and factored it into our
  discussion, however we didn’t consider a low score a reason for a project to
  not be considered critical.

* [Census II
  Program](https://www.linuxfoundation.org/research/census-ii-of-free-and-open-source-software-application-libraries):
  This is [Harvard Census II of Free and Open Source Software — Application
  Libraries](https://www.linuxfoundation.org/research/census-ii-of-free-and-open-source-software-application-libraries)
  report. This uses data from multiple SCAs and dependency data to identify
  widely-used OSS. This analysis tends to emphasize lower-level application
  libraries that are depended on, transitively, by many. We also used the
  preliminary [Census Program
  II](https://www.coreinfrastructure.org/programs/census-program-ii/) document
  until the final version was available.

* OSTIF Managed Audit Program: Programs OSTIF has recommended for audit. These
  were selected earlier from research sources, focusing on securing the most
  critical projects. You can see the [OSTIF Managed Audit Program
  (MAP25)](https://docs.google.com/spreadsheets/d/1oytKuD7UCX6nDXWQMr6ZgYYgap_SH_JVBof5gNrgSxo/edit#gid=0)

* [Featured Google Project](https://opensource.google/projects): Featured on
  Google Open Source page and widely adopted.

* [Featured Microsoft Project](https://opensource.microsoft.com/projects/):
  Featured on Microsoft Open Source page and widely adopted.

* [Featured Linux Foundation
  Project](https://www.linuxfoundation.org/projects/): Featured on Linux
  Foundation Project page.

* Secure Supply Chain Tool: Directly related to supply chain security (as
  identified by the WG)

* Survey Response: [Response to public
  survey](https://forms.gle/19PKPS17zkL5fTFUA)

* Language implementation: Identified by community as a widely-used language
  implementation

* Community Addition: Separately identified by the community as important.

* Widely Covered: If software has been previously attacked & it made headlines,
  it must be critical enough to attack.

### Evaluation

The selection criteria used to find projects above was sometimes used as an
evaluation factor to support a project being critical. Values like download
counts, or criticality score are generally in support of a project’s widespread
or important use. We also knew to not consider an absence of these things as
reasoning for a project to not be critical, for example a project not on GitHub
wouldn't have a criticality score, but that would not be held against the
project.

Generally in classes of software (ex: databases), we would set a high bar for
ubiquitous use, and only include a top number of those types of
projects. Another factor discussed was the exposure that project or type of
software has in a typical software system. For example, an http server or load
balancer is typically exposed directly to the internet, while a basic library
may be separated by many layers from untrusted input.

Using a combination of supporting metrics, known widespread use, and system
criticality the working group came to a consensus for each package to be
considered critical or not.

## Wrapup

**Limitations of this Set**: We used these things as initial input. It wasn’t a
matter of considering it comprehensive, we just used different inputs to the
best of our abilities within the time frame we worked with. We understand that
many other factors can influence or determine a project’s criticality, and that
our set would not be comprehensive.

Every method for identifying critical OSS projects has its strengths and
weaknesses. We believe the combination of quantitative analysis, combined with
human review by a group, is better than only applying one analysis
approach. For example, a high criticality score tends to emphasize very busy
projects; human review can remove projects that are busy but for whatever
reason are less critical (e.g., because they are not widely depended on or
because vulnerabilities in it are unlikely to cause significant harm). Also,
some projects are very important yet not active; by using other measures (not
just the OpenSSF criticality score) we can still identify them.

The set represents a snapshot in time and was based on the proposed projects
and analysis at the time of creation.  We have no doubt that other OSS projects
will be added to the critical OSS projects list over time. There are millions
of OSS projects; all are important to someone, and it is challenging to review
those millions to find which ones are widely depended on. If you're interested
in helping to do that, please [join the working
group](https://github.com/ossf/wg-securing-critical-projects).

The set gravitated to OSS projects related to server-side Internet
functionality, not other regimes, such as embedded, edge, safety critical, life
critical, financial, etc. that may utilize Open Source software. Those areas
were not excluded intentionally, and would be welcome to be considered for
inclusion in the set.

Being a set of only Open Source projects, only the OSI approved license version
of a project was considered for inclusion when there were multiple versions of
a project. For example, some projects have an Open Source licensed version and
a parallel commercially licensed version. Although the non-OSI version might be
widely used or “critical”, if the Open Source version was not widely used, the
project would not be deemed critical.

# The Set

| Project Name                               | Home Page or Source Repository                                                                                                                                                                                                                                                                 |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| alpine                                     | [](https://www.alpinelinux.org/)[https://www.alpinelinux.org/](https://www.alpinelinux.org/)                                                                                                                                                                                                      |
| AMP Project                                | [](http://github.com/ampproject)[https://github.com/ampproject](http://github.com/ampproject)                                                                                                                                                                                                     |
| Android                                    | [](https://source.android.com/)[https://source.android.com/](https://source.android.com/)                                                                                                                                                                                                         |
| angular                                    | [](http://github.com/angular/angular)[https://github.com/angular/angular](http://github.com/angular/angular)                                                                                                                                                                                      |
| ansible                                    | [](http://github.com/ansible/ansible)[https://github.com/ansible/ansible](http://github.com/ansible/ansible)                                                                                                                                                                                      |
| ant-design                                 | [](http://github.com/ant-design/ant-design)[https://github.com/ant-design/ant-design](http://github.com/ant-design/ant-design)                                                                                                                                                                    |
| Apache httpd                               | [](https://github.com/apache/httpd)[https://github.com/apache/httpd](https://github.com/apache/httpd)                                                                                                                                                                                             |
| ARM Trusted Firmware                       | [](https://github.com/ARM-software/arm-trusted-firmware)[https://github.com/ARM-software/arm-trusted-firmware](https://github.com/ARM-software/arm-trusted-firmware)                                                                                                                              |
| async                                      | [](http://github.com/caolan/async)[https://github.com/caolan/async](http://github.com/caolan/async)                                                                                                                                                                                               |
| autotools                                  | [](https://github.com/autotools-mirror)[https://github.com/autotools-mirror](https://github.com/autotools-mirror)                                                                                                                                                                                 |
| babel                                      | [](https://github.com/babel/babel)[https://github.com/babel/babel](https://github.com/babel/babel)                                                                                                                                                                                                |
| bash                                       | [https://www.gnu.org/software/bash/](https://www.gnu.org/software/bash/)                                                                                                                                                                                                                          |
| bitwarden                                  | [https://bitwarden.com/](https://bitwarden.com/)                                                                                                                                                                                                                                                  |
| bootstrap                                  | [](https://github.com/twbs/bootstrap)[https://github.com/twbs/bootstrap](https://github.com/twbs/bootstrap)                                                                                                                                                                                       |
| brew                                       | [](https://github.com/Homebrew/brew)[https://github.com/Homebrew/brew](https://github.com/Homebrew/brew)                                                                                                                                                                                          |
| buildroot                                  | [https://buildroot.org/](https://buildroot.org/)                                                                                                                                                                                                                                                  |
| busybox                                    | [https://busybox.net/](https://busybox.net/)                                                                                                                                                                                                                                                      |
| cassandra                                  | [](https://cassandra.apache.org/_/index.html)[https://cassandra.apache.org/_/index.html](https://cassandra.apache.org/_/index.html)                                                                                                                                                               |
| ceph                                       | [](https://github.com/ceph/ceph)[https://github.com/ceph/ceph](https://github.com/ceph/ceph)                                                                                                                                                                                                      |
| Chromium                                   | [](https://github.com/chromium/chromium)[https://github.com/chromium/chromium](https://github.com/chromium/chromium)                                                                                                                                                                              |
| cmake                                      | [](https://github.com/Kitware/CMake)[https://github.com/Kitware/CMake](https://github.com/Kitware/CMake)                                                                                                                                                                                          |
| coa                                        | [](https://github.com/veged/coa/issues/99)[https://github.com/veged/coa](https://github.com/veged/coa/issues/99)                                                                                                                                                                                  |
| commons-codec                              | [](https://github.com/apache/commons-codec)[https://github.com/apache/commons-codec](https://github.com/apache/commons-codec)                                                                                                                                                                     |
| commons-io                                 | [](http://github.com/apache/commons-io)[https://github.com/apache/commons-io](http://github.com/apache/commons-io)                                                                                                                                                                                |
| commons-lang3                              | [](http://github.com/apache/commons-lang)[https://github.com/apache/commons-lang](http://github.com/apache/commons-lang)                                                                                                                                                                          |
| core                                       | [](https://github.com/home-assistant/core)[https://github.com/home-assistant/core](https://github.com/home-assistant/core)                                                                                                                                                                        |
| core-utils                                 | [](https://www.gnu.org/software/coreutils/)[https://www.gnu.org/software/coreutils/](https://www.gnu.org/software/coreutils/)                                                                                                                                                                     |
| cpython                                    | [](https://github.com/python/cpython)[https://github.com/python/cpython](https://github.com/python/cpython)                                                                                                                                                                                       |
| curl                                       | [](https://github.com/curl/curl)[https://github.com/curl/curl](https://github.com/curl/curl)                                                                                                                                                                                                      |
| DefinitelyTyped                            | [](https://github.com/DefinitelyTyped/DefinitelyTyped)[https://github.com/DefinitelyTyped/DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped)                                                                                                                                    |
| distribution (formerly knows as: registry) | [https://github.com/distribution/distribution](https://github.com/distribution/distribution)                                                                                                                                                                                                      |
| drupal                                     | [](https://github.com/drupal/drupal)[https://github.com/drupal/drupal](https://github.com/drupal/drupal)                                                                                                                                                                                          |
| Eclipse Mosquitto                          | [](https://mosquitto.org/)[https://mosquitto.org/](https://mosquitto.org/)                                                                                                                                                                                                                        |
| Electron                                   | [](https://github.com/electron/electron)[https://github.com/electron/electron](https://github.com/electron/electron)                                                                                                                                                                              |
| Firefox                                    | [](https://www.mozilla.org/en-US/firefox/)[https://www.mozilla.org/en-US/firefox/](https://www.mozilla.org/en-US/firefox/)                                                                                                                                                                        |
| flutter                                    | [](https://github.com/flutter/flutter)[https://github.com/flutter/flutter](https://github.com/flutter/flutter)                                                                                                                                                                                    |
| gatsby                                     | [](https://github.com/gatsbyjs/gatsby)[https://github.com/gatsbyjs/gatsby](https://github.com/gatsbyjs/gatsby)                                                                                                                                                                                    |
| GCC                                        | [](https://gcc.gnu.org/)[https://gcc.gnu.org/](https://gcc.gnu.org/)                                                                                                                                                                                                                              |
| git                                        | [](https://git-scm.com/)[https://git-scm.com/](https://git-scm.com/)                                                                                                                                                                                                                              |
| glibc                                      | [](https://www.gnu.org/software/libc/libc.html)[https://www.gnu.org/software/libc/libc.html](https://www.gnu.org/software/libc/libc.html)                                                                                                                                                         |
| GNU make                                   | [https://www.gnu.org/software/make/](https://www.gnu.org/software/make/)                                                                                                                                                                                                                          |
| gnupg                                      | [](https://gnupg.org/)[https://gnupg.org/](https://gnupg.org/)                                                                                                                                                                                                                                    |
| go                                         | [](https://go.googlesource.com/go)[https://go.googlesource.com/go](https://go.googlesource.com/go)                                                                                                                                                                                                |
| gradle                                     | [](https://github.com/gradle/gradle)[https://github.com/gradle/gradle](https://github.com/gradle/gradle)                                                                                                                                                                                          |
| grafana                                    | [](https://github.com/grafana/grafana)[https://github.com/grafana/grafana](https://github.com/grafana/grafana)                                                                                                                                                                                    |
| grub                                       | [](https://www.gnu.org/software/grub/)[https://www.gnu.org/software/grub/](https://www.gnu.org/software/grub/)                                                                                                                                                                                    |
| guava                                      | [](https://github.com/google/guava)[https://github.com/google/guava](https://github.com/google/guava)                                                                                                                                                                                             |
| HAProxy                                    | [](https://www.haproxy.org/)[https://www.haproxy.org/](https://www.haproxy.org/)                                                                                                                                                                                                                  |
| homebrew-cask                              | [](https://github.com/Homebrew/homebrew-cask)[https://github.com/Homebrew/homebrew-cask](https://github.com/Homebrew/homebrew-cask)                                                                                                                                                               |
| homebrew-core                              | [](https://github.com/Homebrew/homebrew-core)[https://github.com/Homebrew/homebrew-core](https://github.com/Homebrew/homebrew-core)                                                                                                                                                               |
| httpcomponents-client                      | [](https://github.com/apache/httpcomponents-client)[https://github.com/apache/httpcomponents-client](https://github.com/apache/httpcomponents-client)                                                                                                                                             |
| httpcomponents-core                        | [](https://github.com/apache/httpcomponents-core)[https://github.com/apache/httpcomponents-core](https://github.com/apache/httpcomponents-core)                                                                                                                                                   |
| inherits                                   | [](http://github.com/isaacs/inherits)[https://github.com/isaacs/inherits](http://github.com/isaacs/inherits)                                                                                                                                                                                      |
| isarray                                    | [](http://github.com/juliangruber/isarray)[http://github.com/juliangruber/isarray](http://github.com/juliangruber/isarray)                                                                                                                                                                        |
| jackson-core                               | [](https://github.com/FasterXML/jackson-core)[https://github.com/FasterXML/jackson-core](https://github.com/FasterXML/jackson-core)                                                                                                                                                               |
| jackson-databind                           | [](https://github.com/FasterXML/jackson-databind)[https://github.com/FasterXML/jackson-databind](https://github.com/FasterXML/jackson-databind)                                                                                                                                                   |
| jenkins                                    | [](https://www.jenkins.io/)[https://www.jenkins.io/](https://www.jenkins.io/)                                                                                                                                                                                                                     |
| joomla                                     | [](https://github.com/joomla/joomla-cms)[https://github.com/joomla/joomla-cms](https://github.com/joomla/joomla-cms)                                                                                                                                                                              |
| julia                                      | [](https://github.com/JuliaLang/julia)[https://github.com/JuliaLang/julia](https://github.com/JuliaLang/julia)                                                                                                                                                                                    |
| Kata Containers                            | [](https://katacontainers.io/)[https://katacontainers.io/](https://katacontainers.io/)                                                                                                                                                                                                            |
| keycloak                                   | [](https://www.google.com/url?q=https://www.keycloak.org/&sa=D&source=editors&ust=1648159614004390&usg=AOvVaw2TuVmwjfCjtX98VxskSjsh)[https://www.keycloak.org/](https://www.google.com/url?q=https://www.keycloak.org/&sa=D&source=editors&ust=1648159614004390&usg=AOvVaw2TuVmwjfCjtX98VxskSjsh) |
| kind-of                                    | [](http://github.com/jonschlinkert/kind-of)[http://github.com/jonschlinkert/kind-of](http://github.com/jonschlinkert/kind-of)                                                                                                                                                                     |
| Knative                                    | [](https://github.com/knative/community)[https://github.com/knative/community](https://github.com/knative/community)                                                                                                                                                                              |
| kong                                       | [](https://konghq.com/)[https://konghq.com/](https://konghq.com/)                                                                                                                                                                                                                                 |
| kubernetes                                 | [](https://github.com/kubernetes/kubernetes)[https://github.com/kubernetes/kubernetes](https://github.com/kubernetes/kubernetes)                                                                                                                                                                  |
| KVM Hypervisor                             | [](https://www.linux-kvm.org/page/Main_Page)[https://www.linux-kvm.org/page/Main_Page](https://www.linux-kvm.org/page/Main_Page)                                                                                                                                                                  |
| laravel                                    | [](https://github.com/laravel/framework)[https://github.com/laravel/framework](https://github.com/laravel/framework)                                                                                                                                                                              |
| libarchive                                 | [](https://www.libarchive.org/)[https://www.libarchive.org/](https://www.libarchive.org/)                                                                                                                                                                                                         |
| libjpeg                                    | [](https://libjpeg.sourceforge.net/)[https://libjpeg.sourceforge.net/](https://libjpeg.sourceforge.net/)                                                                                                                                                                                          |
| libpng                                     | [](http://www.libpng.org/pub/png/libpng.html)[http://www.libpng.org/pub/png/libpng.html](http://www.libpng.org/pub/png/libpng.html)                                                                                                                                                               |
| linux                                      | [](https://www.kernel.org/)[https://www.kernel.org/](https://www.kernel.org/)                                                                                                                                                                                                                     |
| llvm                                       | [](https://github.com/llvm)[https://github.com/llvm](https://github.com/llvm)                                                                                                                                                                                                                     |
| lodash                                     | [](https://github.com/lodash/lodash)[https://github.com/lodash/lodash](https://github.com/lodash/lodash)                                                                                                                                                                                          |
| log4j                                      | [](https://github.com/apache/logging-log4j2)[https://github.com/apache/logging-log4j2](https://github.com/apache/logging-log4j2)                                                                                                                                                                  |
| logback-core                               | [](http://github.com/qos-ch/logback)[http://github.com/qos-ch/logback](http://github.com/qos-ch/logback)                                                                                                                                                                                          |
| magento2                                   | [](https://github.com/magento/magento2)[https://github.com/magento/magento2](https://github.com/magento/magento2)                                                                                                                                                                                 |
| make                                       | [](https://www.gnu.org/software/make/)[https://www.gnu.org/software/make/](https://www.gnu.org/software/make/)                                                                                                                                                                                    |
| MariaDB                                    | [](https://github.com/mariadb)[https://github.com/mariadb](https://github.com/mariadb)                                                                                                                                                                                                            |
| material-ui                                | [](https://github.com/mui-org/material-ui)[https://github.com/mui-org/material-ui](https://github.com/mui-org/material-ui)                                                                                                                                                                        |
| Maven                                      | [](https://github.com/apache/maven)[https://github.com/apache/maven](https://github.com/apache/maven)                                                                                                                                                                                             |
| mbedTLS                                    | [](https://www.trustedfirmware.org/projects/mbed-tls/)[https://www.trustedfirmware.org/projects/mbed-tls/](https://www.trustedfirmware.org/projects/mbed-tls/)                                                                                                                                    |
| memcached                                  | [](https://www.memcached.org/)[https://www.memcached.org/](https://www.memcached.org/)                                                                                                                                                                                                            |
| meson                                      | [](https://github.com/mesonbuild/meson)[https://github.com/mesonbuild/meson](https://github.com/mesonbuild/meson)                                                                                                                                                                                 |
| minimist                                   | [](http://github.com/substack/minimist)[http://github.com/substack/minimist](http://github.com/substack/minimist)                                                                                                                                                                                 |
| Mozilla nss                                | [](https://wiki.mozilla.org/NSS)[https://wiki.mozilla.org/NSS](https://wiki.mozilla.org/NSS)                                                                                                                                                                                                      |
| musl                                       | [](https://www.musl-libc.org/)[https://www.musl-libc.org/](https://www.musl-libc.org/)                                                                                                                                                                                                            |
| MySQL                                      | [](https://github.com/mysql)[https://github.com/mysql](https://github.com/mysql)                                                                                                                                                                                                                  |
| natives                                    | [](http://github.com/addaleax/natives)[http://github.com/addaleax/natives](http://github.com/addaleax/natives)                                                                                                                                                                                    |
| NGINX                                      | [](https://github.com/nginx/nginx)[https://github.com/nginx/nginx](https://github.com/nginx/nginx)                                                                                                                                                                                                |
| nixpkgs                                    | [](https://github.com/NixOS/nixpkgs)[https://github.com/NixOS/nixpkgs](https://github.com/NixOS/nixpkgs)                                                                                                                                                                                          |
| node.js                                    | [](https://github.com/nodejs/node)[https://github.com/nodejs/node](https://github.com/nodejs/node)                                                                                                                                                                                                |
| Npm                                        | [](https://www.npmjs.com/)[https://www.npmjs.com/](https://www.npmjs.com/)                                                                                                                                                                                                                        |
| numpy                                      | [](https://github.com/numpy/numpy)[https://github.com/numpy/numpy](https://github.com/numpy/numpy)                                                                                                                                                                                                |
| OpenJDK                                    | [](https://github.com/openjdk/)[https://github.com/openjdk/](https://github.com/openjdk/)                                                                                                                                                                                                         |
| OpenSSH                                    | [](https://www.openssh.com/)[https://www.openssh.com/](https://www.openssh.com/)                                                                                                                                                                                                                  |
| openssl                                    | [](https://github.com/openssl/openssl)[https://github.com/openssl/openssl](https://github.com/openssl/openssl)                                                                                                                                                                                    |
| OpenVPN                                    | [](https://github.com/OpenVPN/openvpn)[https://github.com/OpenVPN/openvpn](https://github.com/OpenVPN/openvpn)                                                                                                                                                                                    |
| pandas                                     | [](https://github.com/pandas-dev/pandas)[https://github.com/pandas-dev/pandas](https://github.com/pandas-dev/pandas)                                                                                                                                                                              |
| perl                                       | [](https://www.perl.org/)[https://www.perl.org/](https://www.perl.org/)                                                                                                                                                                                                                           |
| PHP                                        | [](https://www.php.net/)[https://www.php.net/](https://www.php.net/)                                                                                                                                                                                                                              |
| php symfony                                | [](https://github.com/symfony/symfony)[https://github.com/symfony/symfony](https://github.com/symfony/symfony)                                                                                                                                                                                    |
| php-src                                    | [](https://github.com/php/php-src)[https://github.com/php/php-src](https://github.com/php/php-src)                                                                                                                                                                                                |
| Pip                                        | [](https://pypi.org/project/pip/)[https://pypi.org/project/pip/](https://pypi.org/project/pip/)                                                                                                                                                                                                   |
| Postgres                                   | [](https://github.com/postgres/postgres)[https://github.com/postgres/postgres](https://github.com/postgres/postgres)                                                                                                                                                                              |
| powershell                                 | [](https://github.com/PowerShell/PowerShell)[https://github.com/PowerShell/PowerShell](https://github.com/PowerShell/PowerShell)                                                                                                                                                                  |
| PrestaShop                                 | [](https://github.com/PrestaShop/PrestaShop)[https://github.com/PrestaShop/PrestaShop](https://github.com/PrestaShop/PrestaShop)                                                                                                                                                                  |
| puppet                                     | [](https://github.com/puppetlabs/puppet)[https://github.com/puppetlabs/puppet](https://github.com/puppetlabs/puppet)                                                                                                                                                                              |
| Python                                     | [](https://www.python.org/)[https://www.python.org/](https://www.python.org/)                                                                                                                                                                                                                     |
| pytorch                                    | [](https://github.com/pytorch/pytorch)[https://github.com/pytorch/pytorch](https://github.com/pytorch/pytorch)                                                                                                                                                                                    |
| qs                                         | [](https://github.com/ljharb/qs)[https://github.com/ljharb/qs](https://github.com/ljharb/qs)                                                                                                                                                                                                      |
| rabbitmq                                   | [](https://www.rabbitmq.com/)[https://www.rabbitmq.com/](https://www.rabbitmq.com/)                                                                                                                                                                                                               |
| rails                                      | [](https://github.com/rails/rails)[https://github.com/rails/rails](https://github.com/rails/rails)                                                                                                                                                                                                |
| rc                                         | [](https://github.com/dominictarr/rc/issues/131)[https://github.com/dominictarr/rc](https://github.com/dominictarr/rc/issues/131)                                                                                                                                                                 |
| react native                               | [](https://github.com/facebook/react-native)[https://github.com/facebook/react-native](https://github.com/facebook/react-native)                                                                                                                                                                  |
| readable-stream                            | [](http://github.com/nodejs/readable-stream)[http://github.com/nodejs/readable-stream](http://github.com/nodejs/readable-stream)                                                                                                                                                                  |
| redis                                      | [](https://redis.io/)[https://redis.io/](https://redis.io/)                                                                                                                                                                                                                                       |
| reprepro                                   | [](https://salsa.debian.org/brlink/reprepro)[https://salsa.debian.org/brlink/reprepro](https://salsa.debian.org/brlink/reprepro)                                                                                                                                                                  |
| Ruby                                       | [](https://github.com/ruby/ruby)[https://github.com/ruby/ruby](https://github.com/ruby/ruby)                                                                                                                                                                                                      |
| RubyGems                                   | [](https://github.com/rubygems/rubygems)[https://github.com/rubygems/rubygems](https://github.com/rubygems/rubygems)                                                                                                                                                                              |
| rust                                       | [](https://github.com/rust-lang/rust)[https://github.com/rust-lang/rust](https://github.com/rust-lang/rust)                                                                                                                                                                                       |
| safe-buffer                                | [https://github.com/feross/safe-buffer](https://github.com/feross/safe-buffer)                                                                                                                                                                                                                    |
| salt (saltstack)                           | [](https://github.com/saltstack/salt)[https://github.com/saltstack/salt](https://github.com/saltstack/salt)                                                                                                                                                                                       |
| signal                                     | [](https://github.com/signalapp)[https://github.com/signalapp](https://github.com/signalapp)                                                                                                                                                                                                      |
| sigstore                                   | [](https://www.sigstore.dev/)[https://www.sigstore.dev/](https://www.sigstore.dev/)                                                                                                                                                                                                               |
| slf4j                                      | [](https://github.com/qos-ch/slf4j)[https://github.com/qos-ch/slf4j](https://github.com/qos-ch/slf4j)                                                                                                                                                                                             |
| solr                                       | [](https://solr.apache.org/)[https://solr.apache.org/](https://solr.apache.org/)                                                                                                                                                                                                                  |
| spark                                      | [](https://github.com/apache/spark)[https://github.com/apache/spark](https://github.com/apache/spark)                                                                                                                                                                                             |
| SQLite                                     | [](https://sqlite.org/index.html)[https://sqlite.org/index.html](https://sqlite.org/index.html)                                                                                                                                                                                                   |
| storybook                                  | [](https://github.com/storybookjs/storybook)[https://github.com/storybookjs/storybook](https://github.com/storybookjs/storybook)                                                                                                                                                                  |
| string_decoder                             | [](http://github.com/nodejs/string_decoder)[http://github.com/nodejs/string_decoder](http://github.com/nodejs/string_decoder)                                                                                                                                                                     |
| systemd                                    | [](https://github.com/systemd/systemd)[https://github.com/systemd/systemd](https://github.com/systemd/systemd)                                                                                                                                                                                    |
| tensorflow                                 | [](https://github.com/tensorflow/tensorflow)[https://github.com/tensorflow/tensorflow](https://github.com/tensorflow/tensorflow)                                                                                                                                                                  |
| three.js                                   | [](https://github.com/mrdoob/three.js)[https://github.com/mrdoob/three.js](https://github.com/mrdoob/three.js)                                                                                                                                                                                    |
| tomcat                                     | [](https://tomcat.apache.org/)[https://tomcat.apache.org/](https://tomcat.apache.org/)                                                                                                                                                                                                            |
| tor                                        | [](https://github.com/torproject/tor)[https://github.com/torproject/tor](https://github.com/torproject/tor)                                                                                                                                                                                       |
| traefik                                    | [](https://traefik.io/)[https://traefik.io/](https://traefik.io/)                                                                                                                                                                                                                                 |
| typescript                                 | [](https://github.com/microsoft/TypeScript)[https://github.com/microsoft/TypeScript](https://github.com/microsoft/TypeScript)                                                                                                                                                                     |
| u-boot                                     | [](https://u-boot.readthedocs.io/en/latest/)[https://u-boot.readthedocs.io/en/latest/](https://u-boot.readthedocs.io/en/latest/)                                                                                                                                                                  |
| UA-Parser-JS                               | [](https://github.com/faisalman/ua-parser-js)[https://github.com/faisalman/ua-parser-js](https://github.com/faisalman/ua-parser-js)                                                                                                                                                               |
| vault                                      | [](https://www.vaultproject.io/)[https://www.vaultproject.io/](https://www.vaultproject.io/)                                                                                                                                                                                                      |
| vscode                                     | [](https://github.com/microsoft/vscode)[https://github.com/microsoft/vscode](https://github.com/microsoft/vscode)                                                                                                                                                                                 |
| webpack                                    | [](https://github.com/webpack/webpack)[https://github.com/webpack/webpack](https://github.com/webpack/webpack)                                                                                                                                                                                    |
| WordPress                                  | [](https://github.com/WordPress/WordPress)[https://github.com/WordPress/WordPress](https://github.com/WordPress/WordPress)                                                                                                                                                                        |
| yocto project                              | [](https://www.yoctoproject.org/)[https://www.yoctoproject.org/](https://www.yoctoproject.org/)                                                                                                                                                                                                   |
| Zephyr                                     | [](https://github.com/zephyrproject-rtos/zephyr)[https://github.com/zephyrproject-rtos/zephyr](https://github.com/zephyrproject-rtos/zephyr)                                                                                                                                                      |
| zlib                                       | [](https://zlib.net/)[https://zlib.net/](https://zlib.net/)                                                                                                                                                                                                                                       |
| zookeeper                                  | [](https://zookeeper.apache.org/)[https://zookeeper.apache.org/](https://zookeeper.apache.org/)                                                                                                                                                                                                   |
| zstd                                       | [](https://facebook.github.io/zstd/)[https://facebook.github.io/zstd/](https://facebook.github.io/zstd/)                                                                                                                                                                                          |
