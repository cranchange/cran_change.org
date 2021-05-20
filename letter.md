We, the undersigned R users, R package developers, and R community members stand unified in our concern for the future of the R package ecosystem.

A pattern of increasingly inconsistent and heavy-handed behaviour by CRAN administrators has diminished our trust that our community's central package archive is being managed sustainably.

If left unchecked we believe this pattern will undermine CRAN's position as a comprehensive archive of quality software, since is it already leading many of us to question whether submitting to CRAN is worthwhile, and wonder if tests deployed on CRAN are truly assets or liabilities.

In particular we believe three practices are harmful:

**Rejecting submissions based on undocumented criteria, or inconsistently applied criteria** makes it difficult for contributors to predict if their submissions will be accepted without issues, and so erodes willingness to contribute. For example:

  * There seems to have been an undocumented change in stance toward examples, with many contributors reporting CRAN administrators are rejecting submissions citing not enough examples whilst also refusing to accept any examples with `\dontrun{}` and `\donttest{}`. These blocks have been used liberally in historical submissions. 
  * On multiple occasions packages premised around colour palettes have been rejected due to triviality only to have other packages with almost identical premises, and of similar complexity be accepted shortly after. 
  
These types of experiences are felt heavily by new contributors who are not aware of hidden criteria they need to meet or the "luck" element of getting a package accepted smoothly.

**Archiving packages for a small number of test failures on proprietary platforms** harms package test coverage. For example:

  * Recently a package with 100% test coverage and over 2000 tests was archived when 2 of those tests began failing on an expensive proprietary platform. The failure could not be reproduced on RHub.
  
This practice discourages extensive testing on CRAN, and has already lead developers among us to limit functionality exposed to CRAN to low-risk subsets. The degradation of the reverse dependency checking system in this way weakens both packages and the R language itself, since package checks are used to validate core changes.

**Archiving packages with little or no warning** discriminates against contributors with less time available on short notice. Under the current practice there are many categories of contributor who may find it difficult to keep their contributions on CRAN, for example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell or on leave

Aside from the nature of these actions, the tone taken by CRAN administrators in their communications with contributors is at times abrupt and unsympathetic. This routinely takes new contributors by surprise since it is out of step with the norms of the larger R community. 

Contributors are a precious resource and discouraging them threatens CRAN's 'comprehensive** aspect.

The fact that there is currently no avenue by which we, R community members, can engage CRAN administrators on these topics points to an operating model that our community may have outgrown. There are aspects of the way CRAN works that we feel are unnecessarily opaque, and incompatible with the open nature of the R community and its other governing bodies.

We therefore propose the following reforms to CRAN to ensure a robust, comprehensive, and diverse R package ecosystem:

1. Consult with the community to create a policy on archival. For example: Minimum 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access
2. Standardise build environments and publish reproducible configuration so that contributors can test against CRAN environments, e.g. via RHub
3. Consult with the community to create a policy on editorialisation that can be consistently applied. Do we want CRAN rejecting packages based on qualitative assessments of content? Detailed criteria must be published if so. For example: https://devguide.ropensci.org/policies.html#policies
4. If CRAN modifies a package's source code for any reason this must be made clear with an onLoad message, and version number bump
5. Publish a policy on resubmission intervals that can be consistently applied 
6. Cease punitive temporary submission bans for contributors with repeated rejections or test failures
7. Establish a governance model including a process by which community members can propose changes to CRAN policies or processes. For example the PEP system in Python
8. Establish a code of conduct for the behaviour of CRAN administrators and contributors in their dealings
9. Publish minutes of CRAN governence meetings
10. Publish a succession plan for the CRAN administrators nearing retirement
11. Establish a process whereby CRAN notifies the R community of shortfalls in resources which could be met by community contributions 

We appreciate a lot of reform is being sought from what is a famously small team of administrators. However, being under-resourced does not mitigate the shortcomings of CRAN's current practices, rather it is an argument in itself that reform is needed so that CRAN may attract the resources to perform its valuable role sustainably.

Finally, we wish to acknowledge the dedication of the CRAN administrators and thank them for the foundational piece of community architecture that has made the way we work together with R possible. If the reform process creates opportunities for the community to share our skills and resources with CRAN in return, there are many signed here who would pleased to do so.

## Supporting this petition

With this action we wish to advocate for a respectful dialogue about reforming the administration of CRAN's package ecosystem. We do not wish to disparage the contributions that have been provided to this point by CRAN administrators. There are several steps R commnity members can take to show their support for these reforms:

1. share this petition with your networks
2. withhold submitting new packages or new features to CRAN where you are comfortable doing so, and use this badge in your README <BADGE URL>
3. configure alternative package repositories where you trust the developers e.g. https://r-universe.dev for rOpensci, RStudio et. al. packages
4. refer to the CRAN team as "CRAN administrators" rather than their self-assigned label of "volunteers". The former label befits their role, the latter resists accountability.
