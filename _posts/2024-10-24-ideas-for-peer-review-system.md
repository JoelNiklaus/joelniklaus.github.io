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

## What is the Problem?

I spent four years in academia and submitted my fair share of papers to academic conferences (and twice to a journal, unfortunately to no avail). 
In total, I made 32 submissions for 15 papers. So on average, I submitted each paper at least twice. 
Some lucky papers found a home the first time, but another one I submitted four times, and it still remains unpublished. 
Especially that one, I actually really liked and considered one of my best works. 
However, now it is outdated and requires additional experiments to again be a competitive submission.

I would say most academics know the bad feeling that negative reviews evoke. 
But in my opinion, the most frustrating experience in the entire process are reviews that ask for nonsense "improvements", only list as weaknesses points we openly discuss in the limitations or give low scores while criticizing minor details.
In general, I think the field of NLP/ML/AI is quite progressive, compared to other fields.
For example, most top-tier publications are open-access and the review process is fast (2-4 months vs more than a year for other fields).
The ACL Rolling Review (ARR) even [conducts polls](https://www.aclweb.org/portal/content/survey-anonymity-period-policy) regarding changes to the review process and then actually [changes the process quickly](https://aclrollingreview.org/anonymity) based on the results!

However, with the advent of ChatGPT and the recent surge of submission in the field of NLP/ML/AI (see [NeurIPS](https://papercopilot.com/statistics/neurips-statistics) and [ICLR](https://papercopilot.com/statistics/iclr-statistics)) I feel like the review quality is dropping further. 
I get it, people are busy and have many other priorities. In addition, reviewing is often anonymous and not paid.
It is great to see such a huge inflow of people into the field, but it exacerbates the peer review problem due to record-breaking submission numbers every year.
Currently, the cost of making a submission is quite small. One way of getting more reviewers is requiring authors to review when submitting papers, as recently enacted by [ARR](https://aclrollingreview.org/reviewing-workload-requirement) and [CVPR](https://cvpr.thecvf.com/Conferences/2025/CVPRChanges).
While this may alleviate the problem, I am not sure, it solves it. I could imagine that authors forced to review may see it as a unwanted chore, possibly leading to low-quality reviews. 
As far as I know, there is no quality control process in place leading to desk-rejection of author's papers in case their reviews are of low quality.
There are other ideas for improving the peer review system like [giving more credit](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7029384) [to reviewers](https://blog.degruyter.com/the-ideal-future-of-peer-review-through-the-editors-lens) or assisting the process through [AI tools](https://www.researchinformation.info/feature/how-do-we-improve-peer-review) (apart from that, I haven't really seen much discussion around this online). 
However, I believe we need more drastic structural changes for sustainable change.

## A Potential Solution

We need to associate a cost to a submission. In Switzerland, where I live, the [Polluter Pays Principle](https://en.wikipedia.org/wiki/Polluter_pays_principle) (Verursacherprinzip in German) is important and often followed in political discourse.
It says that the people who cause the damages to a common good (i.e., make submissions) should pay the costs (i.e., review). 
Currently, in most peer reviewed venues there is no direct connection, to my knowledge.

Here is how I imagine the system:
Submitting a paper costs 1000 USD. From that we can pay 200 USD per reviewer (4 times), 150 USD for the meta-reviewer and 50 USD for the program-chair.  
1000 USD is a drop in the bucket for most universities compared to the costs of actually producing the research.
However, 200 USD for writing a review is a welcome addition for many PhD students doing most of the reviewing. 
Since we now have a monetary reward for reviewing services, it makes reviewing attractive, and it allows us to put quality controls in place. 
For example, we may only want to pay out the reward if the meta-reviewer and/or the authors rate the review as sufficient.

This idea does not come completely out of the blue: In court proceedings we also pay professionals for expert opinions.
Like in law, in science we build a network of precedence, so ensuring this body is of high quality, should be of utmost importance.

As mentioned above, CVPR and ARR already make authors review. So how is it different to just forcing authors to review?
- The submitting authors might not be motivated or suited to review
- Due to pay for reviewers we have more leverage to expect quality reviews
- Since there is a market, it allows for more efficient allocation of time globally

## Further Thoughts
1000 USD might not be a lot for an ivy league university, but it might be for universities in developing countries for example. 
Also, 200 USD is a lot of money in many countries, but we may need to compensate researchers more in places with high living costs. 
It might be worth thinking about how we can adjust these numbers based on the institutions people work at and places people live in.

Another potential problem might be the following:
When the cost of a submission rises, the quality of submitted papers likely rises alongside, so the acceptance rate may need to rise with it. This means the venue may be seen as less selective and prestigious. 
There I would propose a system similar to Findings in the NLP community, where the main review process ensures that the accepted papers are sound. 
The conferences then further select the exciting papers from all sound papers to be presented at the conference.
