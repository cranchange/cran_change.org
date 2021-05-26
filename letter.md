The Comprehensive R Archive Network, CRAN from now forward, is one of the central pieces of the R ecosystem (besides R itself). As such, the role it has played on the R development and adoption of R is huge. CRAN has benefited both R developers and the R community by providing a place to evaluate the impact of R changes, explore solutions to the language itself, provide support to package with functionality beyond the R language and most importantly ensure a common quality threshold for packages, among other benefits.

CRAN also requires many resources from the community: The machines and software infrastructure, reviewing packages, the CRAN mirrors, the security of the site... 
All this takes much time from all the R core members, the R foundation and R package contributors. All have dedicated many hours if not days or years to make it such a successful resource. 
There is no question that holding an ever increasing pool of software and contributors to high standards, and continuously validating those standards are held is a resource intensive technical feat from which great public good has been derived.

We specially want to recognize and praise the dedication of the R core members to this task. As R package developers and/or R users we usually just see a slice of the work required instead of the herculean effort done as attest that R is one of the few languages that has such resource. Thanks!

CRAN has made possible a vibrant and growing community of R users who many of them want to make available their work and solutions to other R members. As such  contributing to the archive has become even more important to all. 

However, with an increased support to several architectures, settings and a growing number of packages, the pressure on CRAN maintainers and admins has increased too. 

Current efforts to decrease the pressure has been addressed to ensure that the packages submitted pass some automatic quality checks: The R foundation has provided support to lighten the pressure on CRAN package maintainers such as the R hub, which has dramatically helped R package maintainers. CRAN administrators has also provided checking venues to test packages before the submissions for some settings. But both efforts are not complete a still the R hub does not have the same configuration and environments as CRAN. 

As the number of R package contributors outnumbers the R core members dedicated to CRAN we agree on the general direction of the efforts: a small improvement done by each maintainer helps all. We are keen to invest more time on improving the quality of the packages and reduce the work passed to the R cored.

In particular we believe three practices are harmful:

**Rejecting submissions based on undocumented criteria, or inconsistently applied criteria** makes it difficult for contributors to predict if their submissions will be accepted without issues, and so erodes willingness to contribute. For example:

  * There seems to have been an undocumented change in stance toward examples, with many contributors reporting CRAN administrators are rejecting submissions citing not enough examples whilst also refusing to accept any examples with `\dontrun{}` and `\donttest{}`. These blocks were previously accepted as standard practice. 
  * On multiple occasions packages premised on colour palettes have been rejected due to triviality only to have other packages with almost identical premises, and of similar complexity be accepted shortly after. 
  
This practice wastes the time of both CRAN administrators and contributors. We believe the submission burden on both sides could be significantly reduced by fully documenting acceptance criteria, and reducing ambiguity with guidance and examples. 

**Archiving packages for a small number of test failures on proprietary platforms** harms package test coverage. For example:

  * Recently a package with 100% test coverage and over 2000 tests was archived when 2 of those tests began failing on an expensive proprietary platform. The failure could not be reproduced on RHub.
  
This practice discourages extensive testing on CRAN, and has already lead developers among us to limit functionality exposed to CRAN to low-risk subsets. The degradation of the reverse dependency checking system in this way weakens both packages and the R language itself, since package checks are used to validate core changes.

**Archiving packages with little or no warning** discriminates against contributors with less time available on short notice. Typical periods attached to the threat of archival seem to range in zero to six weeks. Under this practice there are many categories of contributor who will find it difficult to keep their work on CRAN, for example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell or on leave

Aside from the nature of these actions, the tone taken by CRAN administrators in their communications with contributors is at times abrupt and unsympathetic. This routinely takes new contributors by surprise since it is out of step with the norms of the larger R community. 

Contributors are a precious resource and discouraging them threatens CRAN's 'comprehensive' aspect.

The fact that there is currently no avenue by which R community members can engage CRAN administrators on these topics points to an operating model that our community may have outgrown. There are aspects of the way CRAN works that we feel are unnecessarily opaque, and incompatible with the open nature of the R community and its other governing bodies.

We therefore propose the following reforms to CRAN to ensure a robust, comprehensive, and diverse R package ecosystem:

1. Consult with the community to create a policy on archival. For example: Minimum 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access
2. Standardise build environments and publish reproducible configuration so that contributors can test against CRAN environments, e.g. via RHub
3. Publish a single exhaustive and authoritative source of criteria that a package must meet to be accepted on CRAN
4. Consult with the community to create a CRAN editorial policy that can be consistently applied. Do we want CRAN rejecting packages based on qualitative assessments of content? Detailed criteria must be published if so. For example: https://devguide.ropensci.org/policies.html#policies
5. If CRAN modifies a package's source code for any reason this must be made clear to maintainers and users. Maintainers should receive an email, the package version number should be bumped, and users should receive an onLoad message 
6. Publish a policy on re-submission intervals that can be consistently applied 
7. Cease punitive temporary submission bans for contributors with repeated rejections or test failures
8. Establish a governance model including a process by which community members can propose changes to CRAN policies or processes. For example the PEP system in Python
9. Establish a code of conduct for the behaviour of CRAN administrators and contributors in their dealings
10. Publish minutes of CRAN governence meetings
11. Establish a process whereby CRAN notifies the R community of shortfalls in resources which could be met by community contributions 

We appreciate a lot of reform is being sought from what is a famously small team of administrators. However, being under-resourced does not mitigate the damage being done by CRAN's current practices, rather it is an argument in itself that reform is needed so that CRAN may attract the resources to perform its valuable role sustainably.

## Supporting this petition

With this action we wish to advocate for a respectful dialogue about reforming the administration of CRAN's package ecosystem. We do not wish to disparage the contributions that have been provided to this point by CRAN administrators.

In addition to signing the petition there are several steps R community members can take to show their support for these reforms:

1. Share this petition with your networks
2. Withhold submitting new packages or new features to CRAN where you are comfortable doing so, and use this badge in your README [BADGE URL] 
3. Configure alternative package repositories where you trust the developers e.g. https://r-universe.dev for rOpensci, RStudio et. al. packages
4. Contribute your own packages to alternative repositories and advertise these ways to install them in your README
4. refer to the CRAN team as "CRAN administrators" rather than their self-assigned label of "volunteers". This label describes a role which we can clarify the expectations of as opposed to a remuneration status.
