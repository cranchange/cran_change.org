The Comprehensive R Archive Network (CRAN), is unusual among similar user-contributed software package infrastructure due to the high standards to which contributed packages are held, and the continuous checking system that validates packages against reverse dependencies and operating systems. 

These features combine to create an extremely smooth user experience where users can trust that any software they install from CRAN is likely to work, be compatible with other CRAN packages, and most importantly leave their local R package library in a consistent state.

There is no question that moving software package pain points out of the way of statistics practitioners has made a large contribution to R becoming an extremely popular statistical programming environment.

Unfortunately, we, the undersigned R community members, are unified in our concern that CRAN is showing signs that it is struggling to scale with popularity of the R language. 

In particular there appears to be pattern of increasingly unreliable criteria coupled with authoritarian practices that is adding to the burden on both package contributors and CRAN administrators.

This pattern is driving behavioural change in contributors among us. Many are acting to reduce their exposure to CRAN's policies and checks. This not only undermines CRAN's checking system but also the R language itself since CRAN checks are used to validate core changes.

There are also contributors for whom the increasing burden has reached a tipping point, leading them to feel frustrated and discouraged. There is evidence that this frustration is mirrored by some CRAN administrators with numerous accounts of communications that are apparently coloured by it. 

The fact that there is currently no avenue by which R community members can engage CRAN administrators on these topics is another indication that our community may have outgrown CRAN's operating model. There are aspects of the way CRAN works that seem unnecessarily opaque, and likely leading to the contributions of CRAN's administrators being under-appreciated and thus under-resourced.

We therefore petition CRAN's administrators to make the following reforms to ensure CRAN continues to serve the R community as a robust, comprehensive, and diverse R package ecosystem:

1. **Consult with the community to create a policy on archival.**

For example: Minimum 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access.

Consider that short timelines make it challenging for certain classes of contributor to keep their work on CRAN. For example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell or on leave
  
Also consider that archiving packages quickly may increase future review overhead if CRAN administrators apply a higher standard of review to packages returning from archived status. 

2. **Standardise build environments and publish reproducible configuration.**

Expecting contributors to ensure no test failures in environments they cannot access guarantees CRAN administrators will be burdened by chasing contributors for fixes for those environments. Contributors are burdened by challenges in diagnosing issues in those environments.

Having reproductions of CRAN's environments available on infrastructure like RHub or GitHub actions could greatly reduce instances of platform specific issues making their way onto CRAN.

3. **Publish a single exhaustive and authoritative source of criteria that a package must meet to be accepted on CRAN.**

Fully documenting criteria, like for example the current stance on `\donttest`/`\donttrun`, or providing detailed guidance as to the interpretation of terms like "publication quality" and "trivial" has the potential to significantly reduce the submission burden for administrators and contributors. An increased ability for contributors to predict if their package is CRAN-ready may also bolster will to contribute.


4. **Consult with the community to create or modify CRAN policy**.

Publicly flagging policy changes some time before they come into effect can reduce policy ignorance and the associated burden of policy police work on CRAN administrators. It would also give contributors a chance to bring their work into line with policy without requiring threat of archive, reducing pressure and frustration. 

Publicly consulting on policy with the community has the added benefit of potentially identifying policies that stifle innovation in unexpected ways, or will motivate unanticipated work-arounds. These insights can reduce policy churn in the long term, along with associated administrator police work and contributor frustration.

5. **If CRAN modifies a package's source code for any reason this must be made clear to maintainers and users** 

Maintainers should receive an email, the package version number should be bumped, and users should receive an onLoad message 

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
