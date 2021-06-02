# Introduction

The Comprehensive R Archive Network, CRAN from now forward, is one of the central pieces of the R ecosystem (besides R itself). 
CRAN has made possible a vibrant and growing community of R users who many of them want to make available their work and solutions to other R members. It has unified the R users and the role it has played on the R development and adoption of R. 
CRAN has benefited both R core developers and the R community. 

CRAN also requires many resources from the community: The machines and software infrastructure, reviewing and updating packages, the CRAN mirrors, the security of the site... 
All this takes much time from all the R core members and R package contributors who have dedicated many hours if not days or years to make it such a successful resource. 
There is no question that holding an ever increasing pool of software and contributors to high standards, and continuously validating those standards are held is a resource intensive technical feat from which great public good has been derived.

Past efforts to decrease the pressure has been addressed to ensure that the packages pass some automatic quality checks before the submission:
The R foundation has provided support to lighten the pressure on CRAN package maintainers such as the R hub, which has dramatically helped R package maintainers and CRAN has provided alternative checking venues for some settings. 

We want to add our suggestion of changes to the R Core and R Foundation to continue improving CRAN. 
They have been motivated by an increasing divergent view of what is CRAN and what it will be on the future, which has lead to different opinions about what is accepted on CRAN, how to check, keep or increase the quality of CRAN packages and the transparency of how CRAN operates. 
We think that these petitions will help reducing CRAN's team time spend on packages and package maintainers to submit better packages more prone to be accepted on the archive.
Most of the measures are focused on providing a healthier bidirectional communication between CRAN and R packages maintainers at large.
We think better communication, which is key to the success of the project, would and create smoother submissions and experiences maintaining a package on CRAN.
We understand that this measures will cause an initial work but we argue that they will pay off soon.

# Petitions

We propose the following measures to improve how CRAN works and its role on the R ecosystem:

1. **Consult with the community to create a policy on archival**. 

This would help to set expectations beforehand and the package maintainers to organize their time to work on the package to address any required change. Longer time on difficult platforms, those without alternative checking venues, also ensures that the package maintainers have time to explore these platforms, identify and fix any potential error. For example: Minimum 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access.
More time would prevent archival of packages with extensive testing but lack of resources to test on platforms and settings difficult to access, this would also enable that packages maintainer to confidently not expose more test to CRAN checks without fear of a sudden archival. This will also help contributors who have no paid time to work on open source, with other familiar responsabilities, or with health issues at the moment the bugs are detected on CRAN. 

2. **Standardise build environments** and publish reproducible configuration so that contributors can test against CRAN environments.

The environments and system configuration are hard to set up to reproduce the environments. Currently the R Foundation supports R-Hub but these servers do not have the same environments as on CRAN. 
Some CRAN values for R environmental variables are documented on the R internals manual page https://cran.r-project.org/doc/manuals/r-release/R-ints.html#Tools, which is not linked on CRAN policy. Others environment variables used by CRAN are not documented on R internals neither, such as "_R_CHECK_CRAN_INCOMING_CHECK_FILE_URIS_". This is a source of confusion when package developers checks do not return the same results as CRAN, and the package developers do not know how to properly test their packages.
Sharing more of the environment would increase the fidelity that package maintainers could test their package as CRAN team does before submitting to CRAN, thus reducing the resubmissions on CRAN and time spend checking packages on CRAN machines as well as CRAN reviewers time.  


3. Publish a single exhaustive and **authoritative source of criteria that a package must meet to be accepted on CRAN**.

Currently some package authors do not have a clear idea whether their package will be accepted on CRAN, not on base of the automatic checks but about the content and goal of their packages. The policy currently says of "publication quality ", but that might be not well understood for those outside academia and leaves out many useful packages to the community that are not scientific or academic. 

This sets the CRAN reviewers in a position to judge on a nebulous criteria and differences between what reviewers deem of publication quality and hence on what is suitable for CRAN. Which has lead to rejecting submissions based on undocumented criteria, or inconsistently applied criteria. For instance packages for colour palettes have been rejected as insufficient while others where accepted or requiring sufficient documentation but refusing to accept any examples with `\dontrun{}` and `\donttest{}`. If CRAN rejecting packages based on qualitative assessments of content detailed criteria should be published. For example: https://devguide.ropensci.org/policies.html#policies

4. **Consult with the community to create or modify CRAN policy**. 

To our knowledge CRAN policy changes have been made without announcing or consulting the package maintainers affected. The community has set up ways to track changes on it. Discussing and announcing those changes, for example on the R-pkg-devel mailing list before they are being acted upon will reduce CRAN reviewers work as package maintainers will be able to be proactive and apply the CRAN policies while developing their packages or before they receive a message from CRAN, reducing the work from CRAN team.

5. Establish a **governance model** including a **process** by which community members can propose changes to CRAN policies or processes. 

This governance would ensure that future changes keep all involved aligned. For example the PEP system in Python, or the boards of Bioconductor are some examples of governance bodies on similar communities. 

6. If **CRAN modifies or archives a package** for any reason this must be **notified** to maintainers.

Currently CRAN reserves the right to remove and modify any package. We understand that CRAN only exercises this power on very rare occasions but on those cases there has been some inconsistency which affected downstream packages, consistently applying this petition would help those packages affected and their dependencies to be aware of any change and update their packages accordingly.
On package modifications, the package version number should be bumped. If the changes modify package output, users should be also notified either via an onLoad message, NEWS or other methods.

7. **Clarify a policy on updates to previously-published packages** intervals that can be consistently applied.

There is some confusion about when can a package be resubmitted on CRAN and on what basis. A clarification to this regard on the policy will be greatly appreciated.

8. Cease **punitive temporary submission bans** for contributors with repeated rejections or test failures.

There has been some cases when some authors received an email banning them from submitting a package for some time. We understand that this might be necessary if this is a SPAM or DOS attack but in all the other cases if packages pass the automatic checks the submission should be considered. If CRAN reviewers consider that there is a considerable number of cases where package authors do not follow their advice and impose more work on them, setting a clear CRAN policy of ban duration will be appreciated.

9. **Establish a code of conduct** for the behaviour on the exchange on between CRAN and package contributors.

Currently the R project has a code of conduct for the useR! conferences. Extending a similar code of conduct to CRAN will help people from different backgrounds and cultures know how to address to CRAN and how CRAN will address them. A process to know what to expect when anyone involved does not follow the professional etiquette would be we also pertinent. 

10. Publish minutes of **CRAN governance meetings**.

This will provide a venue to those interested on helping CRAN to be aware of any discussion where their expertise could help CRAN and avoid duplication of efforts between CRAN and other communities. For example, the Bioconductor governance boards publish their minutes after they are approved on the next meeting which has lead to an increased participation from some members. 

11. Establish a process whereby **CRAN notifies the R community** of shortfalls in resources which could be met by community contributions.

As seen the pressure on CRAN resources is increasing and we do not want to see a break down of CRAN, so if there were a method or channel that CRAN could requests resources some members of the community might step up. Using the recently created blog at https://developer.r-project.org/Blog/public/ might be a good site to post such needs as well as the R-devel-pkg mailing list.
