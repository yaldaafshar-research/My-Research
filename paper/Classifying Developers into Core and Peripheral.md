# Classifying Developers into Core and Peripheral: 
# An Emperical Study on Count and Network Metrics 

## Relevencies:

[Paper's link](https://ieeexplore.ieee.org/document/7985659")
- We investigate whether count-based operationalizations of developer roles produce consistent results, and we validate them with respect to developers’ perceptions
- We identify structural and temporal patterns in the project’s organizational structure that operationalize core– peripheral roles using network-analysis techniques, referred to as the network-based operationalizations.

## Take aways

- Classification of developers into core and periherial is besed on simple counts of individual developer activities (e.g., number of commits), which has a threat to validaty
- Classification of developers into core and periherial is based on simple counts of individual developer activities (e.g., number of commits), which has a threat to validaty
- One common approach is to apply thresholding on the number of lines of code contributed by each developer, but this could result in incorrectly classifying developers who just make large numbers of trivial cleanups.
- A very small fraction of developers is responsible for performing the majority of work
- Core developers play an essential role in developing the system architecture and forming the general leadership structure, and they have substantial, long-term involvement. In contrast, peripheral developers are typically involved in bug fixes or small enhancements, and they have irregular or short-term involvement
- We recognize inter-developer relationships to be of primary importance for the operationalization of developer roles.
- Regarding social characteristics, core developers have substantial communication ties to other core developers, especially in projects with a small developer community
- Regarding technical characteristics, core developers typically exhibit strong ownership over particular files that they manage, they often have detailed knowledge of the system architecture, and they have demonstrated themselves to be extremely competent
- The top 20% of contributors are responsible for 80% of the contributions)
- We identified three variations of count-based operationalizations of core–peripheral roles:(Commit count, Lines of code (LOC) count, Mail count)
- **comit count:** Core developers typically make frequent contributions to the code base and should, in theory, achieve a higher commit count than peripheral developers
- **Lines of code (LOC) count** follows a similar rationale as commit count. A potential source of error is that developers writing inefficient code or changing a large number of lines with trivial alterations (e.g., whitespace changes) could artificially affect the classification.
- **Mail count:** This is still only a very basic metric because a developer answering many questions and one asking many questions will appear to be similar, and there is no inter-developer information, so who is speaking with whom or with how many people is completely
ignored.
- **Practical opportunities for network insights are, for example:** 
    - 1. Identifying core developers that are overwhelmed by the peripheral developers they need to coordinate with
    - 2. Structural equivalence (that is two nodes with the same neighbors) could reveal which core developers have similar knowledge or technical abilities, which helps to determine appropriate developers for sharing or shifting development tasks
    - 3. Structural holes between core developers may indicate deteriorating coordination; or a single globally central core developer may indicate an important organizational risk.
- Intuition and prior research led us to the conclusion that the role a developer fulfills can change over time 
- ### five network-based operationalizations that are rooted in the structure and evolution of developer networks
    - **1. Degree centrality:** It represents the number of ties (edges) a developer has to other developers. The expectation is that core developers
then have a larger degree than peripheral developers.
    - **1. Degree centrality:** It represents the number of ties (edges) a developer has to other developers. The expectation is that core developers then have a larger degree than peripheral developers.
    - **2. Eigenvector centrality:** Represents the expected importance of a developer by either connecting to many developers or by connecting to developers that are themselves in globally central positions. We expect core developers to occupy globally central positions in the developer network.
    - **3. Hierarchy:** In a hierarchical network, nodes with high degree tend to have edges that span across cohesive groups, and we expect core developers to play a role in coordinating the effort of these communities of developers. 
    - **4. Role stability:** A temporal property of how developers switch between roles. As core developers typically attain their credibility
through consistent involvement and often have accumulated knowledge in particular areas of the system over substantial time periods, we expect core developers stability in the developer network to be higher than for peripheral developers.
    - **5. Core–peripheral block model:** The block model specifies the core–core region of the matrix as a 1-block (i.e., completely connected), the core–peripheral regions as imperfect 1-blocks, and the peripheral– peripheral region as a 0-block
- Overall, the results demonstrate that the count-based operationalizations largely produce consistent results regarding the classification of developers into core and peripheral groups. We therefore accept H1.
- Developers in a core state are substantially less likely to transition to the absent state (i.e.,
leave the project) or isolated state (i.e., have no neighbors in the developer network by working exclusively on isolated tasks), in comparison to developers in a peripheral state.
- The core developers represent a more stable group than peripheral developers.
- The network-based operationalizations illustrate clear manifestations of core and peripheral developer roles that agree with the abstract characteristics established by earlier empirical work. We also found evidence in terms of the core–peripheral block model that developer roles imply specific coordination preferences. On the basis of these results, we accept H2 and H3. 
- Overall, the results indicate that the network-based and countbased operationalizations are mostly consistent. While the agreement is imperfect, the results show that the divergence from perfect agreement is similar what is seen among the count-based operationalizations. We therefore accept H4.
- Time plays a central role in the developer-advancement process
- Core developers will exhibit globally central positions, relatively high positional stability, and hierarchical embedding.
- Core developers have a preference to coordinate with other core developers; peripheral developers have a preference to coordinate with core developers instead of other peripheral developers.
- Peripheral developers are twice as likely to coordinate with core developers as opposed to other peripheral developers.
- The strength of agreement between all operationalizations significantly exceeds what is expected by chance.
- In general, the mailing list is most accurate in capturing characteristics that reflect developer perception of roles. However, in many projects communication archives are not available, and in this case, a network perspective on version control system data can closely resemble the insights (regarding developer roles) provided by the communication archive. Overall, we see that a network perspective always improves the
agreement with developer perception over the simpler countbased operationalizations. To this end, we accept H5.
- Developer roles are often defined in terms of differences in the mode of interaction between developers. Core maintainers participate in discussions on areas outside the ones that they maintain.
- Core developers are likely to occupy upper positions in a hierarchy, as they provide coordination bridges between the peripheral developers that have a comparatively narrow focus.
- We see that agreement between operationalizations defined on same data source typically have substantial agreement
## Method

- **Count-based operationalization:** We apply the standard 80th percentile threshold.
- **Network model:** We analyze multiple contiguous periods over one year of a project in question using overlapping analysis windows. Each analysis window is three months in length, and each subsequent analysis period is separated by two weeks because developer role changes over time. Beyond three months window size, the development community does not change significantly, but temporal resolution in their activities is lost 
    - **1. E-mail networks:** For a given project, we download the mailing lists archives either from gmane using nntp-pull or directly from the project’s homepage to obtain an mbox formatted file containing all messages sent to the mailing list. We apply several preprocessing steps to remove duplicated messages, normalize author names, and organize the mails into threads using the Message-IDs and In-Reply- To-IDs. Furthermore, we decompose the From lines of each mail into a (name, e-mail address) pair. To construct a network representation of developer communication, we apply the standard approach, where edges are added between individuals who make subsequent contributions to a common thread of
    communication. 
    - **2. Version-control-system networks:** Data in version-control systems are organized in a tree structure composed of commits. We analyze only the main branch of development. we analyze only the authors of commits, not the committer. we count total lines of code(the sum of added and deleted lines.)
- **Role stability:** We operationalize developer stability by estimating the probability that a developer in a given role leaves the
project by not participating for, at least, three months. For each developer the role during each development window is determined using the degree-centrality operationalization. The time-ordered sequence of roles for each developer is then used in a maximum-likelihood estimation to solve for each state transition parameter (e.g., the probability that a core developer transitions to a peripheral role)
- **Developer Perception:** we asked developers to report the roles of developer’s in their project according to their perception(developers who have knowledge of the project state)
- **Core-periphery block model:** we must compute the edge-presence probabilities for core–core, core–peripheral, and peripheral–peripheral edges. If the edge-presence probabilities are arranged according to, pcore–core > pcore–periph > pperiph–periph
- **Developer Perception vs. Network-Based and Count-Based Operationalizations:** we computed the number of core and peripheral votes for each developer from the survey responses (see Section V-D). For each developer, we chose the role with the highest number of votes as the ground truth and, if the count was equal, the developer was removed.
- **Network-based vs cout-based agreement:** Agreement was computed for 163 ground-truth samples provided by the survey participants. Three participant responses were eliminated because they were incomplete.
- 
## Data
- By surveying 166 developers,they achieved 982 samples and propose a relational perspective on developer roles, using fine-grained developer networks modeling the organizational structure, and by examining developer roles in terms of developers’ positions and stability within the developer network. 
- By studying 10 substantial open-source projects, over at least one year of development, with data from two sources (version-control system and mailing list), we evaluated count-based operationalizations.
- The projects vary by the following dimensions: (a) size (source lines of code from 50KLOC to over 16 MLOC, number of developers from 15 to 1000), (b) age (days since first commit), (c) technology (programming language, libraries), (d) application domain (operating system, development, productivity, etc.), (e) development process employed.
- For the remaining 9 projects(one project was excluded), we sent recruitment e-mails to 3369 addresses of which 166 elicited a complete response. In total, we obtained 982 role classifications
## Result
- Core developers exhibit high positional stability, upper positions in the hierarchy, and high levels of coordination with other core developers, which confirms assumptions of previous work.
- The networkbased operationalizations are more reflective of developer perception than the count-based operationalizations.
- Positional stability, hierarchical embeddings, and interaction patterns between core and peripheral developers can not be explained in count-based operationalization.
## Refernce
They referenced to 34 articles