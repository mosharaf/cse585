# CSE 585: Advanced Scalable Systems for Generative AI (F'25)

## Administrivia
* Catalog Number: 31041
* Lectures/Discussion: 2150 DOW, TTh: 10:30 AM – 12:00 PM
* Projects/Makeup: 1500 EECS, F 1:30 PM – 2:30 PM
* Counts as: Software Breadth and Depth (PhD); Technical Elective and 500-Level (MS/E)

### Team

| Member (uniqname) | Role | Office Hours |
| :---------------- | :--- | :----------- |
| [Mosharaf Chowdhury](http://www.mosharaf.com/) (mosharaf) | Faculty | 4156 LEIN. **By appointments only.**
| [Jae-Won Chung](https://jaewonchung.me/about) (jwnchung) | GSI | 4828 BBB. Fri 10:30 AM - 11:30 AM.

### Communication
**ALL** communication regarding this course must be via [Ed](https://edstem.org/us/join/F6zqDH).
This includes questions, discussions, announcements, as well as private messages.

Presentation slides and paper summaries should be emailed to [cse585-staff@umich.edu](mailto:cse585-staff@umich.edu).

## Course Description
This iteration of CSE585 will introduce you to the key concepts and the state-of-the-art in practical, scalable, and fault-tolerant systems for Generative AI (GenAI) and encourage you to think about either building new tools or how to apply the existing ones.

Since datacenters and cloud computing form the backbone of modern computing, we will start with an overview of the two. 
We will then take a deep dive into systems for the Generative AI landscape, focusing on different types of problems. 
Our topics will include: basics on generative models from a systems perspective; systems for GenAI lifecycle including pre-training, post-training, and inference serving systems; agentic AI; etc. 
We will cover GenAI topics primarily from top conferences that take a systems view to the relevant challenges.

Note that this course is **NOT focused on AI methods**. 
Instead, we will *focus on how one can build systems* so that existing AI methods can be used in practice and new AI methods can emerge. 

### Prerequisites
Students are expected to have good programming skills and must have taken *at least one* undergraduate-level systems-related course (from operating systems/EECS482, databases/EECS484, distributed systems/EECS491, and networking/EECS489).
Having an undergraduate ML/AI course may be helpful, but not required or necessary. 

### Textbook
This course has no textbooks.
We will read recent papers from top venues to understand trends in scalable GenAI and agentic systems, and their applications.

## Tentative Schedule and Reading List

*This is an evolving list and subject to changes due to the breakneck pace of GenAI innovations.*

| Date | Readings | Presenter | Summary | Reviewer |
| :---- | :---- | :---- | :---- | :---- |
| Aug 26 | **Introduction** | [Mosharaf](Slides/082625-MChowdhury.pdf) |  |  |
|  | [How to Read a Paper](http://svr-sk818-web.cl.cam.ac.uk/keshav/papers/07/paper-reading.pdf) (Required) |  |  |  |
|  | [How to Give a Bad Talk](http://www.cs.berkeley.edu/~pattrsn/talks/BadTalk.pdf) (Required) |  |  |  |
|  | [The Datacenter as a Computer](https://link.springer.com/book/10.1007/978-3-031-01761-2) (Chapters 1 and 2\) |  |  |  |
|  | [Machine Learning Fleet Efficiency: Analyzing and Optimizing Large-Scale Google TPU Systems with ML Productivity Goodput](https://arxiv.org/abs/2502.06982) |  |  |  |
| Aug 28 | **Introduction to GenAI and Systems for GenAI** | [Jae-Won](Slides/082825-jwnchung.pdf) |  |  |
|  | [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) (Required) |  |  |  |
|  | [The Illustrated Stable Diffusion](https://jalammar.github.io/illustrated-stable-diffusion/) (Required) |  |  |  |
|  | [Deep Dive into LLMs like ChatGPT](https://www.youtube.com/watch?v=7xTGNNLPyMI) (Required) |  |  |  |
| Sep  2 | **No Lecture: Find Project Groups** |  |  |  |
|  | [Hints and Principles for Computer System Design](https://arxiv.org/abs/2011.02455) (Required) |  |  |  |
| Sep  4 | **Distributed Training Basics** | [Jae-Won](Slides/090425-jwnchung.pdf) |  |  |
|  | [Efficient Large-Scale Language Model Training on GPU Clusters Using Megatron-LM](https://dl.acm.org/doi/10.1145/3458817.3476209) (Required) |  |  |  |
| Sep  9 | **No Lecture: Work on Project Proposals** |  |  |  |
|  | [Writing Reviews for Systems Conferences](http://people.inf.ethz.ch/troscoe/pubs/review-writing.pdf) (Required) |  |  |  |
|  | [Worse is Better](https://en.wikipedia.org/wiki/Worse_is_better) (Required) |  |  |  |
|  | **Pre-Training** |  |  |  |
| Sep 11 | [Pipeline Parallelism with Controllable Memory](https://proceedings.neurips.cc/paper_files/paper/2024/hash/527dad0b9159805289906d5740a0bdd3-Abstract-Conference.html) (Required) | [Patrick, Nathan, Hannah](Slides/091125-pnhalim-nyap-hyshu.pdf) | [Letian, Terry, Fu-Shiang](Summaries/091125-ruanlt-weiceica-fsyang.pdf) | Eric, John, Albert, Vishnu |
|  | [Zero Bubble (Almost) Pipeline Parallelism](https://openreview.net/forum?id=tuzTN0eIO5) |  |  |  |
|  | [WLB-LLM: Workload-Balanced 4D Parallelism for Large Language Model Training](https://www.usenix.org/conference/osdi25/presentation/wang-zheng) (Required) |  |  |  |
| Sep 16 | [Alpa: Automating Inter- and Intra-Operator Parallelism for Distributed Deep Learning](https://www.usenix.org/conference/osdi22/presentation/zheng-lianmin) (Required) | [Aaron, Uygur, Brandon](Slides/091625-aaronbar-tepe-bchao.pdf) | [Yana, Sami, David](Summaries/091625-samiuf-dmcde-yrpatel.pdf) | Gary, Tongyuan, Annie, Kai Jun |
|  | [PartIR: Composing SPMD Partitioning Strategies for Machine Learning](https://dl.acm.org/doi/10.1145/3669940.3707284) (Required) |  |  |  |
| Sep 18 | [Understanding Stragglers in Large Model Training Using What-if Analysis](https://www.usenix.org/conference/osdi25/presentation/lin-jinkun) | [Satyam, Arjun, Tanush, Kushal](Slides/091825-sagoyal-arlx-tmittal-patelku.pdf) | [Arnav Reddy, Nishant, Muzhe, Yuxuan](Summaries/091825-arnavr-ndash-henrw-liurick.pdf) | Yuewen, Dhanvi, Rudrajyoti, Haoran |
|  | [SuperBench: Improving Cloud AI Infrastructure Reliability with Proactive Validation](https://www.usenix.org/conference/atc24/presentation/xiong) (Required) |  |  |  |
|  | [Training with Confidence: Catching Silent Errors in Deep Learning Training with Automated Proactive Checks](https://www.usenix.org/conference/osdi25/presentation/jiang) (Required) |  |  |  |
| Sep 23 | [Oobleck: Resilient Distributed Training of Large Models Using Pipeline Templates](https://dl.acm.org/doi/10.1145/3600006.3613152) (Required) | [Sharvani, Shresth, Divya](Slides/092325-sharvani-shresth-shdivya.pdf) | [Eric, John, Albert, Vishnu](Summaries/092325-zhaoeric-johnxie-caoalb-vishnuka.pdf) | Hui, Zesen, Boyuan |
|  | [Tenplex: Dynamic Parallelism for Deep Learning using Parallelizable Tensor Collections](https://dl.acm.org/doi/10.1145/3694715.3695975) (Required) |  |  |  |
|  | **Post-Training** |  |  |  |
| Sep 25 | [Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters](https://arxiv.org/abs/2408.03314) (Required) | [Krithika, Kristine, Thomas](Slides/092525-krithiv-ksmcl-mperform.pdf) | [Evan, Naveen, Pranavkumar, Anirudh](Summaries/092525-anikrish-evanzimm-naveenu-pmallela.pdf) | Letian, Terry, Fu-Shiang |
|  | [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948) (Required) |  |  |  |
| Sep 30 | [HybridFlow: A Flexible and Efficient RLHF Framework](https://dl.acm.org/doi/10.1145/3689031.3696075) (Required) | Esha, Chimaobi, Alvaro | Gary, Tongyuan, Annie, Kai Jun | Yana, Sami, David |
|  | [AReaL: A Large-Scale Asynchronous Reinforcement Learning System for Language Reasoning](https://arxiv.org/abs/2505.24298) (Required) |  |  |  |
|  | **Inference** |  |  |  |
| Oct  2 | **Inference Basics** | Jae-Won |  |  |
|  | [Orca: A Distributed Serving System for Transformer-Based Generative Models](https://www.usenix.org/conference/osdi22/presentation/yu) (Required) |  |  |  |
|  | [Efficient Memory Management for Large Language Model Serving with PagedAttention](https://dl.acm.org/doi/10.1145/3600006.3613165) (Required) |  |  |  |
| Oct  7 | [DistServe: Disaggregating Prefill and Decoding for Goodput-Optimized Large Language Model Serving](https://www.usenix.org/conference/osdi24/presentation/zhong-yinmin) (Required) | Wonbin, Roee, Rohit, Arnav Shah | Patrick, Nathan, Hannah | Evan, Naveen, Pranavkumar, Anirudh |
|  | [Taming Throughput-Latency Tradeoff in LLM Inference with Sarathi-Serve](https://www.usenix.org/conference/osdi24/presentation/agrawal) (Required) |  |  |  |
| Oct  9 | [NanoFlow: Towards Optimal Large Language Model Serving Throughput](https://www.usenix.org/conference/osdi25/presentation/zhu-kan) (Required) | Eric, John, Albert, Vishnu | Yuewen, Dhanvi, Rudrajyoti, Haoran | Aaron, Uygur, Brandon |
|  | [Mooncake: Trading More Storage for Less Computation — A KVCache-centric Architecture for Serving LLM Chatbot](https://www.usenix.org/conference/fast25/presentation/qin) (Required) |  |  |  |
| Oct 14 | **Fall Study Break** |  |  |  |
| Oct 16 | [LoongServe: Efficiently Serving Long-Context Large Language Models with Elastic Sequence Parallelism](https://dl.acm.org/doi/10.1145/3694715.3695948) (Required) | Letian, Terry, Fu-Shiang | Esha, Chimaobi, Alvaro | Arnav Reddy, Nishant, Muzhe, Yuxuan |
|  | Tentative: Cornserve (Required) |  |  |  |
| Oct 21 | **Mid-Semester Presentations** |  |  |  |
| Oct 23 | **Mid-Semester Presentations** |  |  |  |
| Oct 28 | **No Lecture: Work on Projects** |  |  |  |
| Oct 30 | [PowerInfer: Fast Large Language Model Serving with a Consumer-Grade GPU](https://dl.acm.org/doi/10.1145/3694715.3695964) (Required) | Gary, Tongyuan, Annie, Kai Jun | Satyam, Arjun, Tanush, Kushal | Krithika, Kristine, Thomas |
|  | [FlexGen: High-Throughput Generative Inference of Large Language Models with a Single GPU](https://icml.cc/virtual/2023/oral/25565) (Required) |  |  |  |
| Nov  4 | [Andes: Defining and Enhancing Quality-of-Experience in LLM-Based Text Streaming Services](https://arxiv.org/abs/2404.16283) (Required) | Arnav Reddy, Nishant, Muzhe, Yuxuan | Sharvani, Shresth, Divya | Satyam, Arjun, Tanush, Kushal |
|  | [On Evaluating Performance of LLM Inference Serving Systems](https://arxiv.org/abs/2507.09019) (Required) |  |  |  |
|  | [Tempo: Application-aware LLM Serving with Mixed SLO Requirements](https://arxiv.org/abs/2504.20068) |  |  |  |
|  | **Agentic Systems** |  |  |  |
| Nov  6 | [Parrot: Efficient Serving of LLM-based Applications with Semantic Variable](https://www.usenix.org/conference/osdi24/presentation/lin-chaofan) (Required) | Hui, Zesen, Boyuan | Krithika, Kristine, Thomas | Esha, Chimaobi, Alvaro |
|  | [Towards End-to-End Optimization of LLM-based Applications with Ayo](https://dl.acm.org/doi/10.1145/3676641.3716278) (Required) |  |  |  |
| Nov 11 | [METIS: Fast Quality-Aware RAG Systems with Configuration Adaptation](https://arxiv.org/abs/2412.10543) (Required) | Evan, Naveen, Pranavkumar, Anirudh | Aaron, Uygur, Brandon | Sharvani, Shresth, Divya |
|  | [Fast Vector Query Processing for Large Datasets Beyond GPU Memory with Reordered Pipelining](https://www.usenix.org/conference/nsdi24/presentation/zhang-zili-pipelining) (Required) |  |  |  |
|  | **Hardware / Infrastructure** |  |  |  |
| Nov 13 | [WaferLLM: Large Language Model Inference at Wafer Scale](https://www.usenix.org/conference/osdi25/presentation/he) (Required) | Yuewen, Dhanvi, Rudrajyoti, Haoran | Wonbin, Roee, Rohit, Arnav Shah | Patrick, Nathan, Hannah |
|  | [Insights into DeepSeek-V3: Scaling Challenges and Reflections on Hardware for AI Architectures](https://dl.acm.org/doi/10.1145/3695053.3731412) (Required) |  |  |  |
|  | [Meta's Second Generation AI Chip: Model-Chip Co-Design and Productionization Experiences](https://dl.acm.org/doi/10.1145/3695053.3731409) |  |  |  |
|  | [Ironwood: The first Google TPU for the age of inference](https://blog.google/products/google-cloud/ironwood-tpu-age-of-inference/) |  |  |  |
|  | **Power and Energy Management** |  |  |  |
| Nov 18 | [Reducing Energy Bloat in Large Model Training](https://dl.acm.org/doi/10.1145/3694715.3695970) (Required) | Invited lecture by [Ruofan Wu](https://ruofan-wu.github.io/) |  |  |
|  | [TAPAS: Thermal- and Power-Aware Scheduling for LLM Inference in Cloud Platforms](https://dl.acm.org/doi/10.1145/3676641.3716025) (Required) |  |  |  |
|  | Tentative: Kareus |  |  |  |
| Nov 20 | [Power Stabilization for AI Training Datacenters](https://arxiv.org/abs/2508.14318) (Required) | Yana, Sami, David | Hui, Zesen, Boyuan | Wonbin, Roee, Rohit, Arnav Shah |
|  | [AI Training Load Fluctuations at Gigawatt-scale – Risk of Power Grid Blackout?](https://semianalysis.com/2025/06/25/ai-training-load-fluctuations-at-gigawatt-scale-risk-of-power-grid-blackout) (Required) |  |  |  |
|  | **Wrap Up** |  |  |  |
| Nov 25 | [On the Dangers of Stochastic Parrots: Can Language Models be too Big?🦜](https://dl.acm.org/doi/abs/10.1145/3442188.3445922) (Required) | Mosharaf |  |  |
|  | [We Need a New Ethics for a World of AI Agents](https://www.nature.com/articles/d41586-025-02454-5) (Required) |  |  |  |
| Nov 27 | **No Lecture: Thanksgiving Recess** |  |  |  |
| Dec  2 | **No Lecture: Work on Posters** | |  |  |
|  | [How to Write a Great Research Paper](https://www.microsoft.com/en-us/research/academic-program/write-great-research-paper/) (Required) |  |  |  |
| Dec  4 | **Final Poster Presentations** TBA | [Template](http://Resources/poster.pptx) |  |  |

## Policies

### Honor Code
[The Engineering Honor Code](https://ecas.engin.umich.edu/honor-council/honor-code/) applies to all activities related to this course.

### Groups
All activities of this course will be performed in **groups of 3-4 students**.

### Required Reading
Each lecture will have **two required reading that everyone must read**.  
There will be *one or more optional related reading(s)* that only the presenter(s) should be familiar with.
They are optional for the rest of the class.

### Student Lectures
The course will be conducted as a seminar. 
Only one group will present in each class.
Each group will be assigned *at least one lecture* over the course of the semester. 
Presentations should cover all required papers for that lecture.
The duration of the presentation should be **at most 40 minutes** if there were no interruptions.
Presenters should expect questions and interruptions throughout.

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
  - You are required to [submit](https://docs.google.com/forms/d/e/1FAIpQLSdkFwdHw3AnJPl_7QiKvWK7XqdzsVFg8WUjbXu-4hfFbh3Chw/viewform?usp=dialog) **one insightful question** for each presented paper before each class. 
  - During the panel discussions, feel free to actively **ask questions** and engage in the dialogue. 

### Participation
Given the discussion-based nature of this course, participation is required both for your own understanding and to improve the overall quality of the course.
You are expected to attend **all** lectures (you may skip up to 2 lectures due to legitimate reasons), and more importantly, participate in class discussions.

A key part of participation will be in the form of discussion in Ed.
The group in charge of the summary should initiate the discussion and the rest should participate.
Not everyone must have add something every day, but it is expected that everyone has something to say over the semester.

### Project
You will have to complete substantive work an instructor-approved problem and have original contribution.
Surveys are not permitted as projects; instead, each project must contain a survey of background and related work.

You must meet the following milestones (unless otherwise specified in future announcements) to ensure a high-quality project at the end of the semester:

* Form a group of 3-4 members and [declare your group's membership and paper preferences](https://docs.google.com/forms/d/e/1FAIpQLScLAghst8rcX5b1hdXXQlYVLTb1SMMRTSNnO5XrPQppnq437w/viewform?usp=dialog) by **September 4**. After this date, we will form groups from the remaining students.
* Turn in a 2-page draft proposal (including references) by **September 18**. Remember to include the names and Michigan email addresses of the group members. 
* Each group must present mid-semester progress during class hours on **October 21 and October 23**.
* Each group must turn in an 8-page final report and your code via email **on or before 1:00PM EST on December 15.** The report must be submitted as a PDF file, with formatting similar to that of the papers you've read in the class. It should point to a git repository with all the code along with a README file with a step-by-step guide on how to compile and run the code.
* You can find how to access GPU resources [here](./Resources/Starting%20with%20Cloudlab).

## Tentative Grading
|                         | Weight | 
| ------------------------| ------:| 
| Paper Presentation      | 15%    | 
| Paper Summary           | 15%    | 
| Participation           | 10%    | 
| Project Report          | 40%    | 
| Project Presentations   | 20%    | 
