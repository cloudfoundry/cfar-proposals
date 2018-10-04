
### Application Runtime Proposal Template
___

##### Created: MM/DD/YYYY

##### Owner:  

##### Work-Group:  

##### Status: WIP | In Review | Approved | Obsolete

##### Release Version: N/A

##### Reviewers: xxxx[ ], xxx []

##### Approvers: xxx [], xxx []

##### Short self link: https://goo.gl/fAFwgT

___
#### 1. Summary (what is this document about?)

<role> wants to <use this feature> so that <problem they have is solved>.

Portfolio Epic Label: <common epic label tagged to applicable stories across teams’ backlogs in order to improve our ability to predict when we will solve this problem>

Contributing Teams:
<List of teams required to contribute in order to achieve the Feature Narrative + summary of their scope/responsibilities>


Useful Links:
<any useful links pin at the top>


#### 2. Problems this Feature Narrative Solves

Summary of which user or buyer persona has this problem and what the problem is.

Real-world examples of potential and actual customers who have this problem.


#### 3. Community Goals (why do this and by when?)

<define any community goals this feature narrative is intended to achieve such as:>

<How it aligns with community’s goal to deliver continuous quality>
<How it helps promote the common business interests of users, operators, and providers of CF technology>
<How it helps provide value and promote innovations to users, operators, and providers of CF technology>

<define the degree to which there is a time criticality to deliver this and why>


#### 4. Product Goals (what solution will we implement?)
Solution Description
<Introduction of the solution we want to deliver for context>

User Workflows
<Summarize workflows that describe each relevant user persona’s goals and tasks to achieve the goal>

<user1 can achieve workflow goal x>
<user’s first task to achieve this goal>
<user’s Nth task to achieve this goal>

<user2 can achieve workflow goal x>
<user’s first task to achieve this goal>
<user’s Nth task to achieve this goal>

Feature Epic(s)
<Describe the feature epics team will work on to achieve the workflows above>
Team 1
<One sentence summary of Epic #1>
<One sentence summary of Epic #2>
Team 2
<One sentence summary name of Epic #1>

Anti-Goals
<Describe any anti-goals to be avoided>


#### 5. Risks and Unknowns

<list any serious risks and mitigation strategies that have a meaningful effect on ensuring success of this Feature Narrative>
<list steps required to resolve unknowns that block the work from starting>
<things to consider: examples: how does this affect our security posture? How should we consider user privacy as we build this feature?


#### 6. Quality and Maintainability Plan

<list any quality requirements specific to the feature and strategies (beyond standard TDD / XP practices) that will have a meaningful effect on ensuring quality and maintainability once delivered. Some standard considerations include:>

Burn-in - Will the feature be deployed to a long lived web services environment or customer-facing deployment prior to delivery ? 
Load Testing - Have we run this at increasing levels of load, ideally we want to get to the edges of the product before our customers do?
Performance Testing - Coupled with above, do we see any performance degradation when at this level of load?
Upgrades / Deployments - Have we validated that zero downtime is working? that applications successfully move / rebalance & perform the expected behavior
Backup / Restore - If this is needed have we built it, fire drilled it and tested continuous restore?
Operations - How does an Operator (or other applicable persona) know...
how to operate this feature? 
when it is broken? 
when it is performing badly? 
Failure Modes - How could the feature / product fail in customers’ production environments or cause other CF components to fail?

<list any measures / metrics that indicate success upon delivering the feature>


#### 7. Feedback from Customers and Stakeholders (How do we know if this is successful in solving the problem?)

<Note down observations / feedback from customers, PMM, sales/FEs, engineers on relevant teams, other PMs, foundation, etc..>

<Note down by what measurements will we know if we were successful in solving the problem or not>


#### 8. Scoping Estimate

<An area to summarize the estimated scope of work in terms of time.  Please estimate whether each item is more likely to be a day, a week, a month, 3 months, 6 months or a year.>
