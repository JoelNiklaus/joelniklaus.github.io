---
layout: post 
title: The Broken Peer Review System: Some Ideas for fixing it
date: 2024-08-17
---

<!--
Paper Submission Tracking:
Legalbench: A collaboratively built benchmark for measuring legal reasoning in large language models: 1 => conference
MultiLegalSBD: a multilingual legal sentence boundary detection dataset: 1 => conference
Towards Explainability and Fairness in Swiss Judgement Prediction: Benchmarking on a Multilingual Dataset: 1 + 1 => conference
Resolving Legalese: A Multilingual Exploration of Negation Scope Resolution in Legal Documents: 1 + 1 => conference
Swiss-judgment-prediction: A multilingual legal judgment prediction benchmark: 1 => workshop
ClassActionPrediction: A challenging benchmark for legal judgment prediction of class action cases in the US: 1 => workshop
Automatic Anonymization of Swiss Federal Supreme Court Rulings: 1 => workshop
LEXTREME: A multi-lingual and multi-task benchmark for the legal domain: 2 + 1 => conference
Multilegalpile: A 689gb multilingual legal corpus: 2 + 2 => conference
An empirical study on cross-x transfer for legal judgment prediction: 2 => conference
LegalLens: Leveraging LLMs for Legal Violation Identification in Unstructured Text: 2 => conference
Anonymity at Risk? Assessing Re-Identification Capabilities of Large Language Models in Court Decisions: 2 + 1 => conference
Can we Pretrain a SotA Legal Language Model on a Budget From Scratch?: 2 => workshop
FLawN-T5: An Empirical Examination of Effective Instruction-Tuning Data Mixtures for Legal Reasoning: 3 => conference
One Law, Many Languages: Benchmarking Multilingual Legal Reasoning for Judicial Support: 3 + 1 => unpublished
-->

# The Broken Peer Review System: Some Ideas for fixing it

## What is the Problem?

During my four years in academia, I submitted numerous papers to academic conferences and made two attempts at journal
publication, though neither proved successful. All told, I made 32 submissions across 15 papers, meaning each paper was
submitted at least twice on average. While some fortunate manuscripts found their home on the first try, one particular
paper went through four submission cycles and still remains unpublished. Ironically, that one was among my favorites and
what I considered some of my best work. However, time hasn't been kind to it—the paper is now outdated and would require
additional experiments to be competitive for submission again.

Most academics are intimately familiar with the sting of negative reviews. Yet in my experience, the truly frustrating
aspects of peer review aren't the criticisms themselves, but rather reviews that demand nonsensical "improvements,"
point out supposed weaknesses that we've already openly acknowledged in our limitations section, or assign low scores
while fixating on minor details. That said, I believe the NLP/ML/AI field stands out for its progressive approach to
academic publishing. Unlike many disciplines, most top-tier venues offer open access to publications, and the review
process moves at a comparatively brisk pace - typically 2-4 months versus the year-plus timeline common in other fields.
The ACL Rolling Review (ARR) system particularly exemplifies this forward-thinking attitude. Not only do they actively
[solicit community input through polls](https://www.aclweb.org/portal/content/survey-anonymity-period-policy) about
potential process changes, but they also implement corresponding reforms swiftly, as demonstrated by
their [recent updates to anonymity policies](https://aclrollingreview.org/anonymity). This responsive approach to
improving the publication process sets a valuable example for academia at large.

With the rise of ChatGPT and the unprecedented surge in NLP/ML/AI submissions (
see [NeurIPS](https://papercopilot.com/statistics/neurips-statistics)
and [ICLR](https://papercopilot.com/statistics/iclr-statistics) statistics), review quality seems to be declining
further. This is understandable – reviewers are overwhelmed with competing priorities, and the work is both anonymous
and unpaid. While the field's growing popularity is exciting, the record-breaking submission numbers each year intensify
the peer review challenges. Currently, submitting a paper requires minimal effort. Some venues
like [ARR](https://aclrollingreview.org/reviewing-workload-requirement)
and [CVPR](https://cvpr.thecvf.com/Conferences/2025/CVPRChanges) have attempted to address reviewer shortages by
requiring authors to serve as reviewers. However, this approach may not be a complete solution. Authors who view
reviewing as an unwanted obligation might produce low-quality reviews. To my knowledge, there's no quality control
system in place that would desk-reject papers from authors who submit subpar reviews. Other proposed improvements to the
peer review system include
providing [more recognition](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7029384) [for reviewers](https://blog.degruyter.com/the-ideal-future-of-peer-review-through-the-editors-lens)
and incorporating [AI-assisted tools](https://www.researchinformation.info/feature/how-do-we-improve-peer-review).
Beyond these suggestions, I haven't seen much public discourse on this topic. In my view, achieving sustainable
improvement will require more fundamental structural changes to the system.

## A Potential Solution

In Switzerland, where I live, the [Polluter Pays Principle](https://en.wikipedia.org/wiki/Polluter_pays_principle) (
Verursacherprinzip in German) plays a significant role in political discourse. This principle states that those who
generate costs by using common resources should bear those costs. Applied to academic publishing, this would suggest
that authors submitting papers (the "polluters") should compensate for the review effort they necessitate. However, to
my knowledge, most peer-reviewed venues currently lack such a direct cost-responsibility connection.

The proposed system works as follows: Authors pay 1000 USD to submit a paper. This fee is distributed among the review
team - 200 USD for each of the four reviewers, 150 USD for the meta-reviewer, and 50 USD for the program chair. While
1000 USD represents a minimal expense for universities compared to the actual cost of conducting research, the 200 USD
reviewer payment provides meaningful compensation for PhD students, who typically handle most reviews. By introducing
this monetary incentive, reviewing becomes an attractive task. Moreover, the payment structure enables quality control
measures - for instance, we could make payment contingent on the meta-reviewer's or authors' assessment of the review
quality.

The concept has established precedent: courts routinely compensate professionals for their expert opinions. Just as
legal systems rely on case law and precedent, science builds upon a network of prior work. Therefore, ensuring the
quality of this foundational knowledge should be paramount. While conferences like CVPR and ARR already require authors
to review papers, paid reviewing offers distinct advantages:

- Rather than depending on potentially unmotivated or unsuitable authors for reviews, we can select qualified reviewers
- Financial compensation provides leverage to demand and enforce high-quality reviews
- Creating a market for reviews enables more efficient global allocation of expertise and time

The result is more thoughtful, robust peer review that better serves the scientific community.

## Further Thoughts

The significance of a 1,000 USD submission fee varies greatly across academic institutions. While this might be a
negligible amount for Ivy League universities, it could pose a substantial barrier for universities in developing
nations. Similarly, while 200 USD may seem modest in some regions, it represents a significant sum in others. We should
consider implementing a flexible fee structure that accounts for both institutional resources and regional cost of
living when determining appropriate compensation for researchers.

An additional consideration emerges regarding submission fees and paper quality. As submission costs increase, we
expect to observe a corresponding rise in paper quality, which may necessitate higher acceptance rates. This could
potentially diminish the perceived selectivity and prestige of the venue. To address this, we might adopt an approach
similar to the "Findings" model used in the NLP community. Under this system, the primary review process would focus on
ensuring scientific soundness across all accepted papers, while conferences would then select particularly innovative or
impactful works from this pool for presentation.
