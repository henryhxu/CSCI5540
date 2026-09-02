# CSCI5540 Machine Learning Systems, Fall 2026

## Administrivia

### Schedule
- Lectures: 
  * Mon 10:30am – 1:15pm, WMY 408
- Tutorials:
  * Mon 1:30pm - 2:15pm, WMY 408

### Team
| Member | Role | Office Hours |
| :---------------- | :--- | :----------- |
| [Xu, Hong](https://henryhxu.github.io/) | Prof | Tue 9:00-11:00 pm, SHB 914. **By appointment** |
| [Deng, Yangtao](TA_pics/yangtao.jpg) (ytdeng25@cse) | Head TA | Thu 9:30am - 11:30am, SHB 117 |
| [Jia, Chaobo](TA_pics/chaobo.jpg) (cbjia25@cse) | TA | Tue 3:00pm -5:00pm, SHB 117 |

**[NOTE]**: Due to the large class size, please do **not** email us individually. Ed should be used for all Q&A.

### Ed
The Ed page for this course is [here](https://edstem.org/au/join/y5we2K).
**All** communication about this course is done over Ed. This includes questions, discussions, announcements, as well as private messages. 

## Course outline

This graduate course will introduce you to the key concepts and the state-of-the-art in large-scale software systems for LLMs and agents, and encourage you to think about either building new tools or how to apply existing ones in various domains.

Since datacenters and cloud computing form the backbone of modern computing, we will start with an overview of the two. We will then take a deep dive into three key aspects of the landscape: systems for LLM, systems for agents, and the common infra. Our topics will include: basics on generative models and agentic AI from a systems perspective; systems for LLMs such as pre-training, inference; systems for agents such as post-training, sandbox; and common infra issues such as reliability, simulation; etc. We will cover topics primarily from top conferences that take a systems view to the relevant challenges.

Note that this course is NOT focused on ML/AI algorithms or methods. Instead, we will focus on how one can build software systems so that existing AI methods can be used in practice and new AI methods can emerge.

### Prerequisites
Students are expected to have good programming skills and must have taken at least one undergraduate-level systems-related course (from operating systems, databases, distributed systems, and networking). This is not formally enforced but without some background students may find this course quite challenging. Having an undergraduate ML/AI course may be helpful, but not required or necessary.

###  Textbook
This course has no textbooks. We will read recent papers from top venues to understand trends in scalable GenAI and agentic systems, and their applications.

## Tentative Schedule and Reading List

*This is an evolving list and subject to changes due to the breakneck pace of agentic and generative AI innovations.*

| Date | Readings | Presenter | Summary | Reviewer |
| :---- | :---- | :---- | :---- | :---- |
| **Sep 7** | **Introduction (Cloud, systems, and transformers)** | [Henry](Slides/083126-MChowdhury.pdf) |   |   |
|   | [Hints and Principles for Computer System Design](https://www.microsoft.com/en-us/research/wp-content/uploads/2019/09/Hints-and-Principles-v1-full.pdf) (Required) |   |   |   |
|   | [Machine Learning Fleet Efficiency: Analyzing and Optimizing Large-Scale Google TPU Systems with ML Productivity Goodput](https://arxiv.org/abs/2502.06982) |   |   |   |
|   | [The Datacenter as a Computer](https://web.eecs.umich.edu/~mosharaf/Readings/DC-Computer.pdf) (Chapters 1 and 2\) |   |   |   |
|   | [Heterogeneity at Hyperscale: Characterization and Scheduling of Large Production AI Clusters at Alibaba](https://www.usenix.org/conference/osdi26/presentation/li-suyi) |   |   |   |
| **Sep 14** | **No Class: Find Project Groups** |   |   |   |
|   | [How to Read a Paper](http://ccr.sigcomm.org/online/files/p83-keshavA.pdf) (Required) |   |   |   |
|   | [How to Give a Bad Talk](https://www.cs.ucf.edu/courses/cop4910/fall2004/BadTalk.pdf) (Required) |   |   |   |
|   | ***Systems for LLMs*** |   |   |   |
| **Sep 21** | **Pre-training: DP, TP, PP** |   |   |   |
|   | [Megatron-LM]() (Required) |   |   |   |
|   | [ZeRO]() (Required) |   |   |   |
|   | [FSDP]() |   |   |   |
|   | [GPipe]() |   |   |   |
| **Sep 28** | **Pre-training: EP, SP, compiler, memory** |   |   |   |
|   | [Alpa]() (Required) |   |   |   |
|   | [DeepSpeed-Ulysses]() (Required) |   |   |   |
|   | [BigMac](https://arxiv.org/pdf/2605.25451) (Required)|   |   |   |
|   | [Ring attention]() |   |   |   |
|   | [SimpleFSDP](); [torch.compile]() |   |   |   |
|   | [AutoSP](https://arxiv.org/abs/2604.27089) |   |   |   |


### Grading
|  | Weight 
| :---------------- | :--- | 
| Paper Presentation | 15% | 
| Paper Summary | 15% |
| Participation | 10% |
| Project Report | 40% | 
| Project Presentation | 20% | 
