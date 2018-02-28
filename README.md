# Possessive Pronoun Usage in Bloggers with ASD

## Contents of This Repository

* [Glossary of terms](documentation/glossary.md)
* [Lit Review notes](documentation/lit_review.md)

## Background and Goals

[Preliminary, exploratory research](https://github.com/pm0kjp/neurodiverse-blog-data-miner) by this author on part of speech usage in bloggers who self-disclose an ASD (autism spectrum disorder) diagnosis found that bloggers with ASD use fewer possessive pronouns (_his_, _hers_, _my_, etc.) than bloggers who do not disclose a an ASD diagnosis (and are presumed to have typical development).  

This finding is consistent with other analyses on spoken communication in ASD, and may be explained by a lack of "common ground" (mutually understood shared mental model of conversation topic) in spoken communication.  __(Lit review here!)__  To my knowledge, no analysis has been done on written communication without a specific interlocutor.  This project seeks to extend existing scholarship on linguistic differences in ASD to communications like blog posts.

In this version of my research, I intend to mine a larger number of texts by more bloggers, with more carefully chosen controls.  My research questions include:

* Do bloggers who self-disclose an ASD diagnosis use significantly fewer possessive pronouns than bloggers who do not self-disclose an ASD diagnosis?  
* If so, can this be explained by factors other than ASD diagnosis (e.g. blog topic, semantic complexity, post length, age, sentiment valence, etc.?)
* If there is indeed a difference in possessive pronoun usage which seems to be explained by ASD diagnosis, what language tools, if any, are being employed by bloggers with ASD to compensate for the lack of possessive pronouns?
 - Is there simply less reference to possession, possibly signaling different pragmatic language choices by bloggers with ASD?
 - Or are bloggers with ASD using possessive nouns (_mom's_, _David's_, _the teacher's_) to replace possessive pronouns, perhaps indicating a difference in linguistic common ground?

## Hypothesis

For research to be truly reproducible, hypotheses should be declared ahead of any conduct of research.  Based on prior exploration and lit review, I hypothesize the following:

* There will be a group difference between autistic and non-autistic bloggers with regard to the use of possessive pronouns.  Autistic bloggers will use fewer possessive pronouns.
* Qualitative textual analysis will reveal that the reduction in possessive pronouns is accompanied by the use of noun phrases to replace / compensate for the lack of possessive pronouns.
* Subject pronouns may also be reduced in the autistic blogger group.
* Qualitative textual analysis may also reveal subtle deficits in theory of mind, such as sudden topic changes, unclear referents, or overly pedantic narration.
* Because autistic bloggers constitute an unusual sample of autistic people and have strong language skills and motivation to communicate, the differences detected here will have a relatively small effect size and will not rise to the point of being predictive.  

## Project Plan

### Human Subjects Protection

This study is exempt from review under exemption 4.  This author has completed Human Subjects Protection training through CITI.

### Literature Review

Lit review is under construction right now.  There is a [very rough draft](lit_review/lit_review_draft.md) as well as some [notes on various publications](lit_review) in this repo.
### Cohort Selection

 The more difficult cohort to assemble will be bloggers with self-disclosed autism.  Once that cohort is complete, preliminary analysis on blog topics will allow me to see if matching controls by topic will be doable.

### Blog Mining

Blog scraping will take place using Beautiful Soup 4, a python package.

### Linguistic Analysis

I will gather data on pronoun usage and other parts of speech based on the Penn Treebank part of speech tagger in the Natural Language Tool Kit.

### Statistical Methods

Group differences will be measured by analyzing mean proportion of possessive pronouns using an independent two-sample T-test.

### Disclosure of Findings

