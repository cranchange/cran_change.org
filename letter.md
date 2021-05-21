There is no question that holding an ever increasing pool of software and contributors to high standards, and continuously validating those standards are held is a resource intensive and technical feat from which great public good has been derived. 

To continue providing this great service this letter seeks to draw attention to deficiencies in empathy and fairness that are impacting the R community. 

Yet in the spirit of empathy for the experiences of CRAN's users, and in fairness to the future R community that we, the undersigned R community members, find ourselves with no other reasonable alternative than to unify our voices in a call to reform CRAN practices that are damaging the R package ecosystem.

We want to acknowledge the sustained dedication of our CRAN administrators, and thank them for the foundational piece of infrastructure they have built which has made the way we work together with R possible. However, a pattern of increasingly inconsistent and heavy-handed behaviour by CRAN administrators has shaken our trust that our community's central package archive is being managed sustainably.

If left unchecked we believe this pattern will undermine CRAN's position as a comprehensive archive of quality software, since is it already leading many of us to question whether submitting to CRAN is worthwhile, and wonder if tests deployed on CRAN are truly assets or liabilities.

In particular we believe three practices are harmful:

**Rejecting submissions based on undocumented criteria, or inconsistently applied criteria** makes it difficult for contributors to predict if their submissions will be accepted without issues, and so erodes willingness to contribute. For example:

  * There seems to have been an undocumented change in stance toward examples, with many contributors reporting CRAN administrators are rejecting submissions citing not enough examples whilst also refusing to accept any examples with `\dontrun{}` and `\donttest{}`. These blocks were previously accepted as standard practice. 
  * On multiple occasions packages premised on colour palettes have been rejected due to triviality only to have other packages with almost identical premises, and of similar complexity be accepted shortly after. 
  
These types of experiences are felt heavily by new contributors who are not aware of hidden criteria they need to meet or the "luck" element of getting a package accepted smoothly.

**Archiving packages for a small number of test failures on proprietary platforms** harms package test coverage. For example:

  * Recently a package with 100% test coverage and over 2000 tests was archived when 2 of those tests began failing on an expensive proprietary platform. The failure could not be reproduced on RHub.
  
This practice discourages extensive testing on CRAN, and has already lead developers among us to limit functionality exposed to CRAN to low-risk subsets. The degradation of the reverse dependency checking system in this way weakens both packages and the R language itself, since package checks are used to validate core changes.

**Archiving packages with little or no warning** discriminates against contributors with less time available on short notice. Typical periods attached to the threat of archival seem to range in zero to six weeks. Under this practice there are many categories of contributor who will find it difficult to keep their contributions on CRAN, for example:

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
3. Configure alternative package archives where you trust the developers e.g. https://r-universe.dev for rOpensci, RStudio et. al. packages
4. Contribute your own packages to alternative repositories e.g. https://r-universe.dev and advertise these ways to install them in your README
4. refer to the CRAN team as "CRAN administrators" rather than their self-assigned label of "volunteers". This label describes a role which we can clarify the expectations of as opposed to a remuneration status.
