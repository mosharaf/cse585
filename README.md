# CSE 585: Advanced Scalable Systems for Agentic AI (W'26)

## Administrivia
* Catalog Number: 29242
* Lectures/Discussion: 1005 DOW, MoWe: 10:30 AM - 12:00 PM
* Projects/Makeup: 1005 DOW, F 1:30 PM - 2:30 PM
* Counts as: Software Breadth and Depth (PhD); Technical Elective and 500-Level (MS/E)

### Team

| Member (uniqname) | Role | Office Hours |
| :---------------- | :--- | :----------- |
| [Mosharaf Chowdhury](http://www.mosharaf.com/) (mosharaf) | Faculty | 4156 LEIN. **By appointments only.**
| [Kevin Xue](https://kevinrsx.github.io/) (kaiwenx) | GSI | TBA.

### Communication
**ALL** communication regarding this course must be via [Ed](https://edstem.org/us/join/bPfM9H).
This includes questions, discussions, announcements, as well as private messages.

Presentation slides and paper summaries should be emailed to [cse585-staff@umich.edu](mailto:cse585-staff@umich.edu).

## Course Description
This iteration of CSE585 will introduce you to the key concepts and the state-of-the-art in practical, scalable, and fault-tolerant systems for Agentic and Generative AI and encourage you to think about either building new tools or how to apply the existing ones.

Since datacenters and cloud computing form the backbone of modern AI, we will start with an overview of the two.
We will then take a deep dive into systems for the Agentic and Generative AI landscape, focusing on different types of problems.
Our topics will include: basics on generative models and agentic AI from a systems perspective; systems for the AI lifecycle including pre-training, post-training, and inference serving; serving systems for text, multimodal, and agentic workloads; state management, system interfaces, and security for agents; and the operational realities of running AI at scale, including capacity and cost, reliability and fault tolerance, and power and energy.
We will cover topics primarily from top conferences that take a systems view to the relevant challenges.

Note that this course is **NOT focused on AI methods**.
Instead, we will *focus on how one can build systems* so that existing AI methods can be used in practice and new AI methods can emerge.

### Prerequisites
Students are expected to have good programming skills and must have taken *at least one* undergraduate-level systems-related course (from operating systems/EECS482, databases/EECS484, distributed systems/EECS491, and networking/EECS489).
Having an undergraduate ML/AI course may be helpful, but not required or necessary. 

### Textbook
This course has no textbooks.
We will read recent papers from top venues to understand trends in scalable GenAI and agentic systems, and their applications.

## Tentative Schedule and Reading List

*This is an evolving list and subject to changes due to the breakneck pace of agentic and generative AI innovations.*


| Date | Readings | Presenter | Summary | Reviewer |
| :---- | :---- | :---- | :---- | :---- |
| **Aug 31** | **Introduction** | [Mosharaf](Slides/083126-MChowdhury.pdf) |   |   |
|   | [Hints and Principles for Computer System Design](https://www.microsoft.com/en-us/research/wp-content/uploads/2019/09/Hints-and-Principles-v1-full.pdf) (Required) |   |   |   |
|   | [Machine Learning Fleet Efficiency: Analyzing and Optimizing Large-Scale Google TPU Systems with ML Productivity Goodput](https://arxiv.org/abs/2502.06982) (Required) |   |   |   |
|   | [The Datacenter as a Computer](https://web.eecs.umich.edu/~mosharaf/Readings/DC-Computer.pdf) (Chapters 1 and 2\) |   |   |   |
|   | [Heterogeneity at Hyperscale: Characterization and Scheduling of Large Production AI Clusters at Alibaba](https://www.usenix.org/conference/osdi26/presentation/li-suyi) |   |   |   |
| **Sep 2** | **No Class: Find Project Groups** |   |   |   |
|   | [How to Read a Paper](http://ccr.sigcomm.org/online/files/p83-keshavA.pdf) (Required) |   |   |   |
|   | [How to Give a Bad Talk](https://people.eecs.berkeley.edu/~pattrsn/talks/BadTalk.pdf) (Required) |   |   |   |
| **Sep 7** | **Labor Day** |   |   |   |
| **Sep 9** | **Systems for AI (Agents) Basics** | Kevin |   |   |
|   | [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) (Required) |   |   |   |
|  | [Dive into Claude Code: The Design Space of Today's and Future AI Agent Systems](https://arxiv.org/abs/2604.14228) (Required) |  |  |  |
|  | [Anthropic, When AI builds itself](https://www.anthropic.com/institute/recursive-self-improvement) |  |  |  |
|  | [Kimi K3: Open Frontier Intelligence](https://arxiv.org/abs/2607.24653) |  |  |  |
| **Sep 14** | **Distributed Training Basics** | Kevin |   |   |
|   | [Efficient Large-Scale Language Model Training on GPU Clusters Using Megatron-LM](https://dl.acm.org/doi/10.1145/3458817.3476209) (Required) |   |   |   |
|   | [The Ultra-Scale Playbook: Training LLMs on GPU Clusters](https://huggingface.co/spaces/nanotron/ultrascale-playbook) |   |   |   |
| **Sep 16**  | **Pre-Training at Scale** |  |  |  |
|   | [Tessera: A Holistic Pipeline Parallelism Framework for Trillion-Parameter Heterogeneous MoE Training](https://www.usenix.org/conference/osdi26/presentation/hu-weifang) (Required) |   |   |   |
|  | [Scaling Llama 3 Training with Efficient Parallelism Strategies](https://dl.acm.org/doi/10.1145/3695053.3731410) (Required) |  |  |  |
|  | [WLB-LLM: Workload-Balanced 4D Parallelism for Large Language Model Training](https://www.usenix.org/conference/osdi25/presentation/wang-zheng)  |   |   |   |
| **Sep 21** | **Post-Training** |  |  |  |
|  | [HybridFlow: A Flexible and Efficient RLHF Framework](https://dl.acm.org/doi/10.1145/3689031.3696075) (Required) |   |   |   |
|  | [RollArt: Disaggregated Multi-Task Agentic RL Training at Scale](https://www.usenix.org/conference/osdi26/presentation/gao) (Required) |  |  |  |
|   | [AReaL: A Large-Scale Asynchronous Reinforcement Learning System for Language Reasoning](https://openreview.net/forum?id=X9diEuva9R) |   |   |   |
|  | [Weave: Efficient Co-Scheduling for Disaggregated RL Post-Training](https://www.usenix.org/conference/osdi26/presentation/wu-tianyuan) |  |  |  |
| **Sep 23** | **No Class: Work on Project Proposals** |   |   |   |
|   | [Writing Reviews for Systems Conferences](https://people.inf.ethz.ch/troscoe/pubs/review-writing.pdf) (Required) |   |   |   |
|   | [Worse is Better](https://en.wikipedia.org/wiki/Worse_is_better) (Required) |   |   |   |
| **Sep 28** | **Inference Basics** | Kevin |   |   |
|   | [Efficient Memory Management for Large Language Model Serving with PagedAttention](https://dl.acm.org/doi/10.1145/3600006.3613165) (Required) |   |   |   |
|  | [DistServe: Disaggregating Prefill and Decoding for Goodput-Optimized Large Language Model Serving](https://dl.acm.org/doi/10.5555/3691938.3691949) (Required) |  |  |  |
|  | [Orca: A Distributed Serving System for Transformer-Based Generative Models](https://www.usenix.org/conference/osdi22/presentation/yu) |  |  |  |
|   | [On Evaluating Performance of LLM Inference Serving Systems](https://openreview.net/forum?id=VG7F3Auy9T) |   |   |   |
| **Sep 30**  | **Inference: Disaggregation and Fusion** |  |  |  |
|  | [MPK: A Compiler and Runtime for Mega-Kernelizing Tensor Programs](https://www.usenix.org/conference/osdi26/presentation/cheng) (Required) |  |  |  |
|  | [Mooncake: Trading More Storage for Less Computation — A KVCache-centric Architecture for Serving LLM Chatbot](https://www.usenix.org/conference/fast25/presentation/qin) (Required) |  |  |  |
|  | [Not All Prefills Are Equal: PPD Disaggregation for Multi-turn LLM Serving](https://openreview.net/pdf?id=RW23qIUb5f) |   |   |   |
|  | [LoongServe: Efficiently Serving Long-Context Large Language Models with Elastic Sequence Parallelism](https://dl.acm.org/doi/10.1145/3694715.3695948) |  |  |  |
| **Oct 5** | **Inference: Beyond Text** |  |  |  |
|   | [Cornfigurator: Automated Planning for Any-to-Any Multimodal Model Serving](https://arxiv.org/abs/2512.14098) (Required) |   |   |   |
|  | [DiFlow: A System for Micro-Serving Text-to-Image Diffusion Workflows](https://arxiv.org/abs/2604.08123) (Required) |  |  |  |
|   | [TetriServe: Efficiently Serving Mixed DiT Workloads](https://dl.acm.org/doi/10.1145/3779212.3790233) |   |   |   |
| **Oct 7**  | **Agents as a New System Workload** |  |  |  |
|  | [The Cost of Dynamic Reasoning: Demystifying AI Agents and Test-Time Scaling from an AI Infrastructure Perspective](https://ieeexplore.ieee.org/document/11408569/) (Required) |   |   |   |
|   | [Towards Understanding, Analyzing, and Optimizing Agentic AI Execution: A CPU-Centric Perspective](https://arxiv.org/abs/2511.00739) (Required) |   |   |   |
|   | [What Limits Agentic Systems Efficiency?](https://openreview.net/pdf?id=HcGK3IRZn0) |   |   |   |
| **Oct 12** | **Serving Systems for Agents** |   |   |   |
|   | [Pie: A Programmable Serving System for Emerging LLM Applications](https://dl.acm.org/doi/10.1145/3731569.3764814) (Required) |   |   |   |
|   | [Murakkab: Resource-Efficient Agentic Workflow Orchestration in Cloud Platforms](https://www.usenix.org/conference/osdi26/presentation/chaudhry) (Required) |   |   |   |
|   | [Towards End-to-End Optimization of LLM-based Applications with Ayo](https://dl.acm.org/doi/10.1145/3676641.3716278) |   |   |   |
| **Oct 14** | **Agentic State Management** |   |   |   |
|  | [Continuum: Efficient and Robust Multi-Turn LLM Agent Scheduling with KV Cache Time-to-Live](https://openreview.net/attachment?id=sVzK0LC9pn&name=pdf) (Required) |  |  |  |
|  | [Strata: Hierarchical Context Caching for Long-Context LLM Serving](https://www.usenix.org/conference/osdi26/presentation/xie-zhiqiang) (Required) |  |  |  |
|   | [Conveyor: Efficient Tool-aware LLM Serving with Tool Partial Execution](https://arxiv.org/abs/2406.00059) |   |   |   |
|  | [Agentic Plan Caching: Test-Time Memory for Fast and Cost-Efficient LLM Agents](https://openreview.net/pdf?id=n4V3MSqK77) |  |  |  |
| **Oct 19** | **Fall Study Break** |  |  |  |
| **Oct 21** | **No Lecture: Work on Presentations** |  |  |  |
| **Oct 26** | **Test-Time Compute as Resource Allocation** |  |  |  |
|   | [Breaking the Reward Barrier: Accelerating Tree-of-Thought Reasoning via Speculative Exploration](https://www.usenix.org/conference/osdi26/presentation/zhong) (Required) |  |  |  |
|   | [Speculative Actions: A Lossless Framework for Faster Agentic Systems](https://openreview.net/pdf?id=P0GOk5wslg) (Required) |  |  |  |
|   | [Act While Thinking: Accelerating LLM Agents via Pattern-Aware Speculative Tool Execution](https://www.microsoft.com/en-us/research/publication/act-while-thinking-accelerating-llm-agents-via-pattern-aware-speculative-tool-execution/) |  |  |  |
| **Oct 28** | **System Interfaces for Agents** |   |   |   |
|   | [From Imperative to Declarative: Towards LLM-friendly OS Interfaces for Boosted Computer-Use Agents](https://dl.acm.org/doi/10.1145/3767295.3803576) (Required) |   |   |   |
|  | [Agent JIT Compilation for Latency-Optimizing Web Agent Planning and Scheduling](https://openreview.net/pdf?id=7NiATKcx1B) (Required) |  |  |  |
|  | [Branch-and-Browse: Efficient and Controllable Web Exploration with Tree-Structured Reasoning and Action Memory](https://aclanthology.org/2026.acl-long.838.pdf) |  |  |  |
|   | [AgentCgroup: Understanding and Controlling OS Resources of AI Agents](https://arxiv.org/abs/2602.09345) |   |   |   |
| **Nov 2** | **Mid-Semester Presentations** |   |   |   |
| **Nov 4** | **Mid-Semester Presentations** |   |   |   |
| **Nov 9** | **Agents in the Physical World** |   |   |   |
|   | [ASPIRE: Agentic `/Skills` Discovery for Robotics](https://research.nvidia.com/labs/gear/aspire/assets/Aspire.pdf?v=20260630d) (Required) |   |   |   |
|   | [TimelyLLM: Time-sensitive LLM Serving System for Physical-I/O Limited Agents](https://dl.acm.org/doi/10.1145/3745756.3809203) (Required) |   |   |   |
|   | [VLA-Perf: Demystifying VLA Inference Performance](https://arxiv.org/abs/2602.18397) |   |   |   |
| **Nov 11** | **Multi-Agent Execution** |   |   |   |
|   | [Towards a Science of Scaling Agent Systems](https://arxiv.org/abs/2512.08296) (Required) |   |   |   |
|   | [FlashAgents: Accelerating Multi-Agent LLM Systems via Streaming Prefill Overlap](https://openreview.net/pdf?id=m14PPUfgEc) (Required) |   |   |   |
|   | [Orla: A Library for Serving LLM-Based Multi-Agent Systems](https://dl.acm.org/doi/full/10.1145/3786335.3813227) |   |   |   |
| **Nov 16** | **Agent Security** |   |   |   |
|   | [FragFuse: Bypassing Access Control of Large Language Model Agents via Memory-Based Query Fragmentation and Fusion](https://arxiv.org/abs/2606.15609) (Required) |   |   |   |
|   | [Towards Automating Data Access Permissions in AI Agents](https://www.franziroesner.com/pdf/wu-agentperms-sp26.pdf) (Required) |   |   |   |
|   | [ParaCell: Paravirtualized Secure Containers with Lightweight Intra-Container Isolation](https://arxiv.org/abs/2605.20906) |   |   |   |
| **Nov 18** | **Operations: Capacity and Cost** |  |  |  |
|  | [Rearchitecting Datacenter Lifecycle for AI: A TCO-Driven Framework](https://arxiv.org/abs/2509.26534) (Required) |  |  |  |
|  | [Quota Marketplace: Dynamic Pricing for Efficient Allocation of ML Training Resources](https://www.usenix.org/conference/osdi26/presentation/sivan) (Required) |  |  |  |
|  | [Prism: Cost-Efficient Multi-LLM Serving via GPU Memory Ballooning](https://www.usenix.org/conference/osdi26/presentation/yu-shan) |  |  |  |
| **Nov 23** | **Operations: Reliability and Fault Tolerance** |  |  |  |
|  | [SDCs in the Wild: Characterizing and Diagnosing SDC-Defective GPUs in Production LLM Training](https://www.usenix.org/conference/osdi26/presentation/zheng) (Required) |  |  |  |
|  | [LogAct: Enabling Agentic Reliability via Shared Logs](https://arxiv.org/abs/2604.07988) (Required) |  |  |  |
|  | [RobustRL: Role-Based Fault Tolerance System for RL Post-Training](https://www.usenix.org/conference/osdi26/presentation/chen-zhenqian) |  |  |  |
|  | [LUMEN: Coordinated Failure Recovery for Distributed LLM Serving](https://arxiv.org/abs/2606.17787) |  |  |  |
| **Nov 25** | **Thanksgiving** |   |   |   |
| **Nov 30** | **Operations: Power and Energy** |   |   |   |
|   | [KAIROS: Stateful, Context-Aware, Power-Efficient Agentic Inference Serving](https://arxiv.org/abs/2604.16682) (Required) |   |   |   |
|  | [Provisioning to Runtime Optimization of a 100 MW-Scale AI Cluster](https://arxiv.org/abs/2605.24461) (Required) |  |  |  |
|   | [Where Do the Joules Go? Diagnosing Inference Energy Consumption](https://arxiv.org/abs/2601.22076) |   |   |   |
|  | [Energy Calculus: A Compositional Algebra of Energy in Computational Systems](https://arxiv.org/abs/2607.11087) |  |  |  |
| **Dec 2** | **Wrap Up** | Mosharaf |   |   |
|   | [Barbarians at the Gate: How AI is Upending Systems Research](https://arxiv.org/abs/2510.06189) (Required) |   |   |   |
|   | [We Need a New Ethics for a World of AI Agents](https://arxiv.org/abs/2509.10289) (Required) |   |   |   |
|   | [ECO: An AI-Driven Code Efficiency Optimizer for Warehouse Scale Computers](https://www.usenix.org/conference/osdi26/presentation/lin-hannah) |   |   |   |
| **Dec 7** | **No Lecture: Work on Posters** |   |   |   |
|   | [Creating an Effective Poster](https://designcenter.uiowa.edu/creating-effective-posters) (Required) |   |   |   |
|   | [How to Write a Great Research Paper](https://www.microsoft.com/en-us/research/academic-program/write-great-research-paper/) (Required) |   |   |   |
| **Dec 9** | **Final Poster Presentations (TBD)** |   |   |   |

## Policies

### Honor Code
[The Engineering Honor Code](https://ecas.engin.umich.edu/honor-council/honor-code/) applies to all activities related to this course.

### Groups
All activities of this course will be performed in **groups of 4 students**.

### Required Reading
Each lecture will have **two required readings that everyone must read**.  
There will be *one or more optional related reading(s)* that only the presenter(s) should be familiar with.
They are optional for the rest of the class.

### Student Lectures
The course will be conducted as a seminar. 
Only one group will present in each class.
Each group will be assigned *at least one lecture* over the course of the semester. 
Presentations should succinctly cover all required papers for that lecture.
The duration of the presentation should be **at most 30 minutes** with short clarifying questions and interruptions.
The rest of the lecture time will be dedicated toward discussion on the papers and the broader topic(s) covered by the papers.

In the presentation, you should:

* Provide necessary background and motivate the problem.
* Present the high level idea, approach, and/or insight (using examples, whenever appropriate) in the required reading. 
* Discuss technical details so that one can understand key details without carefully reading.
* Explain the differences between related works.
* Identify strengths and weaknesses of the required reading and propose directions of future research.

*The slides for a presentation must be emailed to the instructor team at least 24 hours prior to the corresponding class.* 
Use Google slides to enable in-line comments and suggestions.

### Lecture Summaries
Each group will also be assigned to **write summaries for at least one lectures**.
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
  - You are required to [submit](TBD) **one insightful question** for each presented paper before each class. 
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

* Form a group and [declare your group's membership and paper preferences](TBA) by **September 14**. After this date, we will form groups from the remaining students.
* Email a 2-page draft proposal (including references) by **September 30**. Remember to include the names and Michigan email addresses of the group members. 
* Each group must present mid-semester progress during class hours on **November 2 and November 4**.
* Each group must turn in an 8-page final report and your code via email **on or before 1:00PM EST on December 17.** The report must be submitted as a PDF file, with formatting similar to that of the papers you've read in the class. It should point to a git repository with all the code along with a README file with a step-by-step guide on how to compile and run the code.
* You can find how to access GPU resources [here](./Resources/Starting%20with%20Cloudlab).

## Tentative Grading
|                         | Weight | 
| ------------------------| ------:| 
| Paper Presentation      | 20%    | 
| Paper Summary           | 10%    | 
| Participation           | 10%    | 
| Project Report          | 40%    | 
| Project Presentations   | 20%    | 
