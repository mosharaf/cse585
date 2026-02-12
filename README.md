# CSE 585: Advanced Scalable Systems for Agentic AI (W'26)

## Administrivia
* Catalog Number: 35120
* Lectures/Discussion: 1200 EECS, TTh: 10:30 AM – 12:00 PM
* Projects/Makeup: 1014 DOW, F 1:30 PM – 2:30 PM
* Counts as: Software Breadth and Depth (PhD); Technical Elective and 500-Level (MS/E)

### Team

| Member (uniqname) | Role | Office Hours |
| :---------------- | :--- | :----------- |
| [Mosharaf Chowdhury](http://www.mosharaf.com/) (mosharaf) | Faculty | 4156 LEIN. **By appointments only.**
| [Shiqi He](https://tctower.github.io/) (shiqihe) | GSI | 1637 BBB. Wed 4:00 PM – 6:00 PM.

### Communication
**ALL** communication regarding this course must be via [Ed](https://edstem.org/us/join/99Gwqq).
This includes questions, discussions, announcements, as well as private messages.

Presentation slides and paper summaries should be emailed to [cse585-staff@umich.edu](mailto:cse585-staff@umich.edu).

## Course Description
This iteration of CSE585 will introduce you to the key concepts and the state-of-the-art in practical, scalable, and fault-tolerant systems for Agentic and Generative AI and encourage you to think about either building new tools or how to apply the existing ones.

Since datacenters and cloud computing form the backbone of modern computing, we will start with an overview of the two. 
We will then take a deep dive into systems for the Agentic and Generative AI landscape, focusing on different types of problems. 
Our topics will include: basics on generative models and agentic AI from a systems perspective; systems for AI lifecycle including pre-training, post-training, and inference serving systems; systems for agentic AI; etc. 
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
| Jan 8 | **No Lecture: Find Project Groups** |  |  |  |
|  | [How to Read a Paper](http://svr-sk818-web.cl.cam.ac.uk/keshav/papers/07/paper-reading.pdf) (Required) |  |  |  |
|  | [How to Give a Bad Talk](http://www.cs.berkeley.edu/~pattrsn/talks/BadTalk.pdf) (Required) |  |  |  |
| Jan 13 | **Introduction** | [Mosharaf](Slides/011326-MChowdhury.pdf) |  |  |
|  | [Hints and Principles for Computer System Design](https://arxiv.org/abs/2011.02455) (Required) |  |  |  |
|  | [The Datacenter as a Computer](https://link.springer.com/book/10.1007/978-3-031-01761-2) (Chapters 1 and 2\) |  |  |  |
|  | [Machine Learning Fleet Efficiency: Analyzing and Optimizing Large-Scale Google TPU Systems with ML Productivity Goodput](https://arxiv.org/abs/2502.06982) (Required) |  |  |  |
| Jan 15 | **Systems for AI Basics** | [Shiqi](Slides/011526-shiqihe.pdf) |  |  |
|  | [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) (Required) |  |  |  |
|  | [Deep Dive into LLMs like ChatGPT](https://www.youtube.com/watch?v=7xTGNNLPyMI) |  |  |  |
|  | [OpenHands: An Open Platform for AI Software Developers as Generalist Agents](https://arxiv.org/abs/2407.16741) (Required) |  |  |  |
| Jan  20 | **Distributed Training Basics** | [Shiqi](Slides/012026-shiqihe.pdf) |  |  |
|  | [Efficient Large-Scale Language Model Training on GPU Clusters Using Megatron-LM](https://dl.acm.org/doi/10.1145/3458817.3476209) (Required) |  |  |  |
| Jan 22 | **No Lecture: Work on Project Proposals** |  |  |  |
|  | [Writing Reviews for Systems Conferences](http://people.inf.ethz.ch/troscoe/pubs/review-writing.pdf) (Required) |  |  |  |
|  | [Worse is Better](https://en.wikipedia.org/wiki/Worse_is_better) (Required) |  |  |  |
|  | **Pre-Training** |  |  |  |
| Jan 27 | [WLB-LLM: Workload-Balanced 4D Parallelism for Large Language Model Training](https://www.usenix.org/conference/osdi25/presentation/wang-zheng) (Required) |  [Rohan, Archit, Divya, Maaz](Slides/012726-Rohan-Archit-Divya-Maaz.pdf) |  [Joshua, Rishith, Olaf, Jimmy](Summaries/012726-Joshua-Rishith-Olaf-Jimmy.pdf) |  Anika, Joshua, Namita, Nandana |
|  | [Zero Bubble (Almost) Pipeline Parallelism](https://openreview.net/forum?id=tuzTN0eIO5) (Required) |  |  |  |
| Jan 29 | [Alpa: Automating Inter- and Intra-Operator Parallelism for Distributed Deep Learning](https://www.usenix.org/conference/osdi22/presentation/zheng-lianmin) (Required) |  [Adam, Qilong, Yung-Hao, Zhe](Slides/012926-Adam-Qilong-Yung-Hao-Zhe.pdf) | [Yiqun, Yicheng, Yihang, Xiangchen](Summaries/012926-Yiqun-Yicheng-Yihang-Xiangchen.pdf) | Evan, Frank, Madeleine, Alan |
|  | [PartIR: Composing SPMD Partitioning Strategies for Machine Learning](https://dl.acm.org/doi/10.1145/3669940.3707284) |  |  |  |
|  | [FSMoE: A Flexible and Scalable Training System for Sparse Mixture-of-Experts Models](https://dl.acm.org/doi/10.1145/3669940.3707272) (Required) |  |  |  |
|  | [FlexMoE: Scaling Large-scale Sparse Pre-trained Model Training via Dynamic Device Placement](https://dl.acm.org/doi/abs/10.1145/3588964) |  |  |  |
| Feb 3 | [TrainVerify: Equivalence-Based Verification for Distributed LLM Training](https://dl.acm.org/doi/10.1145/3731569.3764850) (Required) | [Matthew, Madison, Minkyu, Kevin](Slides/020326-Matthew-Madison-Minkyu-Kevin.pdf) | [Ajay, Allison, Jamal, Tejas](Summaries/020326-Ajay-Allison-Jamal-Tejas.pdf) | Shivam, Aman, Leonard, Dimash |
|  | [SuperBench: Improving Cloud AI Infrastructure Reliability with Proactive Validation](https://www.usenix.org/conference/atc24/presentation/xiong) |  |  |  |
|  | [Oobleck: Resilient Distributed Training of Large Models Using Pipeline Templates](https://dl.acm.org/doi/10.1145/3600006.3613152) (Required) |  |  |  |
|  | **Post-Training** |  |  |  |
| Feb 5 | [HybridFlow: A Flexible and Efficient RLHF Framework](https://dl.acm.org/doi/10.1145/3689031.3696075) | [Joshua, Rishith, Olaf, Jimmy](Slides/020526-Joshua-Rishith-Olaf-Jimmy.pdf) | [Rohan, Archit, Divya, Maaz](Summaries/020526-Rohan-Archit-Divya-Maaz.pdf) | Yiqun, Yicheng, Yihang, Xiangchen |
|  | [AReaL: A Large-Scale Asynchronous Reinforcement Learning System for Language Reasoning](https://arxiv.org/abs/2505.24298) (Required) |  |  |  |
|  | [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948) (Required) |  |  |  |
|  | **Inference** |  |  |  |
| Feb 10 | **Inference Basics** | [Shiqi](Slides/021026-shiqihe.pdf) |  |  |
|  | [Orca: A Distributed Serving System for Transformer-Based Generative Models](https://www.usenix.org/conference/osdi22/presentation/yu) (Required) |  |  |  |
|  | [Efficient Memory Management for Large Language Model Serving with PagedAttention](https://dl.acm.org/doi/10.1145/3600006.3613165) (Required) |  |  |  |
|  | [On Evaluating Performance of LLM Inference Serving Systems](https://arxiv.org/abs/2507.09019) |  |  |  |
| Feb 12 | [DistServe: Disaggregating Prefill and Decoding for Goodput-Optimized Large Language Model Serving](https://www.usenix.org/conference/osdi24/presentation/zhong-yinmin) (Required) | [Anika, Joshua, Namita, Nandana](Slides/021226-Anika-Joshua-Namita-Nandana.pdf) | Jingjing, Yile, Zhengqing, Barry | Shruti, Srikrishnan, Nikhil, Pranav |
|  | [Taming Throughput-Latency Tradeoff in LLM Inference with Sarathi-Serve](https://www.usenix.org/conference/osdi24/presentation/agrawal) (Required) |  |  |  |
| Feb 17 | **No Lecture: Work on Projects** |  |  |  |
| Feb 19 | [NanoFlow: Towards Optimal Large Language Model Serving Throughput](https://www.usenix.org/conference/osdi25/presentation/zhu-kan) (Required) | Evan, Frank, Madeleine, Alan | Matthew, Madison, Minkyu, Kevin | Tea, Nidhil, Dillan |
|  | [Mooncake: Trading More Storage for Less Computation — A KVCache-centric Architecture for Serving LLM Chatbot](https://www.usenix.org/conference/fast25/presentation/qin) (Required) |  |  |  |
| Feb 24 | [LoongServe: Efficiently Serving Long-Context Large Language Models with Elastic Sequence Parallelism](https://dl.acm.org/doi/10.1145/3694715.3695948) (Required) | Shivam, Aman, Leonard, Dimash | Kidus, Blake, Torence, Ethan | Ajay, Allison, Jamal, Tejas |
|  | [MegaScale-Infer: Serving Mixture-of-Experts at Scale with Disaggregated Expert Parallelism](https://arxiv.org/abs/2504.02263) (Required) |  |  |  |
| Feb 26 | [Cornserve: Efficiently Serving Any-to-Any Multimodal Models](https://arxiv.org/abs/2512.14098) (Required) | Jingjing, Yile, Zhengqing, Barry | Anika, Joshua, Namita, Nandana | Vansh, Pranav, Anshul, Shrey |
|  | [TetriServe: Efficient DiT Serving for Heterogeneous Image Generation](https://arxiv.org/abs/2510.01565) |  |  |  |
|  | [Approximate Caching for Efficiently Serving Diffusion Models](https://www.usenix.org/conference/nsdi24/presentation/agarwal-shubham) (Required) |  |  |  |
| Mar 10 | **No Lecture: Work on Presentations** |  |  |  |
| Mar 12 | [Fast-dLLM: Training-free Acceleration of Diffusion LLM by Enabling KV Cache and Parallel Decoding](https://arxiv.org/abs/2505.22618) (Required) | Kidus, Blake, Torence, Ethan | Shruti, Srikrishnan, Nikhil, Pranav | Adam, Qilong, Yung-Hao, Zhe |
|  | [ScaleFusion: Scalable Inference of Spatial-Temporal Diffusion Transformers for High-Resolution Long Video Generation](https://openreview.net/forum?id=anZWBeWnWh) (Required) |  |  |  |
|  | [Sparse VideoGen: Accelerating Video Diffusion Transformers with Spatial-Temporal Sparsity](https://arxiv.org/abs/2502.01776) |  |  |  |
| Mar 17 | **Mid-Semester Presentations** |  |  |  |
| Mar 19 | **Mid-Semester Presentations** |  |  |  |
|  | **Agentic AI Systems** |  |  |  |
| Mar 24 | [Parrot: Efficient Serving of LLM-based Applications with Semantic Variable](https://www.usenix.org/conference/osdi24/presentation/lin-chaofan) (Required) | Ajay, Allison, Jamal, Tejas | Tea, Nidhil, Dillan | Joshua, Rishith, Olaf, Jimmy |
|  | [Pie: A Programmable Serving System for Emerging LLM Applications](https://dl.acm.org/doi/abs/10.1145/3731569.3764814) (Required) |  |  |  |
|  | [Murakkab: Resource-Efficient Agentic Workflow Orchestration in Cloud Platforms](https://arxiv.org/abs/2508.18298)  |  |  |  |
| Mar 26 | [Towards End-to-End Optimization of LLM-based Applications with Ayo](https://dl.acm.org/doi/10.1145/3676641.3716278) (Required) | Yiqun, Yicheng, Yihang, Xiangchen | Shivam, Aman, Leonard, Dimash | Matthew, Madison, Minkyu, Kevin |
|  | [AVA: Towards Agentic Video Analytics with Vision Language Models](https://arxiv.org/abs/2505.00254) (Required) |  |  |  |
| Mar 31 | [METIS: Fast Quality-Aware RAG Systems with Configuration Adaptation](https://arxiv.org/abs/2412.10543) (Required) | Tea, Nidhil, Dillan | Evan, Frank, Madeleine, Alan | Jingjing, Yile, Zhengqing, Barry |
|  | [HedraRAG: Co-Optimizing Generation and Retrieval for Heterogeneous RAG Workflows](https://dl.acm.org/doi/10.1145/3731569.3764806) (Required) |  |  |  |
|  | [Fast Vector Query Processing for Large Datasets Beyond GPU Memory with Reordered Pipelining](https://www.usenix.org/conference/nsdi24/presentation/zhang-zili-pipelining) |  |  |  |
|  | **Hardware / Infrastructure** |  |  |  |
| Apr 2 | [WaferLLM: Large Language Model Inference at Wafer Scale](https://www.usenix.org/conference/osdi25/presentation/he) (Required) | Vansh, Pranav, Anshul, Shrey | Marie, Emily, Haripreeth, Pritesh | Kidus, Blake, Torence, Ethan |
|  | [Rearchitecting Datacenter Lifecycle for AI: A TCO-Driven Framework](https://arxiv.org/abs/2509.26534) (Required) |  |  |  |
|  | [Insights into DeepSeek-V3: Scaling Challenges and Reflections on Hardware for AI Architectures](https://dl.acm.org/doi/10.1145/3695053.3731412) |  |  |  |
|  | **Power and Energy Management** |  |  |  |
| Apr 7 | [Reducing Energy Bloat in Large Model Training](https://dl.acm.org/doi/10.1145/3694715.3695970)  |  Marie, Emily, Haripreeth, Pritesh | Vansh, Pranav, Anshul, Shrey | Rohan, Archit, Divya, Maaz |
|  | [Kareus: Joint Reduction of Dynamic and Static Energy in Large Model Training](https://arxiv.org/abs/2601.17654) (Required) |  |  |  |
|  | [TAPAS: Thermal- and Power-Aware Scheduling for LLM Inference in Cloud Platforms](https://dl.acm.org/doi/10.1145/3676641.3716025) (Required) |  |  |  |
| Apr 9 | [Power Stabilization for AI Training Datacenters](https://arxiv.org/abs/2508.14318) (Required) | Shruti, Srikrishnan, Nikhil, Pranav | Adam, Qilong, Yung-Hao, Zhe | Marie, Emily, Haripreeth, Pritesh |
|  | [AI Training Load Fluctuations at Gigawatt-scale – Risk of Power Grid Blackout?](https://semianalysis.com/2025/06/25/ai-training-load-fluctuations-at-gigawatt-scale-risk-of-power-grid-blackout) (Required) |  |  |  |
|  | **Wrap Up** |  |  |  |
| Apr 14 | [On the Dangers of Stochastic Parrots: Can Language Models be too Big?🦜](https://dl.acm.org/doi/abs/10.1145/3442188.3445922) (Required) | Mosharaf |  |  |
|  | [We Need a New Ethics for a World of AI Agents](https://www.nature.com/articles/d41586-025-02454-5) (Required) |  |  |  |
| Apr 16 | **No Lecture: Work on Posters** |  |  |  |
|  | [How to Write a Great Research Paper](https://www.microsoft.com/en-us/research/academic-program/write-great-research-paper/) (Required) |  |  |  |
| Apr 21 | **Final Poster Presentations** **(TBA)** | [Template](http://Resources/poster.pptx) |  |  |


## Policies

### Honor Code
[The Engineering Honor Code](https://ecas.engin.umich.edu/honor-council/honor-code/) applies to all activities related to this course.

### Groups
All activities of this course will be performed in **groups of 4 students**.

### Required Reading
Each lecture will have **two required reading that everyone must read**.  
There will be *one or more optional related reading(s)* that only the presenter(s) should be familiar with.
They are optional for the rest of the class.

### Student Lectures
The course will be conducted as a seminar. 
Only one group will present in each class.
Each group will be assigned *at least one lecture* over the course of the semester. 
Presentations should succinctly cover all required papers for that lecture.
The duration of the presentation should be **at most 35 minutes** with short clarifying questions and interruptions.
The rest of the lecture time will be dedicated toward discussion on the papers and the broader topic(s) covered by the papers.

In the presentation, you should:

* Provide necessary background and motivate the problem.
* Present the high level idea, approach, and/or insight (using examples, whenever appropriate) in the required reading as well as the additional reading. 
* Discuss technical details so that one can understand key details without carefully reading.
* Explain the differences between related works.
* Identify strengths and weaknesses of the required reading and propose directions of future research.

*The slides for a presentation must be emailed to the instructor team at least 24 hours prior to the corresponding class.* 
Use Google slides to enable in-line comments and suggestions.

### Lecture Summaries
Each group will also be assigned to **write summaries for at least one lectures**.
The summary assigned to a group will not be the reading they gave the lecture on.
The group will write a summary for all presented papers (required readings) for that lecture.

A paper summary must address the following four questions in sufficient details (2-3 pages):

* What is the problem addressed in the lecture, and why is this problem important?
* What is the state of related works in this topic?
* What is the proposed solution, and what key insight guides their solution?
* What is one (or more) drawback or limitation of the proposal?
* What are potential directions for future research?

*The paper summary of a paper must be emailed to the instructor team within 24 hours after its presentation.* 
**Late reviews will not be counted.** 
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
  - You are required to [submit](https://docs.google.com/forms/d/e/1FAIpQLSf2Rzk2qcG3e5YsUFY9BmYTS2Vwy2w6Rj2XQfcHYCDwOaV8rw/viewform?usp=header) **one insightful question** for each presented paper before each class. 
  - During the panel discussions, feel free to actively **ask questions** and engage in the dialogue. 

### Participation
Given the discussion-based nature of this course, participation is required both for your own understanding and to improve the overall quality of the course.
You are expected to attend **all** lectures (you may skip up to 2 lectures due to legitimate reasons), and more importantly, participate in class discussions.
There will be random events to gauge attendance.

A key part of participation will be in the form of discussion in Ed.
The group in charge of the summary should initiate the discussion and the rest should participate.
Not everyone must have add something every day, but it is expected that everyone has something to say over the semester.

### Project
You will have to complete substantive work an instructor-approved problem and have original contribution.
Surveys are not permitted as projects; instead, each project must contain a survey of background and related work.

You must meet the following milestones (unless otherwise specified in future announcements) to ensure a high-quality project at the end of the semester:

* Form a group and [declare your group's membership and paper preferences](https://docs.google.com/forms/d/e/1FAIpQLSe46GejPTulNCZO9q7CRaAJsIQJT0ZesRKlNC2zNIAKWmQxSA/viewform?usp=header) by **January 23**. After this date, we will form groups from the remaining students.
* Turn in a 2-page draft proposal (including references) by **February 6**. Remember to include the names and Michigan email addresses of the group members. You may submit the project proposal [here](https://docs.google.com/forms/d/e/1FAIpQLSd1tBj2B6ErcVtouJWmOoK8K19KS2naR7JmWbpT_DhVty94pA/viewform?usp=dialog).
* Each group must present mid-semester progress during class hours on **March 17 and March 19**.
* Each group must turn in an 8-page final report and your code via email **on or before 1:00PM EST on April 28.** The report must be submitted as a PDF file, with formatting similar to that of the papers you've read in the class. It should point to a git repository with all the code along with a README file with a step-by-step guide on how to compile and run the code.
* You can find how to access GPU resources [here](./Resources/Starting%20with%20Cloudlab).

## Tentative Grading
|                         | Weight | 
| ------------------------| ------:| 
| Paper Presentation      | 15%    | 
| Paper Summary           | 15%    | 
| Participation           | 10%    | 
| Project Report          | 40%    | 
| Project Presentations   | 20%    | 
