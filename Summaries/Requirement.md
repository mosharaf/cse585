# Requirements for CSE 585 Lecture Summary

## Submission 

Your summary should be submitted as a single Google Doc file.
You should share the Google Doc with us by granting [cse585-staff@umich.edu](mailto:cse585-staff@umich.edu) as the Commenter.
Then, email us the Google Doc link at [cse585-staff@umich.edu](mailto:cse585-staff@umich.edu).

At the top of the Google Doc file, note clearly about the full name and unique names of all team members.
Note also the lecture date.

Submissions violating the above will not be graded.

*The paper summary of a paper must be emailed to the instructor team within 24 hours after its presentation.* 
**Late summaries will not be graded.** 

## AI-assisted Lecture Summary

Write a summary for the **research area** your assigned lecture has discussed.
You are required to use any AI tools of your choice to assist you with doing it.

Your submission should contain the following sections:

### Section 1: The general research direction of the area

Each lecture has several papers, all of which belong to a certain research area.
In this section, you should summarize the general area the papers have covered. 

You should discuss the following:
* What is the research problem in the lecture, and why is this problem important?
* What is the state of related work *before* the lecture papers' apperance?
* At a very high level, what problems do the lecture papers solve and where do they stand in the research area?
* If applicable, briefly introduce some follow-up solutions to the lecture papers?

Your area summarization should demonstrate that you have done a careful survey of this area,
and that you understand the high-level idea of the related works other than the lecture papers
(for the lecture papers, you should understand all of its details).
Simply listing what the related works do will receive a low score.

For example, the September 16 lecture discusses systems for LLM pretraining.
A good idea is to introduce what the general system problems (communication, memory usage, work imbalance, etc.) are for large scale training and why they are hard to solve.
Then, explain what problems the lecture papers have solved, and how they have contributed to the area.
Finally, discuss what problems are still open, especially the problems the lecture papers tackle but do not solve.
Use related works as evidence.

### Section 2: Lecture papers

In this part, you should write summaries for all the *required* papers discussed in the lecture.
The summary in this section should focus more on the technical details of the problems and solutions about the papers themselves.

Be sure to address the following aspects in bold text.
Under each aspect, we provide some guidelines that you can choose to follow, but feel free to adjust it to your own preference.
* **What is the problem of this paper?** Guidelines:
  * Is this problem important and/or hard?
  * What aspects have the existing solutions missed?
  * Does the paper provide sufficient theoratical or experimental evidence to support the problem?
* **What is the solution of this paper?** Guidelines:
  * What is the key insight that drives the solution?
  * What assumption does the solution rely on? Do they reduce the problem logically, or do they oversimplify?
  * What might be the tradeoff of the solution?
* **How is the solution evaluated?** Guidelines:
  * Is the evaluation set up in a correct way? How is the solution implemented, what hardware and workload is involved?
  * What are the properties that the solution has evaluated? Are the properties tied to the problem?
  * What results are expected, and what are unexpected in the evaluation?
* **Overall, what are the shortcomings about this paper? List 1-2 shortcomings.**

### Section 3: Lecture discussions

Summarize the main questions raised and discussed in the lecture.
You may summarize it in a Q & A form or any other form you prefer.
According to [FERPA](https://safecomputing.umich.edu/protect-privacy/privacy-u-m/videoconferencing/recording-privacy-concerns),
you are not allowed to record the lecture.
Therefore, pay attention to the lecture discussion and make sure you summarize all the main points.

### Section 4: Proposal for a follow-up work

Propose a new project in this field.
Study the state-of-the-art of the area after the performing the survey in Section 1.
Then, identify an open problem in the field and propose a solution to it.
This does not need to be a lengthy proposal and should be at most 3 short paragraphs.
However, it should reflect that you have thought about the field carefully and have an understanding of its landscape.
You should also evaluate your solution logically, pondering the same questions as when you are writing paper summary.
You may take writing this section as a chance of writing a short version of the proposal of your own group project.

### Section 5: A reflection on AI usage

For Sections 1, 2, and 4, you are required to use AI to assist you with them.
In fact, without AI, it is impossible to perform a survey of a whole field quickly.

In this section, summarize the experience of how AI helped you complete the above sections.
You should reflect where AI was helpful and where not so.
To obtain a high score, you should cite concrete examples from Section 6.

### Section 6: A transcript of your conversation with AI 

Provide a **complete and unmodified** transcript of your multi-turn conversation with your AI tool.
You should label the model (e.g., GPT-6 Astra), tool (ChatGPT Desktop), and the date(s) the conversation takes place.

Start a new page for Section 6.
Paste it as plain text to the Google Doc.
Use different text styles to distinguish prompt and AI responses.

## Guidelines

Try to be creative about the conversation.
Some ideas include (but do not limit yourself to them):

* Give the AI a short spec of how it will summarize the paper
* Ask the AI detailed technical questions that you have trouble understanding in the paper
* Ask it about the paper's relationship to another paper you have read
* State that you dislike a specific aspect of the paper, and ask the AI's opinion
* Ask the AI's opinion about a question raised in the lecture

You are also free to choose the number of sessions to have with the AI and what context to provide.

For Sections 1-5, you are required to write under 3 pages of Google Doc at 12pt and single line space.
We will not read any text that exceeds 3 pages.
Section 6 does not have a length limit, so you should submit a complete conversation.

Your submission will be public on GitHub throughput the semester.
One purpose of this assignment is that the students and instructor can read your summary and pick up the lecture's discussion quickly.
Therefore, it will be a waste of everyone's time if you write a simple prompt to AI and generate massive slop for this summary.
Doing so will result in a very low score.

## Best Summary Award

Toward the end of semester, you will vote on the best summary of all lectures.
All members of the Best Summary Award team will receive 2 bonus points for this course.
