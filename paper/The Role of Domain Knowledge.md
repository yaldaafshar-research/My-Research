# The Role of Domain Knowledge and Cross-Functional Communication in Socio-Technical Coordination

## Relevencies

[Paper's link](https://ieeexplore.ieee.org/document/6606590")

- By understanding the interrelationships between task assignments, cross-functional communication structure, and domain knowledge, organizations gain an increased ability to facilitate communication and coordination in their projects. We hope this will lead to software projects with less wasted communication, less coordination overhead, and increased leverage of the diversity in project roles and domain knowledge.

## Take aways

- We found that communication only partially matched task dependencies and that team members that are boundary spanners have extensive domain knowledge and hold key positions in the control
structure.
- These researchers have analyzed socio-technical alignment, which examines how the technical aspects of software engineering are matched by the work-related interactions of software
developers
- One measure of socio-technical alignment is sociotechnical congruence (STC), which calculates the
alignment of actual communication with the anticipated coordination needs of team members based on technical task assignments and task dependencies.
- A way to study coordination between diverse roles is to look at a higher level of abstraction: requirements.
- Requirements create dependencies among downstream artifacts such as design, architecture, code, and test cases.
- Communication driven by requirements takes place within cross-functional teams involving developers, business analysts and testers, and that the most predominant reason for communication was changes in requirements
- To complete their tasks, team members often stretch their communication by reaching out to those that possess in-depth domain knowledge across different teams and geographical locations
- **RQ1: What is the nature of task dependencies, project communication and socio-technical alignment in a requirements view on coordination?**
- Organizations follow a hierarchical structure in which certain organizational roles control information flow within and across teams or departments
- In popular open-source software projects, communication was centered on small, interoperating groups of developers.
- Dense structures tended to be associated with communication problems
- Hierarchical networks delivered more features than close-knit networks but had lower quality
- Organizational structures may also impede knowledge flow if the structure is not defined according to task assignments, and studies of organizational behavior document the role of informal networks in task accomplishment
- **RQ2: How does the cross-functional communication structure influence actual communication of various roles in coordination?**
- Domain knowledge is the implicit knowledge about client needs, thei business domain and the system’s environment
- Involving multiple functional roles also introduces differences in domain knowledge within the team.
- Often, the domain expert does not plan to be in this brokering position, thus, Thus, coordination and communication patterns within projects may not align with task coordination and instead follow informal connections governed by domain expertise
- **RQ3: How does the spread of domain knowledge influence communication of various roles in coordination?**
- We also asked for the reason of communication between project members and any additional
members s/he communicated with, which was one of the following: requirements clarification, negotiation, communication of requirements changes, or coordination of activities.
- **Analysis Result:** 
- **RQ1:** 
- At least one third of the anticipated coordination needs between team members did not have corresponding communication. However, both
projects had substantial emergent communication, which are communication links not predicted by coordination needs.
- Task dependencies are grouped within application portfolios.
- Since there were no architectural dependencies between the application portfolios, the few cross-portfolio dependencies
were the result of some members being assigned to requirements in multiple portfolios due to their domain knowledge.
- Emergent interactions involve team members that possess domain knowledge who had no coordination needs.
- Most emergent members represent sources of application domain knowledge; they are customers, business analysts or environment coordinators, or had been involved in requirements negotiations in SHIP (e.g. dev leads) or in the reverse engineering efforts in APP
- Communication brokers have domain knowledge.
- Brokers are those who mediate between members not communicating directly
- In APP, the RAs and dev leads were the points of contact when customers needed to be contacted.
- Both the task dependencies and the actual communication were grouped by application portfolios, that there was more communication in the projects than anticipated by the task dependencies.
- **RQ2:** 
- Task assignments create the need for backchannel communication.
- We found that only 45% and 78% of the actual communication links were according to the mandated cross functional communication structure in the APP and SHIP
- In APP, mandated communication structure was restrictive of direct communication between developers and testers, as well as their communication with the RAs who were familiar with the requirements.
- Most emergent communications align with mandated cross-functional communication structure.
- **RQ3**
- Communication clusters around application domains
- Actual communication mainly takes place within the application portfolios, meaning that members communicate more within the same application portfolio than across portfolios
- People within the same application portfolio were contacted for their application domain knowledge.
- Most emergent communications seek domain knowledge within the same portfolio.
- We observed that in three of the four application portfolios there is at least one customer that emerged in the communications, indicating that project members sought customers for their domain knowledge.
- Communication brokers are boundary spanners.
- Across the four application domains in APP. An alternate explanation to the brokers’ communication across domains is that they had higher task dependencies than the other members. However,higher task dependencies alone do not lead to boundary spanning, according to Fig.2b
- **Strategies to overcome the thin spread of domain knowledge.**
    - 1. Involving new hires in training on the application domain or in reverse engineering its functionality
    - 2. Prescribing cross-functional communication structures that controlled information flow.
- Task assignments are not sufficient to explain communication in a project.
- Because application domain knowledge is spread thinly in organisations, one could easily overload the few people with application domain knowledge by involving them in many tasks.
- To prevent this overload, some team members are assigned to tasks when they do not have sufficient domain knowledge to complete them.
- Employees disregard formal structure in order to increase their productivity
- socio-technical alignment can be derived from requirements, the hierarchical control structure and the spread of domain knowledge.
- Boundary spanners are communication brokers that have domain knowledge.
- 
## Method

- Two of the authors conducted a three-month on-site observation of both project teams, inspected project requirements and planning documentation, and deployed a survey. They also attended project meetings, shadowed project members, and interviewed team members to validate our understanding. We used social network analysis to represent and analyze data about the project members and their coordination.

## Data

- We examine and contrast two projects(SHIP and APP) from a large IT organization, we use a case study method to analyze contextual information about tasks, cross-functional communication, and the distribution of domain knowledge. We use a quantitative and qualitative data collection methods
- The projects had different team configurations and the offshore locations, different distributions of application domain knowledge among its members, as well as different cross-functional communication structures
- The SHIP project team included 14 persons whereas the APP project contained 45 project members among which 25 of them were assigned to requirements examined in our study.
- In APP The dev and test leaders were the points of contact between the teams and the RAs, and no direct communication between the different roles was supported.

## Result

- Give particular attention to potential brokers by identifying members that have exceptional knowledge of the particular
application domains or components in the system.
- Communication structures should strive not only to ensure that these experts are not overwhelmed with emergent interactions,
but also to make them accessible for domain knowledge dissemination
- When the communication structure intersects with task assignments, team members will engage in backchannel communication to complete their work.
- The presence of backchannel communication is not necessarily problematic but may indicate areas where the task assignment was not congruent with either the cross-functional communication structure or the distribution of domain knowledge in the team.