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
|   | ***Chapter 1. Systems for LLMs*** |   |   |   |
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

## Policies
The format of this course is heavily borrowed from Prof. Mosharaf Chowdhury's [CSE 585](https://github.com/mosharaf/cse585/tree/f26) from U. Michigan with his consent.

### Groups
All activities of this course will be performed in **groups of 5 students**.

### Required Reading
Each lecture will have **two/three required readings that everyone must read**.  
There will be *two or more optional related reading(s)* that only the presenter(s) should be familiar with.
They are optional for the rest of the class.

### Student Lectures
The course will be conducted as a seminar. 
Only one group will present in each class.
Each group will be assigned *at least one lecture* over the course of the semester. 
Presentations should succinctly cover all required papers for that lecture.
The duration of the presentation should be **at most 40 minutes** with short clarifying questions and interruptions.
The rest of the lecture time will be dedicated toward discussion on the papers and the broader topic(s) covered by the papers.

In the presentation, you should:

* Provide necessary background and motivate the problem (not restricted by the paper itself).
* Present the high level idea, approach, and/or insight (using examples, whenever appropriate) in the required reading. 
* Discuss technical details so that one can understand key details without carefully reading.
* Explain the differences between related works.
* Identify strengths and weaknesses of the required reading and propose directions of future research.

The instructor team will review and suggest improvements for the presentations before each lecture.
Therefore, *the slides for a presentation must be emailed to the instructor team at least 24 hours prior to the corresponding class.*
To enable suggestions, use Google Slides and allow the instructor team give in-line comments.

### Lecture Summaries
Each group will also be assigned to **write summaries for at least one lecture**.
The summary assigned to a group will not be the reading they gave the lecture on.
The group will write a summary for all presented papers (required readings) for that lecture.

A paper summary must address the following questions in sufficient details (2-3 pages):

* What is the problem addressed in the lecture, and why is this problem important?
* What is the state of related works in this topic?
* What is the proposed solution, and what key insight guides their solution?
* What is one (or more) drawback or limitation of the proposal?
* What are potential directions for future research?

*The paper summary of a paper must be emailed to the instructor team within 24 hours after its presentation.* 
**Late summaries will not be counted.** 
You should use [this format](Summaries/Template.md) for writing your summary.
Use Google doc to enable in-line comments and suggestions.

*Allocate enough time for your reading, discuss as a group, write the summary carefully, and finally, include key observations from the class discussion.*

### Post-Presentation Panel Discussion 
To foster a deeper understanding of the papers and encourage critical thinking, each lecture will be followed by a panel discussion. 
This discussion will involve three distinct roles played by different student groups, simulating an interactive and dynamic scholarly exchange.

#### Roles and Responsibilities

1. **The Authors**
- Group Assignment: The group that presents the paper and the group that writes the summary will play the role of the paper's authors.
- Responsibility: As authors, you are expected to defend your paper against critiques, answer questions, and discuss how you might improve or extend your research in the future, akin to writing a rebuttal during the peer-review process.

2. **The Reviewers**
- Group Assignment: Each group will be assigned to one slot to play the role of reviewers for all presented papers (required readings) of that lecture.
- Responsibility: Reviewers critically assess the paper, posing challenging questions and highlighting potential weaknesses or areas for further investigation. 
Your goal is to engage in a constructive critique of the paper, simulating a peer review scenario.

3. **Rest of the Class**
- Responsibility: 
  - You are required to [submit]() **one insightful question** for each presented paper before each class.
  - During the panel discussions, feel free to actively **ask questions** and engage in the dialogue.

### Participation
Given the discussion-based nature of this course, participation is required both for your own understanding and to improve the overall quality of the course.
You are expected to attend **all** lectures (you may skip up to 2 lectures due to legitimate reasons), and more importantly, participate in class discussions.
There will be random events to gauge attendance.

A key part of participation will be in the form of discussion in Ed.
The group in charge of the summary should initiate the discussion and the rest should participate.
Not everyone has to add something every day, but it is expected that everyone has something to say over the semester.

### Project
You will have to complete substantive work on an instructor-approved problem and have original contribution.
Surveys are not permitted as projects; instead, each project must contain a survey of background and related work.

You must meet the following milestones (unless otherwise specified in future announcements) to ensure a high-quality project at the end of the semester:

* Form a group and [declare your group's membership and paper preferences]() by **September 14**.
After this date, we will form groups from the remaining students.
* Email a 2-page draft proposal (including references) by **September 30**. Remember to include the names and CUHK email addresses of the group members. 
* Each group must present mid-semester progress during the tutorial hours on **November 2**.
* Each group must turn in an 8-page final report and your source code via email **on or before 1:00PM EST on December 17.** The report must be submitted as a PDF file, with formatting similar to that of the papers you've read in the class. It should point to a git repository with all the code along with a README file with a step-by-step guide on how to compile and run the code. Code that cannot run will be treated as a non-submission without any debugging effort from the teaching team. Make sure your instructions are complete.

### GPU resources
* The dept has reserved at least 2 servers each with 8 3090 GPUs for this course. Enrolled students have been given access to them already.
* Usage example of the 3090 GPUs (slurm based; cse IP or vpn required)
```
ssh linux1-15
export SLURM_CONF=/opt1/slurm/gpu-slurm.conf
srun --account gpu --qos csci5540 -p csci5540 --gres=gpu:1 --pty /bin/bash
```
* The dept also has much more powerful GPUs shared by all students, and many individual faculty members (i.e. your advisor) have their own GPUs for which their students have highest priority using. More info can be found on the [internal website](https://i.cse.cuhk.edu.hk/technical/gpgpu-hpc-service/server-information/) (CSE IP required).

### Grading
|  | Weight 
| :---------------- | :--- | 
| Paper Presentation | 15% | 
| Paper Summary | 15% |
| Participation | 10% |
| Project Report | 40% | 
| Project Presentation | 20% | 
