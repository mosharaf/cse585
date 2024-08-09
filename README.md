# CSE 585: Advanced Scalable Systems for Generative AI (F'24)

## Administrivia
* Catalog Number: 34176
* Lectures/Discussion: 1003 EECS, TTh: 10:30 AM – 12:00 PM
* Projects/Makeup: 185 EWRE, F 1:30 PM – 2:30 PM
* Counts as: Software Breadth (PhD); Technical Elective and 500-Level (MS/E)

### Team

| Member (uniqname) | Role | Office Hours |
| :---------------- | :--- | :----------- |
| [Mosharaf Chowdhury](http://www.mosharaf.com/) (mosharaf) | Faculty | 4820 BBB. **By appointments only.**
| [Insu Jang](https://insujang.github.io/) (insujang) | GSI | TBA

### Piazza
**ALL** communication regarding this course must be via [Piazza](https://piazza.com/umich/fall2024/cse585).
This includes questions, discussions, announcements, as well as private messages.

Presentation slides and paper summaries should be emailed to [cse585-staff@umich.edu](mailto:cse585-staff@umich.edu).

## Course Description
This iteration of CSE585 will introduce you to the key concepts and the state-of-the-art in practical, scalable, and fault-tolerant software systems for emerging Generative AI (GenAI) and encourage you to think about either building new tools or how to apply an existing one in your own research.

Since datacenters and cloud computing form the backbone of modern computing, we will start with an overview of the two. 
We will then take a deep dive into systems for the Generative AI landscape, focusing on different types of problems. 
Our topics will include: basics on generative models from a systems perspective; systems for GenAI lifecycle including pre-training, fine-tuning/alignment, grounding, and inference serving systems; etc. 
We will cover GenAI topics from top conferences that take a systems view to the relevant challenges.

Note that this course is **NOT focused on AI methods**. 
Instead, we will *focus on how one can build software systems* so that existing AI methods can be used in practice and new AI methods can emerge. 

### Prerequisites
Students are expected to have good programming skills and must have taken *at least one* undergraduate-level systems-related course (from operating systems/EECS482, databases/EECS484, distributed systems/EECS491, and networking/EECS489).
Having an undergraduate ML/AI course may be helpful, but not required or necessary. 

### Textbook
This course has no textbooks.
We will read recent papers from top venues to understand trends in scalable (GenAI) systems and their applications.

## Tentative Schedule and Reading List
*This is an evolving list and subject to changes due to the breakneck pace of GenAI innovations.* 

| Date    | Readings                       | Presenter | Summary | Reviewer
| --------| -------------------------------| --------- | ------- | -------
| Aug 27  | **Introduction** | Mosharaf
|         | [How to Read a Paper](http://svr-sk818-web.cl.cam.ac.uk/keshav/papers/07/paper-reading.pdf) (Required)
|         | [How to Give a Bad Talk](http://www.cs.berkeley.edu/~pattrsn/talks/BadTalk.pdf) (Required)
|         | [Writing Reviews for Systems Conferences](http://people.inf.ethz.ch/troscoe/pubs/review-writing.pdf)
|         | [The Datacenter as a Computer](https://link.springer.com/book/10.1007/978-3-031-01761-2) (Chapters 1 and 2)
|         | **GenAI Basics**
| Aug 29  | 
| Sep  3  | 
| Sep  5  | 
| Sep 10  | **No Lecture: Work on Projects**
| Sep 12  | **Buffer**
|         | **Pre-Training**
| Sep 17  | 
| Sep 19  | 
| Sep 24  | 
| Sep 26  | 
|         | **Post-Training**
| Oct  1  | 
|         | **Inference**
| Oct  3  | 
| Oct  8  | 
| Oct 10  | 
| Oct 15  | **Fall Study Break**
| Oct 17  | 
| Oct 22  | **Mid-Semester Presentations**
| Oct 24  | **Mid-Semester Presentations**
| Oct 29  | **No Lecture: Work on Projects**
| Oct 31  | **Buffer**
| Nov  5  | **No Lecture: Work on Projects**
| Nov  7  | 
| Nov 12  | 
|         | **Grounding**
| Nov 14  | 
|         | **Power, Energy, and Carbon Emissions**
| Nov 19  | 
|         | **GenAI for Systems**
| Nov 21  | 
|         | **Ethical Considerations**
| Nov 26  | 
| Nov 28  | **No Lecture: Thanksgiving Recess**
| Dec  3  | **Buffer**
| Dec  5  | **Final Poster Presentations**<br>TBA

## Policies

### Honor Code
[The Engineering Honor Code](https://ecas.engin.umich.edu/honor-council/honor-code/) applies to all activities related to this course.

### Groups
All activities of this course will be performed in **groups of 2-3 students**.

### Required Reading
Each lecture will have **two required reading that everyone must read**.  
There will be *one or more optional related reading(s)* that only the presenter(s) should be familiar with.
They are optional for the rest of the class.

### Student Lectures
The course will be conducted as a seminar. 
Only one group will present in each class.
Each group will be assigned *at least one lecture* over the course of the semester. 
Presentations should last **at most 40 minutes** without interruption.
However, presenters should expect questions and interruptions throughout. 

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
- Group Assignment: Each group will be assigned to one slot to play the role of reviewers.
- Responsibility: Reviewers critically assess the paper, posing challenging questions and highlighting potential weaknesses or areas for further investigation. 
Your goal is to engage in a constructive critique of the paper, simulating a peer review scenario.

 
3. **Rest of the Class**
- Responsibility: 
  - You are required to [submit](TBA) **one insightful question** for each presented papers before each class. 
  - During the panel discussions, feel free to actively **ask questions** and engage in the dialogue. 

### Participation
Given the discussion-based nature of this course, participation is required both for your own understanding and to improve the overall quality of the course.
You are expected to attend **all** lectures (you may skip up to 2 lectures due to legitimate reasons), and more importantly, participate in class discussions.

A key part of participation will be in the form of discussion in Piazza.
The group in charge of the summary should initiate the discussion and the rest should participate.
Not everyone must have add something every day, but it is expected that everyone has something to say over the semester.

### Project
You will have to complete substantive work an instructor-approved problem and have original contribution.
Surveys are not permitted as projects; instead, each project must contain a survey of background and related work.

You must meet the following milestones (unless otherwise specified in future announcements) to ensure a high-quality project at the end of the semester:

* Form a group of 2-3 members and [declare your group's membership and paper preferences](TBA) by **September 5**. After this date, we will form groups from the remaining students.
* Turn in a 2-page draft proposal (including references) by **September 19**. Remember to include the names and Michigan email addresses of the group members. 
* Each group must present mid-semester progress during class hours on **October 22 and October 24**.
* Each group must turn in an 8-page final report and your code via email **on or before 6:00PM EST on December 16.** The report must be submitted as a PDF file, with formatting similar to that of the papers you've read in the class. The self-contained (i.e., include ALL dependencies) code must be submitted as a zip file. Each zip file containing the code must include a README file with a step-by-step guide on how to compile and run the provided code.
* You can find how to access GPU resources [here](./Resources/Starting%20with%20Cloudlab).

## Tentative Grading
|                         | Weight | 
| ------------------------| ------:| 
| Paper Presentation      | 15%    | 
| Paper Summary           | 15%    | 
| Participation           | 10%    | 
| Project Report          | 40%    | 
| Project Presentations   | 20%    | 
