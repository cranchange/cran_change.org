The Comprehensive R Archive Network (CRAN) is exceptional infrastructure. Thanks to high standards for contributions and a thorough continuous checking system, users can trust that any package from CRAN is likely to work, be compatible with other CRAN packages, and leave the local R package library in a consistent state. These guarantees are fundamental to the success and popularity of R, and they would not be possible without the tireless effort and diligence of the CRAN team.

Because of its success, CRAN has become a fundamental global resource, not only for independent researchers, but also for large organizations across academia, government, and industry, all of whom all depend on the ability to contribute packages in a reliable and predictable manner. The scope and the need have grown bigger than one individual or small team, and it is appropriate that the R community exercise a voice with respect to the conduct and administration of CRAN.

We, the undersigned R community members, are unified in concern that CRAN is struggling to provide a consistent experience for contributors.

New criteria and policies are sometimes introduced without enough notice or documentation for contributors to follow, and enforcement practices can be discourteous and severe. Contributors are experiencing ambiguity, disruption, and frustration, and they are changing their behaviour to reduce exposure to CRAN's policies and checks (e.g. skipping all tests on CRAN). This not only undermines CRAN's checking system but also the R language itself since CRAN checks are used to validate core changes.

To reverse these trends, we are petitioning CRAN for reform. We request measures that:

* Establish channels for CRAN collaboration with the R community.
* Clarify criteria for packages to be accepted on CRAN.
* Ensure a predictable experience for contributors.
* Ensure CRAN is accessible to a diverse set of contributors.

Communication between the community and CRAN precedes our other proposed reforms, and improving transparency and information flow is likely to be a precondition for attracting additional resources for CRAN's important work. Package contributors currently have difficulty engaging CRAN on the topics described here, and we request an avenue for ongoing dialogue with the community.

Many of our proposals have the capacity to reduce the burden on CRAN administrators as well as contributors, making contributing to the R ecosystem more efficient and pleasant for all.

We therefore petition CRAN's administrators to make the following reforms to ensure CRAN continues to serve the R community as a robust, comprehensive, and diverse R package ecosystem:

## 1. Consult with the community to create a policy on archival.

Charitable timelines for contributors to fix issues promote diversity within the contributor community. Short timelines, like 2 weeks, make it challenging for some to keep their work on CRAN, for example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell or on leave

Presenting achievable deadlines is likely to encourage contributors to implement fixes before they expire, since many anecdotes point to a higher standard of review being applied to packages attempting to return from the archive. It would also make sense to formalise this notion of a higher review standard in policy to help contributors understand the ramifications of missing a deadline.

Timelines could also vary by issue type, for example: 6 weeks for policy change, 6 weeks for failing tests. 12 weeks for tests failing on platforms that are difficult to access.

With this policy in place CRAN administrators benefit from having to archive less often, and spend less time reviewing archived package re-submissions. Simultaneously, the whole community benefits from a diverse pool of contributors that helps ensure CRAN continues to offer tools that meet ever-evolving needs.

## 2. Standardise build environments and publish reproducible configuration.

Expecting contributors to ensure no test failures in environments they cannot access guarantees CRAN administrators will be burdened by chasing contributors for fixes for those environments. When that happens, contributors are burdened by challenges in diagnosing issues in those environments.

Having reproductions of CRAN's environments available on infrastructure like RHub or GitHub actions could greatly reduce instances of platform specific issues making their way onto CRAN.

## 3. Publish a single exhaustive and authoritative source of criteria that a package must meet to be accepted on CRAN.

Fully documenting criteria, like for example the current stance on `\donttest`/`\donttrun`, or providing detailed guidance as to the interpretation of terms like "publication quality" and "trivial" has the potential to significantly reduce the submission burden for administrators and contributors. An increased ability for contributors to predict if their package is CRAN-ready may also bolster will to contribute.


## 4. Consult with the community to create or modify CRAN policy.

Publicly flagging policy changes some time before they come into effect can reduce policy ignorance and the associated burden of policy enforcement on CRAN administrators. It would also give contributors a chance to bring their work into line with policy without requiring threat of archive, reducing pressure and frustration. 

Publicly consulting on policy with the community has the added benefit of potentially identifying policies that stifle innovation in unexpected ways, or will motivate unanticipated work-arounds. These insights can reduce policy churn in the long term, along with associated administrator enforcement burden and contributor frustration.

## 5. Notify maintainers and users of any modifications made by CRAN to a package's source code.

When parties are unaware of CRAN modifications unfortunate wasteful events have been observed to occur:

* Authors unknowingly undo CRAN's changes in a subsequent submission causing problems that cost contributors and administrators time. 
* Users submit bug reports relating to CRAN changes leading to difficulty in reproducing issues.

It seems that some of these modifications may relate to intricacies of CRAN's environments, a further argument for reform 4.

At a minimum we propose that maintainers should receive an email, the package version number should be bumped, and users should receive an onLoad message. 

## 6. Publish a policy on re-submission intervals that can be consistently applied.

A recurring source of conflict between administrators and contributors arises when contributors submit too frequently. This may be due to the fact that the allowable frequency of submissions is left rubbery in CRAN policy. It is also unclear if submissions made at CRAN's request are included a contributor's notional quota.

This conflict could be removed if contributors received a set number of submissions per period. CRAN systems could automatically ensure they don't submit more than this, and it could be clear to contributors at all times how many submissions they have, or how long until they can next submit. Additional quota could be granted when making submissions requested by CRAN administrators. 

## 7. Cease punitive temporary submission bans for contributors with repeated rejections or test failures.

Administrators issuing punishments is a cumbersome process that involves effort in decision making, communication, and bookkeeping. Time can be saved by replacing it with more transparent, and automatic processes wherever possible. For example:

* Test failures could trigger automatic notifications, and automatically result in archival if they reach a persistence or recurrence threshold. Package status with respect to these thresholds could be publicly visible to users and contributors encouraging them to resolve these issues without administrator intervention.
* Rejections could be treated similarly to submissions, with a set quota of rejections available before a break period is automatically introduced. Contributors would be able to know at all times how much of their quota remains, and the break period that would result from exceeding it. 

## 8. Establish a governance model including a process by which community members can propose changes to CRAN policies or processes.

A public register of community proposals to be considered transparently is one way other open source peak bodies have handled demonstrating they are listening to communities they are receiving resources to serve (E.g. TC39 Proposals for Javascript, and Python Enhancement Proposals). The community perspective is also an important source of innovations that has ensured those organisations have continued to thrive.

If such a proposal mechanism existed there would have been no need for this petition.

## 9. Establish a code of conduct for the behaviour of CRAN administrators and contributors in their dealings.

A code of conduct would explain to contributors what they can expect in communications from CRAN administrators and what CRAN administrators expect from them. It helps avoid frustration between parties whose expectations do not align. It should also make it clear what will happen when those expectations are not met, and how such issues should be raised.

## 10. Publish minutes of CRAN governence meetings.

These documents are a vehicle for CRAN to communicate the issues administrators are dealing with. This gives the community context for the actions of CRAN administrators, and helps build empathy for them. They also alert the community to opportunities where they can offer solutions.

Highly relevant precedents for this are the published minutes for meetings of the various Bioconductor governance boards.

## 11. Establish a process whereby CRAN notifies the R community of shortfalls in resources which could be met by community contributions.

There is no reason, in a community as large and appreciative as ours, that a key piece of infrastructure like CRAN should struggle to scale due to lack of resources. We believe using community contributions to maintain the quality of the service is preferable to sacrificing quality in the name of efficiency. A community contribution mechanism could help ensure the quality of CRAN into the future. 
