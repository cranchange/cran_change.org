An open letter to CRAN and the R Community

# Supporting this petition

We are now collecting feedback on the draft. Feel free to create an issue or PR to provide public feedback, or if you would prefer you can provide private feedback using a [Google form](https://forms.gle/iS5UFnv3yTtW6Dzg9). 

With this action we wish to advocate for a respectful dialogue about reforming the administration of CRAN's package ecosystem. We do not wish to disparage the contributions that have been provided to this point by CRAN.

When the petition is ready in addition to signing the petition there are several steps R community members can take to show their support for these reforms:

1. Share this petition with your network.
2. Participate and contribute on the R ecosystem beyond using R and developing packages. Such as the [R Contributing Working Group](https://forwards.github.io/rcontribution/)
3. Other initiatives 

# Motivation for this letter

This letter has been written after observing some harmful practices that we believe damage the current trust on the resources. We know that most practices are positive and have fueled the success of CRAN. Nonetheless, we believe three practices are harmful:

**Rejecting submissions based on undocumented criteria, or inconsistently applied criteria** makes it difficult for contributors to predict if their submissions will be accepted without issues, and so erodes willingness to contribute. For example:

  * There seems to have been an undocumented change in stance toward examples, with many contributors reporting CRAN reviewers are rejecting submissions citing not enough examples whilst also refusing to accept any examples with `\dontrun{}` and `\donttest{}`. These blocks were previously accepted as standard practice. 
  * On multiple occasions packages premised on colour palettes have been rejected due to triviality only to have other packages with almost identical premises, and of similar complexity be accepted shortly after. 
  
This practice wastes the time of both CRAN reviewers and contributors. We believe the submission burden on both sides could be significantly reduced by fully documenting acceptance criteria, and reducing ambiguity with guidance and examples. 

**Archiving packages for a small number of test failures on proprietary platforms** harms package test coverage. For example:

  * Recently a package with 100% test coverage and over 2000 tests was archived when 2 of those tests began failing on an expensive proprietary platform. The failure could not be reproduced on RHub.
  
This practice discourages extensive testing on CRAN, and has already lead developers among us to limit functionality exposed to CRAN to low-risk subsets. The degradation of the reverse dependency checking system in this way weakens both packages and the R language itself, since package checks are used to validate core changes.

**Archiving packages with little or no warning** discriminates against contributors with less time available on short notice. Typical periods attached to the threat of archival seem to range in zero to six weeks. Under this practice there are many categories of contributor who will find it difficult to keep their work on CRAN, for example:

  * Contributors who have no paid time to work on open source
  * Contributors with families or others who depend on them
  * Contributors who are unwell or on leave

Aside from the nature of these actions, the tone taken by CRAN reviewers in their communications with contributors is at times abrupt and unsympathetic. This routinely takes new contributors by surprise since it is out of step with the norms of the larger R community. 

Contributors are a precious resource and discouraging them threatens CRAN's 'comprehensive' aspect.

The fact that there is currently no avenue by which R community members can engage CRAN on these topics points to an operating model that our community may have outgrown. There are aspects of the way CRAN works that we feel are unnecessarily opaque, and incompatible with the open nature of the R community and its other governing bodies.
