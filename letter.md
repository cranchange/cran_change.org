We, the undersigned R users, R package developers, and R community members stand unified in our concern for the future of the R package ecosystem and the R community given increasingly unpredictable behaviour by CRAN adminstrators.

In particular we believe two practices are harmful:

Archiving packages for a small number of test failures on proprietary platforms harms both contributor diversity and package test coverage. For example:

  * Apple hardware is expensive to obtain, which makes acessing macOS test environments challenging for some contributors.
  * Recently a package with 100% test coverage and over 2000 tests was archived (at short notice) when 2 of those tests began failing on one specific platform. This practice discourages developers from extensively testing their packages on CRAN which in may degrade the package ecosystem.

Archiving packages with little to no notice discriminates against contributors with less time available on short notice. This harms contributor diversity. Under the current practice there are many categories of contributor who may find it difficult to keep their contributions on CRAN, for example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell
  * Contributors on leave

The fact that there is currently no avenue by which we, R community members, can engage CRAN administrators on this topic points to an operating model that our community may have outgrown. There are aspects of the way CRAN works that we feel are unnecessarily opaque, and incompatible with the open nature of the R community and its other governing bodies.

We therefore propose the following reforms to CRAN to ensure the longevity and stability of the R package ecosystem:

1. Consult with the community to create a policy on archival. For example: Minimum 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access
2. Standardise build environments and publish configuration so that developers can test against CRAN environments, e.g. via RHub
3. Consult with the community to create a policy on editorialisation that can be consistently applied. Do we want CRAN rejecting packages based on qualitative assessments of content? Detailed criteria must be published if so. For example: https://devguide.ropensci.org/policies.html#policies
4. If CRAN modifies a package's source code for any reason this must be made clear with an onLoad message, and version number bump
5. Publish a policy on resubmission intervals that can be consistently applied, and cease punitive temporary submission bans for contributors with repeated rejections
6. Establish a governance model including a process by which community members can propose changes to CRAN policies or processes. For example the PEP system in Python
7. Establish a code of conduct for the behaviour of CRAN administrators and contributors in their dealings
8. Publish minutes of CRAN governence meetings
9. Publish a succession plan for the CRAN administrators nearing retirement
10. Publish an account of resources CRAN receives, detailing how they are spent

The first reaction to our proposal is likely to be: "We're just volunteers, we don't have the resources to do this". A counter argument to that is that being under-resourced does not excuse problems with CRAN administrative practices, rather it provides further evidence that reform is required. 

## Supporting this petition

With this action we wish to advocate for a respectful dialogue about reforming the adminstration of CRAN's package ecosystem. We do not wish to diminish the contributions that have been provided to this point by CRAN administrators. There are several steps R commnity members can take to show their support for these reforms:

1. share this petition with your networks
2. withhold submitting new packages or new features to CRAN where you are comfortable doing so, and use this badge in your README <BADGE URL>
3. configure alternative package repositories where you trust the developers e.g. https://r-universe.dev/organizations/ for rOpensci, RStudio et.al packages
4. refer to the CRAN team as "CRAN administrators" rather than their self-assigned label of "volunteers". The former label befits their role, the latter resists accountability.
