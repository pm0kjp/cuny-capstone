# Possessive Pronoun Usage in Bloggers with ASD

## Contents of This Repository

Each subdirectory will have its own README that can provide detailed information about its contents.

* [Documentation](documentation)
	- [Glossary](documentation/glossary.md) 
	- [Methods](documentation/Methods.md) 
* [Lit Review](lit_review)
	- [Search Results from Google Scholar: Autism and Blogging](lit_review/google_scholar_bloggers.md)
	- [Search Results from Google Scholar: Autism and Pronouns](lit_review/google_scholar_pronouns.md)
	- [Search Results from Pubmed: Autism and Pronouns](lit_review/pubmed_autism_pronouns.md)
	- [Articles Referenced From Other Articles](lit_review/referenced_articles.md)
	- [Lit Review Outline](lit_review/lit_review_outline.md)
	- [Lit Review Draft](lit_review/lit_review_draft.md)
* [Scripts](scripts)
	- [Blog Scraper](scripts/scrape_blogs.ipynb)
	- [Blog Analyzer](scripts/analyze_blogs.ipynb)
	- [TF/IDF Analyzer](scripts/tf_idf_analysis.ipynb)
	- [Watson Topic Analyzer](scripts/watson_analysis.ipynb)
	- [Statistical Comparison](scripts/statistical_comparisons.ipynb)

## What is *Not* Included in This Repository

This study requires lists of blogs, both cases (autistic bloggers) and controls (bloggers who do not self-disclose an autism diagnosis).  For purposes of human subjects protection, these lists are not included.  Additionally, scripts in this repository generate text corpora extracted from the listed blogs.  Again, these texts are not included in the repository.  Detailed instructions for how to create lists comparable to the ones used here are included in scripts and README files to allow for maximal reproducibility while maintaining confidentiality for bloggers.

Additionally, topic matching was done using the IBM Watson topic concept analyzer, which requires an API username and password.  These credentials were not included in this repository but can be generated free of charge by anyone interested in replicating this study.

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

Because we are dealing with human subjects (writing samples found on public blogs), we have to consider human subjects protection.  I have completed human subjects protection training and been approved for an IRB exemption from oversight (CUNY IRB submission number 2018-0208).  

The research proposal was reviewed on 03/05/2018 and does not require CUNY HRPP or IRB review.  It does not involve human subjects as defined by CUNY HRPP: A living individual about whom an investigator (whether professional or student) conducting research obtains (1) data through Intervention or interaction with the individual, or (2) identifiable private information. 

This study is exempt from review under exemption type 4.  This author has completed Human Subjects Protection training through CITI and has instituted data protections to maintain the confidentiality of bloggers included in this study.

### Literature Review

Lit review is under construction right now.  There is a [very rough draft](lit_review/lit_review_draft.md) as well as some [notes on various publications](lit_review) in this repo.

### Cohort Selection

The initial potential cohort of cases consisted of over 1600 blogs written by people who self-disclose an autism diagnosis.  Then, this list was filtered such that only WordPress bloggers with clear evidence of being over age 18 were selected.  

The controls cohort was created by searching for WordPress blogs unrelated to autism.  The list was filtered by topic matching, such that there is a 1:1 case:control model with individual blog posts matched by topic.  Topic was determined using IBM Watson topic concept parsing.

### Blog Mining

Blog scraping will take place using Beautiful Soup 4, a python package.

### Linguistic Analysis

I will gather data on pronoun usage and other parts of speech based on the Penn Treebank part of speech tagger in the Natural Language Tool Kit.

### Topic Matching

We will match cases and controls based on topic using Watson topic analyzer, meta keyword analysis, and/or TF/IDF keyword extraction.

### Statistical Methods

Group differences will be measured by analyzing mean proportion of possessive pronouns using an independent two-sample T-test.

### Disclosure of Findings

