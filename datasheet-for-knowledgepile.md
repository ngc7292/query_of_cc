# Datasheet for dataset "Knowledge Pile"

Questions from the [Datasheets for Datasets](https://arxiv.org/abs/1803.09010) paper, v7.

Jump to section:

- [Motivation](#motivation)
- [Composition](#composition)
- [Collection process](#collection-process)
- [Preprocessing/cleaning/labeling](#preprocessingcleaninglabeling)
- [Uses](#uses)
- [Distribution](#distribution)
- [Maintenance](#maintenance)

### For what purpose was the dataset created? 

The **Knowledge Pile** is utilized enhance the knowledge-related and reasoning capabilities of LLMs through the data collected by *Query of CC".

### Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)?

InternLM team

### Who funded the creation of the dataset? 

School of Computer Science, Fudan University and Shanghai AI Laboratory

### Any other comments?

## Composition

All instances of the dataset are text-only documents, which come from Common Crawl

### What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)?

All instances of the dataset are text-only documents, which extrated from web pages.

### How many instances are there in total (of each type, if appropriate)?

735GB disk size, 188B tokens (using Llama2 tokenizer).

### Does the dataset contain all possible instances or is it a sample (not necessarily random) of instances from a larger set?

Our dataset using *Query of CC* method collect some knowledge-related data from Common Crawl.

### What data does each instance consist of? 

"Raw" data and URL which the data come from
 
### Is there a label or target associated with each instance?

No

### Is any information missing from individual instances?

Perhaps some URL fields will be missing.

### Are relationships between individual instances made explicit (e.g., users’ movie ratings, social network links)?

These data only have Raw data and not have relation in our dataset.

### Are there recommended data splits (e.g., training, development/validation, testing)?

No, the user can split themself.

### Are there any errors, sources of noise, or redundancies in the dataset?

The content is retrieved from Common Crawl, so there may be some noise and error text present.

### Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g., websites, tweets, other datasets)?

No

### Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by doctor-patient confidentiality, data that includes the content of individuals’ non-public communications)?

The content is retrieved from Common Crawl, so there may be some confidential information, if you find some confidential information, please contact us.

### Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety?

The content is retrieved from Common Crawl, so there may be some toxic data , if you find these, please contact us.

### Does the dataset relate to people? 

No

### Does the dataset identify any subpopulations (e.g., by age, gender)?

No

### Is it possible to identify individuals (i.e., one or more natural persons), either directly or indirectly (i.e., in combination with other data) from the dataset?

No

### Does the dataset contain data that might be considered sensitive in any way (e.g., data that reveals racial or ethnic origins, sexual orientations, religious beliefs, political opinions or union memberships, or locations; financial or health data; biometric or genetic data; forms of government identification, such as social security numbers; criminal history)?

Maybe, the content is retrieved from Common Crawl, so there may be the data  might be considered sensitive in any way, if you find these, please contact us.

### Any other comments?

## Collection process

Our collection process have described at our paper [Query of CC: Unearthing Large Scale Domain-Specific Knowledge from Public Corpora](https://arxiv.org/pdf/2401.14624.pdf).

### How was the data associated with each instance acquired?

All content are retrieved from Common Crawl, which come from the web site.

### What mechanisms or procedures were used to collect the data (e.g., hardware apparatus or sensor, manual human curation, software program, software API)?

We use Elastic Search, Large language model(Llama) and some other software for post processing the dataset.

### If the dataset is a sample from a larger set, what was the sampling strategy (e.g., deterministic, probabilistic with specific sampling probabilities)?

We use *Query of CC* to collect the **Knowledge Pile**. 

### Who was involved in the data collection process (e.g., students, crowdworkers, contractors) and how were they compensated (e.g., how much were crowdworkers paid)?

No.

### Over what timeframe was the data collected?

We use the CC dump which the timestamp from 2016 to April 2023.

### Were any ethical review processes conducted (e.g., by an institutional review board)?

Not yet.

### Does the dataset relate to people?

No

## Preprocessing/cleaning/labeling


### Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)?

No, we provide the "Raw" data.

### Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?

Yes

### Is the software used to preprocess/clean/label the instances available?

Yes.

### Any other comments?

No.

## Uses


### Has the dataset been used for any tasks already?

**Knowledge Pile** can improve the ability of the large language model in solving some knowledge-related tasks and reasoning tasks.

### Is there a repository that links to any or all papers or systems that use the dataset?

Query of CC: Unearthing Large Scale Domain-Specific Knowledge
from Public Corpora [📄](https://arxiv.org/pdf/2401.14624.pdf)

### What (other) tasks could the dataset be used for?

Maybe high-quaility data can improve the base abiliyu of LLMs.

### Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses?

No.

### Are there tasks for which the dataset should not be used?

No.

### Any other comments?

## Distribution

### Will the dataset be distributed to third parties outside of the entity (e.g., company, institution, organization) on behalf of which the dataset was created? 

No

### How will the dataset will be distributed (e.g., tarball on website, API, GitHub)?

We released a subset of **Knowledge Pile** in [huggingface](https://huggingface.co/datasets/Query-of-CC/Knowledge_Pile).

### When will the dataset be distributed?

**Knowledge Pile** have been released.

### Will the dataset be distributed under a copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?

No.

### Have any third parties imposed IP-based or other restrictions on the data associated with the instances?

No.

### Do any export controls or other regulatory restrictions apply to the dataset or to individual instances?

No.

### Any other comments?

## Maintenance

### Who is supporting/hosting/maintaining the dataset?

### How can the owner/curator/manager of the dataset be contacted (e.g., email address)?

zyfei20@fudan.edu.cn, lilinyang@pjlab.org.cn

### Will the dataset be updated (e.g., to correct labeling errors, add new instances, delete instances)?

Yes.

### Will older versions of the dataset continue to be supported/hosted/maintained?

Yes

### If others want to extend/augment/build on/contribute to the dataset, is there a mechanism for them to do so?

Not yet, but if anyone want to work based on **Knowledge Pile**, please cite our paper "Query of CC: Unearthing Large Scale Domain-Specific Knowledge
from Public Corpora". [📄](https://arxiv.org/pdf/2401.14624.pdf)

### Any other comments?