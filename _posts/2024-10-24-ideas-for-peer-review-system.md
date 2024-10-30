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
the peer review challenges. Currently, submitting a paper requires minimal effort. There are only few checks allowing
for desk-rejecting low-quality papers leading to lower reviewing load. Some venues
like [ARR](https://aclrollingreview.org/reviewing-workload-requirement)
and [CVPR](https://cvpr.thecvf.com/Conferences/2025/CVPRChanges) have attempted to address reviewer shortages by
requiring authors to serve as reviewers. However, this approach may not be a complete solution. Authors who view
reviewing as an unwanted obligation might produce low-quality reviews. To my knowledge, there's no quality control
system in place that would desk-reject papers from authors who submit subpar reviews.

Other proposed improvements to the peer review system include
providing [more recognition](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7029384) [for reviewers](https://blog.degruyter.com/the-ideal-future-of-peer-review-through-the-editors-lens)
and incorporating [AI-assisted tools](https://www.researchinformation.info/feature/how-do-we-improve-peer-review).
Beyond these suggestions, I haven't seen much public discourse on this topic,
except [this recent tweet from Jakob Foerster](https://x.com/j_foerst/status/1848402835156635972?t=1005GjTOLmWPe2a0EBQuqA&s=19)
. While there appears to be broad consensus in academia that the current peer review system falls short of its goals,
concrete proposals for systemic reform seem to be lacking. I believe that lasting improvements will require deeper, more
fundamental changes to the existing structure.

## A Potential Solution

In Switzerland, where I live, the [Polluter Pays Principle](https://en.wikipedia.org/wiki/Polluter_pays_principle)
(Verursacherprinzip in German) plays a significant role in political discourse. This principle states that those who
generate costs by using common resources should bear those costs. Applied to academic publishing, this would suggest
that authors submitting papers (the "polluters") should compensate for the review effort they necessitate. However, to
my knowledge, most peer-reviewed venues currently lack such a direct cost-responsibility connection.

The proposed system works as follows:

### Author Side

A paper receiving an average review score of 5/10 incurs a base fee of 1000 USD to cover review expenses (base
component), with conference attendance included at no additional cost for accepted papers. The fee adjusts dynamically
based on review performance (score-based component): halving for each point increase in the average score, and doubling
for each point decrease. This pricing structure creates a powerful deterrent against premature or substandard
submissions while rewarding exceptional work. However, implementing such a system would only be feasible if we can
guarantee consistent, high-caliber peer reviews.

### Program Committee Side

The income generated through these submission fees is distributed among the program committee - 200 USD for each of the
four reviewers, 150 USD for the meta-reviewer, and 50 USD for the program chair. While 1000 USD represents a minimal
expense for universities compared to the actual cost of conducting research, the 200 USD reviewer payment provides
meaningful compensation for PhD students, who typically handle most reviews. By introducing this monetary incentive,
reviewing becomes an attractive task. Moreover, the payment structure enables quality control measures - for instance,
we could make payment contingent on the meta-reviewer's and/or authors' assessment of the review quality.

This concept has established precedent: courts routinely compensate professionals for their expert opinions. Just as
legal systems rely on case law and precedent, science builds upon a network of prior work. Therefore, ensuring the
quality of this foundational knowledge should be paramount. While conferences like CVPR and ARR already require
submitting authors to review papers, paid reviewing offers distinct advantages:

- Rather than depending on potentially unmotivated or unsuitable authors for reviews, we can select qualified reviewers
- Financial compensation provides leverage to demand and enforce high-quality reviews
- Creating a market for reviews enables more efficient global allocation of expertise and time

The result is more thoughtful, robust peer review that better serves the scientific community.

## Problems with the Proposed Approach

While this proposed system offers to address the issue of premature submissions, low-quality reviews, and lack of
reviewers, it may lead to new problems such as increased administration, unequal impact of fixed submission prices on
different authors, challenges in ensuring review quality within a paid system, and potential effects on venue prestige
and paper quality due to submission fees. The following section examines these potential problems and explores
strategies to mitigate or resolve them.

### Increased Administration

While implementing a payment system for submissions and reviewer compensation may introduce additional administrative
complexity, modern technology makes this manageable. Although OpenReview serves as a mature platform supporting numerous
leading conferences with various use cases, it currently lacks payment functionality, to my knowledge. Despite the
initial overhead of establishing such a system, the significant improvements to peer review quality justify this
investment. In my opinion, the long-term benefits of a more robust and accountable review process clearly outweigh the
short-term administrative challenges.

### A Fixed Submission Fee Creates Unequal Access

The impact of a 1,000 USD submission fee varies dramatically across academic institutions. For prestigious universities
like those in the Ivy League, such a fee may be insignificant, but it can represent a major obstacle for universities in
developing countries. To address this disparity, I propose scaling the fee based on the GDP (PPP) per capita of the
institution's home country.

While this metric may not perfectly account for institutional differences within large nations, it offers a
straightforward and universally accessible benchmark. For instance, the United States has a GDP (PPP) per capita of 86K
USD, compared to India's 11K
USD [according to the IMF](https://en.wikipedia.org/wiki/List_of_countries_by_GDP_(PPP)_per_capita). This suggests that
submission fees for US institutions should be roughly 8 times higher than those for Indian institutions. Consider these
illustrative examples:

- An IIT Delhi submission scoring 6/10: The US base fee of 1000 USD is normalized to India, resulting in an adjusted
  base fee of 128 USD. Then it is halved due to scoring one point above the 5/10 baseline, resulting in a final fee of
  64 USD.
- A Stanford submission scoring 3/10: The US base fee of 1000 USD stays constant. Then it is doubled twice for scoring
  two points below the 5/10 baseline, resulting in a final fee of 4000 USD.

However, for affluent organizations like Google, even a 1,000 USD fee is unlikely to influence their submission
decisions. While we could consider implementing higher rates for wealthy companies, I believe there's limited downside
to having them pay the standard US rate. This approach still helps subsidize submissions from less resourced
institutions, and importantly, maintains industry engagement – which can lead to valuable sponsorship opportunities for
the field.

### Moderating Score-Based Component to Protect Student Interests

Students responsible for lower-scoring submissions might face institutional consequences for incurring substantial costs
to their university's budget due to exploding fees caused by the score-based component. This concern suggests we should
consider moderating the score-based component by reducing both its magnitude and the multiplier effect. For instance,
instead of halving or doubling the fee for each one-point difference, these adjustments could apply per two-point
interval.

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

Consider this scenario: We allocate 800 USD per paper for reviews. Rather than splitting this equally, we could
distribute funds based on review quality rankings from meta-reviewers and/or authors. For example, we might implement an
exponential decay model:

- First-ranked reviewer: 400 USD
- Second-ranked reviewer: 200 USD
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

## Incentives of the Different Players

There are two main players involved in the peer review system at major CS conferences: authors and program committee (
reviewers, area chairs, senior area chairs and program chairs). In this section, I discuss the incentives of these
groups in the current and new system respectively.

### Current System

Authors' Incentives:

- Submit as many papers as possible since it's free
- Submit early versions to get "free feedback"
- Make minimal revisions and resubmit quickly after rejection since reviews are random

Reviewers' Incentives:

- Review minimally to fulfill obligations (e.g., for ARR/CVPR requirements)
- Little incentive for detailed, thoughtful feedback
- May rush reviews due to competing priorities
- May be overly harsh/lenient since there's no accountability
- May give harsh scores to boost relative chances of own papers in submission

### Proposed System

Authors' Incentives:

- Submit more polished work to justify the fee
- Consider more internal review before submission
- Think twice before submitting borderline papers

Reviewers' Incentives:

- Financial motivation to take on reviews
- Quality matters if payment is tied to meta-reviewer/author ratings
- Compete to be selected as reviewer based on expertise/track record
- Potentially focus on quantity over quality to maximize earnings
- May give harsh scores to generate more resubmissions (and thus more review opportunities)

## Outlook and Rollout

If one venue adopts this policy it may receive less submissions in the beginning, but it will quickly get many more
reviewers. At some point a virtuous cycle may develop, where more and more reviewers will flock to the new conference
where they get paid, leading to higher quality reviews and faster turnaround times. This in turn is attractive to
authors, who will be more likely to submit there in the future, leading the venue to grow.

How do we roll out such fundamental changes in practice? ARR continues to set a progressive example for democratic and
iterative improvements to the review process: They recently formed
the "[ACL Peer Review Standing Committee](https://www.aclweb.org/portal/content/acl-peer-review-standing-committee): a
new body tasked with making data-driven recommendations for the design and implementation of the peer review process
at *CL conferences". Currently, they are [soliciting feedback](https://tinyurl.com/arr-design-survey) from the community
on "the decoupling of reviews and conference decisions, the length/frequency of review cycles, the commitment process,
and the role and acceptance rate of Findings". While the changes proposed in this post are much more fundamental, I
believe these topics could be deliberated in similar committees and eventually put to a community vote.

## Conclusion

In conclusion, the current peer review system in academia --explored at the example of NLP/ML/AI-- faces significant
challenges, including an overwhelming number of submissions, inconsistent and low-quality reviews, and a lack of
incentives for both authors and reviewers. The proposed solution of implementing submission fees and compensating
reviewers aims to address these issues by creating stronger deterrents against premature or low-quality submissions,
while incentivizing reviewers to provide more thoughtful and robust feedback. While this approach introduces new
potential problems around increased administration, unequal access, and the impact on venue prestige, these issues are
not insurmountable and the potential benefits of a more accountable and efficient peer review process justify exploring
such a model. Ultimately, lasting improvements to academic publishing will require a fundamental restructuring of the
existing system, and the ideas presented here offer a starting point for further discussion and refinement within the
research community.

<!-- 
## Acknowledgements

Thanks to Rylan Schaeffer and Mara Häusler for ideas and discussion around this!

TODO: First write a reply to Foersters post tagging him 
TODO: Send post to percy, matthias, chris für feedback
TODO: Then write twitter and linkedin summary posts publicizing it
-->



