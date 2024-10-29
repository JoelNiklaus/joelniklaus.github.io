---
layout: post 
title: The Broken Peer Review System: Some Ideas for Fixing it
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

# The Broken Peer Review System: Some Ideas for Fixing it

## What is the Problem?

During my four years in academia, I submitted numerous papers to academic conferences and made two attempts at journal
publication, though neither proved successful. All told, I made 32 submissions across 15 papers, meaning each paper was
submitted at least twice on average. While some fortunate manuscripts found their home on the first try, one particular
paper went through four submission cycles and still remains unpublished. Ironically, that one was among my favorites and
what I considered some of my best work. However, time hasn't been kind to it—the paper is now outdated and would require
additional experiments to be competitive for submission again.

Most academics are intimately familiar with the sting of negative reviews. Yet in my experience, the truly frustrating
aspects of peer review aren't the criticisms themselves, but rather reviews that demand nonsensical "improvements",
point out supposed weaknesses that we've already openly acknowledged in our limitations section, or assign low scores
while fixating on minor details. That said, I believe the NLP/ML/AI field stands out for its progressive approach to
academic publishing. Unlike many disciplines, most top-tier venues offer open access to publications, and the review
process moves at a comparatively brisk pace - typically 2-4 months versus the year-plus timeline common in other fields.
The ACL Rolling Review (ARR) system particularly exemplifies this forward-thinking attitude. Not only do they actively
[solicit community input through polls](https://www.aclweb.org/portal/content/survey-anonymity-period-policy) about
potential process changes, but they also implement corresponding reforms swiftly, as demonstrated by
their [recent updates to anonymity policies](https://aclrollingreview.org/anonymity). This responsive approach to
improving the publication process sets a valuable example for academia at large.

With the rise of ChatGPT and the unprecedented surge in NLP/ML/AI submissions
(see [NeurIPS](https://papercopilot.com/statistics/neurips-statistics)
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
Beyond these suggestions, I haven't seen much public discourse on this topic,
except [this recent tweet from Jakob Foerster](https://x.com/j_foerst/status/1848402835156635972?t=1005GjTOLmWPe2a0EBQuqA&s=19)
. In my view, achieving sustainable improvement will require more fundamental structural changes to the system.

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

## Problems with the Proposed Approach

### A Fixed Submission Price Does not Affect Everyone Equally

The impact of a 1,000 USD submission fee varies dramatically across academic institutions. For prestigious universities
like those in the Ivy League, such a fee may be insignificant, but it can represent a major obstacle for universities in
developing countries. To address this disparity, I propose scaling the fee based on the GDP (PPP) per capita of the
institution's home country.

While this metric may not perfectly account for institutional differences within large nations, it offers a
straightforward and universally accessible benchmark. For instance, the United States has a GDP (PPP) per capita of 86K
USD, compared to India's 11K
USD [according to the IMF](https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(PPP)_per_capita). This suggests that
submission fees for US institutions should be roughly 8 times higher than those for Indian institutions. In practice,
this would mean Stanford pays 1,000 USD per submission, while IIT Delhi would pay 128 USD.

However, for affluent organizations like Google, even a 1,000 USD fee is unlikely to influence their submission
decisions. While we could consider implementing higher rates for wealthy companies, I believe there's limited downside
to having them pay the standard US rate. This approach still helps subsidize submissions from less resourced
institutions, and importantly, maintains industry engagement – which can lead to valuable sponsorship opportunities for
the field.

### Ensuring Review Quality in a Paid System

The foundation of this proposal rests on the assumption that compensated reviewers will produce higher quality reviews.
However, this raises an important question: How can we prevent abuse from individuals seeking to maximize earnings
through low-effort reviews? Here are several potential safeguards:

#### Existing Quality Controls

We should maintain the current requirement that reviewers must have published at least one paper at the venue they're
reviewing for. This established filter effectively limits the pool to qualified candidates.

#### New Protective Measures

We could implement two additional controls:

1. Set a maximum number of reviews any individual can perform per review cycle
2. Implement a dynamic payment structure when there's an abundance of reviewers

**Dynamic Payment Structure**

Consider this scenario: We allocate 1000 USD per paper for reviews. Rather than splitting this equally, we could
distribute funds based on review quality rankings from meta-reviewers and/or authors. For example, we might implement an
exponential decay model:

- First-ranked reviewer: 500 USD
- Second-ranked reviewer: 250 USD
- And so forth

While this specific distribution might be too aggressive, it illustrates the concept. To maintain transparency,
reviewers would always know:

- The total number of reviewers in the pool for each paper
- The payment structure

This information allows reviewers to evaluate their interest in specific papers against the likelihood of receiving
higher compensation.

### Impact of Submission Fees on Venue Prestige and Paper Quality

An interesting paradox emerges when considering submission fees and their effect on paper quality. As fees increase, we
expect to see authors submitting higher-quality work, which likely leads to higher acceptance rates. However, this
improved acceptance rate could inadvertently reduce the perceived prestige of the venue, as selectivity often serves as
a proxy for excellence. One potential solution draws inspiration from the NLP community's "Findings" model. Under this
framework, the review process would operate in two tiers:

1. First, evaluate all submissions for scientific rigor and validity, accepting those that meet established quality
   standards
2. Then, from this pool of scientifically sound papers, select particularly innovative or influential works for
   conference presentation

This approach preserves high quality standards while maintaining the venue's selective nature for featured
presentations.

## Outlook

One potential approach would be implementing a review score-dependent submission fee structure. Under this system, a
baseline fee of 1000 USD would apply for submissions receiving an average score of 5/10. The fee would then adjust
dynamically: halving for each point increase in the average score, and doubling for each point decrease. This mechanism
would create a strong disincentive for low-quality submissions. However, such a system would only be viable if we can
ensure consistently high-quality reviews.

A more nuanced solution might combine this with a fee structure based on the submitting institution's GDP (PPP) per
capita. This hybrid approach would both discourage lower quality submissions while accounting for institutional wealth
disparities. The final fee would comprise two components: a base fee and a score-dependent fee, both normalized by the
GDP (PPP) per capita. Consider these illustrative examples:

- An Indian submission scoring 6/10: Total fee of 192 USD, consisting of a 128 USD base fee plus a 64 USD score-based
  fee (128 USD adjusted and halved due to scoring one point above the 5/10 baseline).
- A US submission scoring 3/10: Total fee of 5000 USD, consisting of a 1000 USD base fee plus a 4000 USD score-based
  fee (1000 USD adjusted and doubled twice for scoring two points below the 5/10 baseline).

However, this approach reveals a potential issue: students responsible for lower-scoring submissions might face
institutional consequences for incurring substantial costs to their university's budget. This concern suggests we should
consider moderating the score-based fee component by reducing both its magnitude and the multiplier effect. For
instance, instead of halving or doubling the fee for each one-point difference, these adjustments could apply per
two-point interval.

Thanks to Rylan Schaeffer and Mara Häusler for ideas and discussion around this!

# TODO: focus more on the incentives of the different people

# TODO: Konkreter sagen: meiste leute sehen probleme mit review prozess aber es existieren wenige konrere vorschläge für besseres system


