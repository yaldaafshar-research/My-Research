# Do programmers work at night or during the weekend?

## Relevencies:

This paper is written to inform future approaches for automatic stress and overload detection.
[Paper's link](https://ieeexplore.ieee.org/document/8453143"To the paper")

## Take aways:

- They find that two thirds of software engineers mainly follow typical office hours, empirically established to be from 10h to 18h, and do not usually work during nights and weekend
- They found no support that project maturation would decrease abnormal working hours.
- They conclude that the use of working hours or timestamps of work products for stress detection requires establishing baselines at the level of individuals
- Psychological detachment during off-work time reduces emotional exhaustion caused by high job demands and helps to maintain work engagement
- Although worker autonomy seems to reduce the negative health and well-being effects of atypical working hours, it does not completely balance them
- Recent findings suggest that disturbances in circadian rhythm are the cause (not the effect) of depression and anxiety, and that artificial light at night increases the risk of obesity and cancer.
- Extensive use of flexible working time is linked with reduced worker productivity
- The bugginess of commits, i.e., negative effects on overall developer productivity, is related to the hour of the day (the so-called “circadian work pattern”) and to day of the week those commits have been made
- All of those buggy hours might in fact demonstrate the end of a working stint where a developer just wants to be done with the task, leading to prematurely committing the code, for instance commits made between 00:00 and 04:00 contain more bugs, while commits made between 07:00 and 12:00 (noon) contain the least
- The most defect-prone hour was 20:00
- Gender, race, type of work and income affect the likeliness of working during the weekend, Moreover, Individuals are more likely to work out of home during weekends in the winter season than in other seasons.
- They investigated the reasons for increased mortality rate in hospitals during the weekend, with explanations ranging from more seriously ill patients to less experienced staff.
- Industrial blogs on GitHub and StackOverflow report that less main stream languages such as Haskell are more commonly used during the night than languages adopted in the industry such as Java. night work is more technical

### RQ1: What are the circadian and weekly work patterns of software developers?

- There is a slight variation in activity during the week, with Monday and Friday being the least active days in all cases. Tuesday is the most active day for the Mozilla and Apache projects, while in the local company it is Thursday.
- The lowest activity for all projects happens during the night, with the number of commits starting to increase in the morning until a dip in activity happens during lunch hour.
- After lunch hour, the number of commits increases again until a decreasing trend in commits starts setting in from 4pm in all three data sets.
- The decreasing trend in the number of commits plateaus at 7pm for the Apache and Mozilla projects, while for the local company, we can see that work during the evenings is very limited compared with the Mozilla and Apache projects.
- The median start time of work across all projects is at 10:03.
- The top 10% of developers has made 88% out of all commits of our data set
- We observed that going beyond three clusters did not bring new information, instead clusters with 
- Very few individuals and high noise started to appear.
- We think that phase shift in developer’s working hours who follow office hours is due to both 
- Project culture and individual preferences, as some individuals are known as morning persons while others are not
- This suggests that clustering of individual developers may allow personalized stress or overtime detection, for at least two thirds of the developers that follow regular rhythm.

### RQ2: How does the usual work pattern vary across different projects?

- 90% of the projects have similar typical working hours. Mostly (10-18 plus/minus one hour)
- On average, only 60% of work gets done during typical working hours.
- The differences between projects in terms of relative activity happening during 8-hour work days can partially be explained by the presence of paid developers(they have activity outside office)
- The amount of activity outside office hours during the week and during the weekend are correlated. This means that both projects and developers that work a lot outside office hours are also likely to work a lot during the weekend.

### RQ3: Are office hour commits different in terms of size?

- We found no significant difference in terms of added lines of code
- In terms of commit size, we conclude that there is no difference in practice between office hours and outside office hours.

### RQ4:  Is there a difference in the developers’ work patterns over time?

 - We are interested which of these conflicting ideas, i.e., 1) starting on time with eventual delays ending up in death march versus 2) starting with a startup culture and maturing as time passes, is more prevalent in our projects.
- For 18 projects, the activity outside office hours increased by at least 5%, while for 27 projects it decreased by at least 5%.
- Most projects do not encounter a major shift of their time interval. Indeed, most projects (75/91) experienced a shift of less than one hour (X axis). Only 5 projects experienced a positive shift (towards the evening) of more than one hour, and 11 a negative shift (towards the morning) of more than one hour.
- For those companies which had a positive shift, the amount of work done outside these 8-hour periods didn’t change a lot and is relatively high
- Overall, we did not find any correlation between the amount of office hour work and shift of office hours period.
- Most projects do not experience large changes over time in their work pattern. Important changes in the identified 8-hour office hour period are often found in projects with commits being more spread throughout the day. **Fig8**

### RQ5:  Are office hour commits different in terms of content?

- Developers back out more code themselves outside office hours
- After office hours, a developer is backing out changes herself rather than being backed out by some authority.
- The “closed tree” message is proportionally more common outside office hours when we remove the commits where it appears together with the “Backed out changeset” message
- Work involving adding something is more common during office hours while removals and fixes are more common outside office hours. **Table2**

### RQ6: Can demographics explain office hour activity? We investigated whether there was a correlation between the number of commits made by a developer and the amount of abnormal work.

- We did not find a statistically significant correlation between developer seniority and amount of office hour work
- Outside office hour work is mostly performed by unpaid developers.
- Paid developers work less outside office hours than unpaid ones. Yet most paid Firefox developers still work significantly more outside office hours than developers from the local company. **Table3**
- It seems that career moves on the technical ladder, i.e., having a title with the word “senior” or “principle”, decreases the median office hour work by 1.9%. However, career moves on the managerial ladder, i.e., having a title with the word “manager”, decrease the outside office hour commits by 4.5% but again the differences are not statistically significant. We suspect that management positions require less technical work and more communication and coordination, which might explain this difference.
- For managers, using commits as working hour indicators could be misleading

### conclusion

- Two thirds of individuals mostly follow office hours. This information is important if one wishes to build a stress detector that would use among other things commit hours, since such a detector would only work for the two thirds of software engineers who have regular working rhythms.
- With respect to seniority we found no differences in working hours by using two different measures the number of commits and job title. 
- Perhaps developers that make very few commits are hobbyist and commit outside office hours while for the most senior developers the outside office hour commits would be explained by overwork.

## Data:

- They acquire data by studying the software engineers’ working hours and investigating the time stamps of commit activities of 86 large open source software projects, either projects with many hired resources (Mozilla) and those without (Apache Foundation), as well as in a (local) Finnish IT company, both containing hired and volunteer developers. Each of these companies have a minimum of 2,000 commits

### Data about night work:

- (Quora question with over 100 answers and over 500,000 views on why developers love night work 
- Entire book with 2,500 paid readers on the topic, written by an industrial programmer 
- Stack overflow analysis with 3,800 Facebook shares and 91 comments of day-night differences )
- Wang et al. examined work patterns of scientists by looking at the amount of scientific papers being downloaded on different days. Scientists work 60-70% as much of their time during the weekend as during the week. Time worked during weekends differs by country: scientists work proportionally more during weekends in China than in the USA and Germany.
- We mined development data from the Git and Mercurial repositories of Mozilla1 and Apache2 and of a local company’s product.
- The local company’s product contained more than 20,000 commits from nine developers. We have visited the company several times to ensure the validity and usefulness of our work. We then wrote custom scripts to extract the list of commits (code changes), associated timestamps and authors from all code repositories.

## Methods:

- K-means clustering and a dynamic search of office hours instead of a static heuristic. For clustering purposes, we computed the relative share of commits made by each hour of the week by each developer(168 elements). We tested values of k (i.e., the number of clusters) from 2 to 7.
- We used the GrimoireLab tools to extract issue comments from Mozilla’s Bugzill repository
- We linked commit messages to the corresponding issue report by looking for an issue
identifier in a given message
- We only considered commits starting from the first commit with a timezone different than UTC (i.e., the first commit that is clearly made after the import from the old system
•Data extraction method: to study the work patterns of individual developers we performed a basic merging of the different authors’ identities.
- In order to study the work patterns of individual developers, we performed a basic merging of the different authors’ identities. We first cleaned the name and email used in the version control system’s author field. Then we grouped together identities using the same name or email addresses. Finally, two of the authors manually checked the result in order to avoid any false positive.

- **RQ1:** To determine the working period for each of our projects, we searched the week day for the eight-hour stint that covers the largest share of commits in a day. First, for a given project, we computed all the (HH,mm) tuples representing a timestamp (in 24 hour format) for which at least one commit was made during a weekday. For each (HH,mm) tuple, we computed the number of commits made during the 8-hour interval [(HH,mm), (HH+8,mm)[. We then selected the interval with the highest number of commits as the 8-hour office period of the considered project.

- **RQ2:** Clustering allows the separation of projects based on work Patterns: We again used k-means clustering (with k = 7) by the hour of the week. The difference is that here we cluster by project (n=87) while previously we clustered the top 10% individuals (n=1,108)

- **RQ3:** In this paper, we approximate the dichotomy of office hours versus non-office hours using our dynamic office hour detection approach, which ensures that, for each project, only the most active weekday hours are taken into account as office time.

- **RQ4:** For each project, we split the activity history in two equal parts (in terms of number of commits) in order to find whether the work pattern changed over time or not

- **RQ5 :** By comparing word clouds

- **RQ6:** We only considered individuals with 10 or more commits, which reduces the number of analyzed individuals in Firefox significantly from 2,755 to 857, but still retains 98% of the commits.
- We ran a manual background check for the top 10% of developers to determine whether they are paid or non-paid. Our background check considered information available online on websites such as LinkedIn or the developers’ personal websites (e.g., publicly available CVs). In addition to their job status, we also gathered information about their location, experience in the software industry and position at Mozilla

## Refrences:

- They referenced to 34 articles.