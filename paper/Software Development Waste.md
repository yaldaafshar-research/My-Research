# Software Development Waste

## Relevencies

[Paper's link]("https://ieeexplore.ieee.org/document/7985656/")

- The purpose of this paper is to identify and describe nine types of waste and their causes, underlying tension and overall relationship to the waste taxonomy found in Lean Software Development: building the wrong feature or product, mismanaging the backlog, rework, unnecessarily complex solutions, extraneous cognitive load, psychological distress, waiting/multitasking, knowledge loss, and ineffective communication.

- Adapting a taxonomy from a reference discipline (e.g. manufacturing) for a target discipline (e.g. software engineering)
manifests at least four threats to validity. We are not aware of any direct empirical validation of the Lean Software Development waste taxonomy; this motivates the current study.


## Take aways

- “waste” refers to “any activity that consumes resources but creates no value” for customers.
- Reducing waste is difficult not least because identifying waste is difficult. Numerous cognitive phenomena, including status quo bias, hinder practitioners’ propensity and ability to notice waste in existing practices.
- The similarities between batch-and-queue and waterfall software development, as well as just-in-time and iterative software development, inspired methods such as lean principles for software environments.

- **What types of waste are observable in software development?”**

- Lean Thinking discerns three types of activities: activities that clearly create value; activities that create no value for the customer but are currently necessary to manufacture the product; and activities that create no value for the customer, are unnecessary, and therefore
should be removed immediately; i.e., waste.
- Interestingly, these studies only found waiting waste generated in a batch-and-queue system
- These studies typically reduced waste by switching the organization from waterfall to iterative software development or reducing the batch size in iterative software development.

- **A. Waste: Building the Wrong Feature or Product**
- We observed this waste affecting team morale, team code ownership and customer satisfaction.
- **Tension:** Tension: User needs versus business wants.
- Some projects exhibit a tension between user needs and business goals. Practitioners may struggle to produce something that simultaneously
satisfies the users and the business.
- **B. Waste: Mismanaging the Backlog**
- The product backlog can be mismanaged in several ways, leading to delays of key features or lower team productivity.
- Backlog inversion: This occurs when the engineers working through the backlog get ahead of the product manager who is prioritizing the backlog.
- Mismanaging the backlog can also lead to duplicated work. This happens when two engineers working on the same story because one had forgotten to change its status and not communicating what they were doing in the backlog.
- **Tension:** Writing enough stories versus writing stories that will never be implemented
- Writing too few stories causes the team to idle while writing too many stories wastes the product manager’s time. 
- We observed teams running out of work on rare occasions; we did not observe product managers writing too many stories.
- **Tension:** Finishing features versus working on too many features simultaneously
- Starting work, changing priorities, and halting work in flight can result in waste.
- We observed that teams usually prefer to maintain a shippable product while rapidly finishing the simplest possible version of each new feature.
- **Tension:** intransigence versus capricious adjustments.
- Responding to change is more like a middle ground between intransigence (unreasonably refusing to change) and thrashing (changing features too often, especially arbitrarily alternating between equally good alternatives).
- **C. Waste: Rework**
- From a Waterfall perspective, one might classify any revision of existing code as “rework.”
- Our participants classify revising work that should have been done correctly but was not as rework, and improving existing work based on new information as new work.
-  We observed numerous sources of rework including technical debt, defects in work products, poor testing strategy, rejected stories, stories with no clear definition of done, and ambiguous mockups.
-Defects and bugs in the code, stories, mock-ups, and code result in rework.
- **D. Waste: Unnecessarily Complex Solutions**
- Unnecessarily complex solutions can be caused by feature complexity, technical complexity, or lack of reuse.
- Unnecessary feature complexity wastes users’ time as they struggle to understand how to use the system and achieve their objectives.
- In mockups, lack of reuse produces “snowflake designs,” interaction designs which do not take advantage of design reuse, e.g. two unique user interaction flows that could be unified into similar experiences or two visual components that solve the same concern.
- Singular designs require engineering to build unique solutions with no possibility of reuse
- **Tension:** Big design up-front versus incremental design.
- Big upfront design can produce incorrect or out-of-date assumptions and inability to cope with rapidly changing circumstances, also leading to expensive rework.
- No amount of up-front consideration appears sufficient to predict user feedback.
- The observed teams preferred to incrementally deliver functionality and delay integrating with technologies until a feature required it.
- **E. Waste: Extraneous Cognitive Load**
- Cognitive Load Theory posits that our working memory is quite limited and overloading it inhibits learning and problem solving
- Reducing the burden on working memory by removing extraneous cognitive load is therefore associated with more efficient learning among other positive outcomes
- While we cannot observe cognitive load directly, we did observe sources of extraneous cognitive load including overcomplicated stories, ineffective tooling, technical debt, and multitasking.
- Ineffective tooling includes convoluted, nonfunctional, premature, complicated, unstable, outdated, unsupported, timeconsuming, or inappropriate-for-the-task software libraries, as well as poorly designed development environments and deployment processes.
- Technical debt introduces the risks of the code being harder to understand and modify
- We observed teams suffering from technical debt with long-running, existing code bases.
- Overcomplicated stories—user stories that are unnecessarily long, complex, unclear, or replete with pointers to other necessary information
- Multitasking increases cognitive load as the multitasker attempts to hold two or more sets of information in working memory or needs to unnecessarily reload the information into working memory.

- **F. Waste: Psychological Distress** 
- Developers are a limited resource, which distress consumes. Job related psychological distress (e.g. release a fixed feature set by a fixed date.)causes absenteeism, burnout, lower productivity, and a variety of health problems
- Participants felt that fixing both scope and schedule was antithetical to Pivotal’s software process.
- **G. Waste: Waiting/multitasking**
- This “solution” to avoid waiting created extraneous cognitive load waste.
- **Tension:** Wait, block, or guess
- When needed information is missing, engineers appear to have three options,  however, The best option depends on how far into the story the pair is, how long they have to wait, and their confidence in their guess.
- **Tension:** Waiting versus context switching
- For example remedy problems or reduce the duration of future waiting (e.g. shorten the build), or work on something else instead of idling. - - Task switching decreases productivity and increases mistakes. For short waits, taking a break (e.g. playing table tennis) may be less wasteful than switching to another task.
- **H. Waste: Knowledge Loss**
- In projects with knowledge silos, team churn leads to wasted effort as the team regains lost knowledge
- The observed teams reduced knowledge loss of team churn or team member rotation by actively removing knowledge silos and caretaking the code by adopting the principles, policies, and practices of Sustainable Software Development
- We observed that large team sizes, asynchronous communication, imbalance in communication, and inefficient meetings reduced team productivity.
- Teams promoting knowledge sharing appear less susceptible to knowledge loss from team churn or team member rotation.
- **I. Waste: Ineffective Communication**
- Ineffective communication is incomplete, incorrect, misleading, inefficient, or absent communication. We observed that large team sizes, asynchronous communication, imbalance in communication, and inefficient meetings reduced team productivity.

- ## V. COMPARING TO LEAN SOFTWARE DEVELOPMENT

- Handoffs certainly contribute to the wastes of knowledge loss, ineffective communication, and waiting. However, our data does not support handoffs as a type of waste.
- **Building the wrong feature or product and Extra features:**
- Extra features does not cover the waste from missing important business needs. Building the wrong feature or product subsumes extra features. 
- **Mismanaging the backlog and Partially done work:**
- Interaction designers need to produce just enough mockups, product managers need to write just enough stories, and developers need to write just enough code to make the story work. In any continuous flow system, there are unfinished materials at each step.
- Large amounts of waiting designs or stories would have been classified as mismanaging the backlog waste.
- Mismanaging the backlog includes observed wastes beyond partially done work, namely, sequencing low priority work before high priority work,accidentally duplicating work, capricious thrashing, or delaying necessary bug fixes. Lean Software Development does not cover these wastes.
- **Rework and Defects:**
- Rework sunsumes Defects
- **Waiting/multitasking and Task switching:**
- Similar in both models(work on one thing at a time)
- **Waiting/multitasking and Delays**
- Both wastes describe the cost of missing needing information. Waiting subsumes delays
- In Lean Software Development, delays are “waiting for people to be available who are working in other areas” to provide needed information that is not available to the developers
- **Knowledge loss and Relearning:** 
- In our model, knowledge loss is the cost from members rolling off the team while In Lean Software Development, relearning is “rediscovering
something we once knew”, which includes the cost of an individual not remembering a decision already made.
- Knowledge loss focuses relearning to simply regaining departed knowledge.
- Included in relearning is failing to engage people in the development process. We did observe product managers having difficulty in involving some stakeholders, which we include in the building the wrong feature or product waste.

- ## VI. RESULTS EVALUATION AND QUALITY CRITERIA

- Organizations that are newer, less experienced, less concerned with waste, or use less iterative methods may experience additional waste types. 

## Methods

- Following Constructivist Grounded Theory, we conducted a two-year five-month participant-observation study of eight software development projects at Pivotal, a software development consultancy. We also interviewed 33 software engineers, interaction designers, and product managers, and analyzed one year of retrospection topics. We iterated between analysis and theoretical sampling until achieving theoretical saturation.
- Interviews were recorded, transcribed, coded, and analyzed using constant comparison. The data advanced from initial codes to focused codes, focused codes to core categories.
- When Removing Waste emerged as a core category, we incorporated data from retrospection meetings, performed additional interviews, and continued participant observation to refine the category. We constantly compared emerging findings to data from these three data sources until reaching saturation
- **interview method**: 
- The initial interviews began with the question, “Please draw on this sheet of paper your view of Pivotal’s software development process.” The interviewer intentionally avoided forcing initial topics, While exploring new emergent core categories, whenever possible, we initiated subsequent interviews with open-ended questions. The first author transcribed each interview with timecode stamps for each segment. These interviews were spread across the duration of the research study.
- **retrospection**: 
- The observed Pivotal teams mostly use an emotion-based retro format where “happy,” “neutral,” and “sad” faces are written on the top of a whiteboard. The happy-face column represents items that are working well and should be continued or expanded. The neutral-face column represents items that the team needs to “keep an eye on.” The sad-face column represents problems that the team should try to fix.
- Any team member can add any topic to any column. After a few minutes, the team dot-votes on the topics to discuss. The team uses
the remainder of the sixty-minute meeting to discuss topics. Sometimes discussing a topic is sufficient to affect change, other times the team creates action items.
- For co-located teams, the first author took a picture of the whiteboard at the end of the retro and later transcribed the
topics into a master spreadsheet. For distributed teams, we copied data from the online spreadsheets the team used in
place of a whiteboard. Attendees often wrote a short phrase as a proxy for a larger idea (e.g., “Scope” represents “Too much
scope is causing the team stress”). When the provided topic was too vague, we solicited a more detailed description from an engineer that was present at the meeting. This produced 663 total items for analysis.
- **Data Analysis**:
- We used line-by-line coding, to identify nuanced interactions in the data and avoid jumping to conclusions.
- We reviewed the initial codes while reading the transcripts and listening to the audio recordings. We discussed the coding during weekly research collaboration meetings. To avoid missing insights from these discussions, we recorded and transcribed them into Grounded Theory memos.
As data was collected and coded, we stored initial codes in a spreadsheet and we used constant comparison to generate focused codes.
- We routinely compared new codes to existing codes to refine codes and eventually generate categories.
- When this became complex, we printed codes on index cards to facilitate reorganization
- **the results might be influenced by researcher bias or prior knowledge bias**
- During participant observation, the researcher may lose perspective and become biased by being a member of the team. That is, while a participant-observer gains perspective an outsider cannot, an outside observer might see something a participant observer will miss. Similarly,
while prior knowledge helps the researcher interpret events and select lines of inquiry, prior knowledge may also blind the researcher to alternative explanations. We mitigated these risks by recording interviews and having the second and third authors review the coding process.

## Data

- This paper analyses data from three sources: 1) participant observation of eight projects over two years and five months, 2) interviews with Pivotal employees, and 3) topics discussed in 91 retrospection meetings.
- **Participant Observation**:The first author collected field notes while working as an engineer on eight projects. These notes describe individual and collective actions, capture what participants found interesting or problematic, and include anecdotes and observations.)(Projects are de-identified to preserve client confidentiality)
- **Interviews**:The first author interviewed 33 interaction designers, product managers, and software engineers who had experience with Pivotal’s software development process from five different Pivotal offices. Participants were not paid for their time. We relied on "intensive interviews".
- The interviewer attempts to abandon assumptions to better understand and explore the interviewee’s perspective
- **retrospection**: We collected data from 91 retrospection meetings over 59 weeks from Projects Quattuor, Kvin, and Ses. (There are more meetings than weeks since each of Project Quattuor’s three teams held its own retro each week.) an engineer that was present at the meeting. This produced 663 total items for analysis.

## Conclusion

- While this research supports parts of the Lean Software Development waste taxonomy, it differs in three key ways:
1) it introduces four new waste categories: unnecessarily complex solutions, extraneous cognitive load, psychological distress, and ineffective communication; 2) it does not support Lean Software Development’s handoffs waste category; and 3) its waste categories are largely broader than Lean Software Development’s categories.