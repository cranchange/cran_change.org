The Comprehensive R Archive Network (CRAN), is unusual among similar user-contributed software package infrastructure due to the high standards to which contributed packages are held, and the continuous checking system that validates packages against reverse dependencies and operating systems. 

These features combine to create a smooth user-friendly experience where users can trust that any software they install from CRAN is likely to work, be compatible with other CRAN packages, and most importantly leave their local R package library in a consistent state.

There is no question that moving software package pain points out of the way of statistics practitioners has made a large contribution to R becoming an extremely popular statistical programming environment.

Unfortunately, we, the undersigned R community members, are unified in our concern that CRAN is showing signs that it is struggling to scale with the popularity of the R language. 

In particular there appears to be pattern of increasing and shifting the burden of maintaining packages on CRAN via regular introduction of new criteria and policies coupled with an uptick in heavy-handed enforcement practices. Some of these new constraints are not well documented, leading to much confusion that is adding to the burden on both contributors and CRAN administrators.

This pattern is driving behavioural change in contributors among us. Many are acting to reduce their exposure to CRAN's policies and checks. This not only undermines CRAN's checking system but also the R language itself since CRAN checks are used to validate core changes.

There are also contributors for whom the increasing burden has reached a tipping point, leading them to feel frustrated and discouraged. There is evidence that this frustration is mirrored by some CRAN administrators with numerous accounts of communications that are apparently coloured by it. 

To reverse these trends we believe it is time for CRAN to undertake reform. At a high level we are calling for measures that will:

* Increase the clarity of criteria for packages to be accepted and remain on CRAN
* Improve the consistency and predictability of working with CRAN
* Ensure CRAN is accessible to a diverse set of contributors
* Establish channels for CRAN collaboration with the R community 

One of the main themes of our proposal is improving information flow between the community and CRAN. The fact that there is currently no avenue by which R community members can engage CRAN administrators on these topics is evidence of room for improvement in this regard. And while it is unclear whether communication is low due to lack of resources, improving transparency and information flow does seem a necessary precondition for attracting additional resources for CRAN's important work.

As we will argue, many of our proposals have the capacity to reduce the burden on CRAN administrators as well as contributors, making contributing software to the R ecosystem more efficient and pleasant for all.

We therefore petition CRAN's administrators to make the following reforms to ensure CRAN continues to serve the R community as a robust, comprehensive, and diverse R package ecosystem:

1. **Consult with the community to create a policy on archival.**

For example: Minimum 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access.

Consider that short timelines make it challenging for certain classes of contributor to keep their work on CRAN. For example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell or on leave
  
Also consider that archiving packages quickly may increase future review overhead if CRAN administrators apply a higher standard of review to packages returning from archived status. 

2. **Standardise build environments and publish reproducible configuration.**

Expecting contributors to ensure no test failures in environments they cannot access guarantees CRAN administrators will be burdened by chasing contributors for fixes for those environments. When that happens, contributors are burdened by challenges in diagnosing issues in those environments.

Having reproductions of CRAN's environments available on infrastructure like RHub or GitHub actions could greatly reduce instances of platform specific issues making their way onto CRAN.

3. **Publish a single exhaustive and authoritative source of criteria that a package must meet to be accepted on CRAN.**

Fully documenting criteria, like for example the current stance on `\donttest`/`\donttrun`, or providing detailed guidance as to the interpretation of terms like "publication quality" and "trivial" has the potential to significantly reduce the submission burden for administrators and contributors. An increased ability for contributors to predict if their package is CRAN-ready may also bolster will to contribute.


4. **Consult with the community to create or modify CRAN policy**.

Publicly flagging policy changes some time before they come into effect can reduce policy ignorance and the associated burden of policy enforcement on CRAN administrators. It would also give contributors a chance to bring their work into line with policy without requiring threat of archive, reducing pressure and frustration. 

Publicly consulting on policy with the community has the added benefit of potentially identifying policies that stifle innovation in unexpected ways, or will motivate unanticipated work-arounds. These insights can reduce policy churn in the long term, along with associated administrator enforcement burden and contributor frustration.

5. **If CRAN modifies a package's source code for any reason this must be made clear to maintainers and users** 

When parties are unaware of CRAN modifications unfortunate wasteful events have been observed to occur:

* Authors unknowingly undo CRAN's changes in a subsequent submission causing problems that cost contributors and administrators time. 
* Users submit bug reports relating to CRAN changes leading to difficulty in reproducing issues.

It has been observed that some of these modifications may relate to intricacies of CRAN's environments, a further argument for reform4.

At a minimum we propose that maintainers should receive an email, the package version number should be bumped, and users should receive an onLoad message. 

6. Publish a policy on re-submission intervals that can be consistently applied 

A recurring source of conflict between administrators and contributors arises when contributors submit too frequently. This may be due to the fact that the allowable frequency of submissions is left rubbery in CRAN policy. Ideally contributors would receive a set number of submissions per period. CRAN systems would automatically ensure they don't submit more than this, and it would be clear to contributors at all times how many submissions they have, or how long until they can next submit.

7. Cease punitive temporary submission bans for contributors with repeated rejections or test failures

Administrators issuing punishments is a cumbersome process that involves effort in decision making, communication, and bookkeeping. Time can be saved by replacing it with more transparent, and automatic processes wherever possible. For example:

* Test failures could trigger automatic notifications, and automatically result in archival if they reach a persistence or recurrence threshold. Package status with respect to these thresholds could be publicly visible to users and contributors encouraging them to resolve these issues without administrator intervention.
* Rejections could be treated similarly to submissions, with a set quota of rejections available before a break period is automatically introduced. Contributors would be able to know at all times how much of their quota remains, and the break period that would result from exceeding it. 

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
