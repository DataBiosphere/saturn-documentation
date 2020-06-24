#Team Saturn Principles and Processes

##Team principles

We value and respect each other as people, and as colleagues.
We trust each other to act with care and skill when fulfilling our roles.
Our primary goal is to deliver value to users by understanding their needs and helping them solve problems.
We believe that the best way to serve users is by listening to them directly, and providing rapid, iterative improvements to the system.

##Definition of ready

Tasks are considered ready when:

* The team generally understands the underlying problem that users are facing, as well as any relevant context.
* The team generally understands the proposed solution, and how it will address the problem (or, if a solution is not readily available, understands that the task is to explore and come up with a way forward).
* The proposed solution is immediately actionable by the team.
* The team generally understands the cost of the proposed solution, in terms of difficulty, time, and risk.

"General understanding" provides for some flexibility based on the task. For example, it might mean that the whole team discussed the issue in depth and came to a consensus. Alternatively, it could mean that there is one person with a solid understanding of the issue, and the rest of the team trusts their judgement.

##Definition of done

Tasks are considered done when:

* The solution has been fully delivered and is actively providing value to users.
* The team has thoroughly tested the solution and verified that it works as intended.
* If the task was modified or split up into separate tasks during development, those changes are recorded.

##Definition of quality

The team holds software to the following standard of quality:

* Provides value: Software should provide leverage to users, enabling them to solve problems that they are facing, and/or make decisions related to their goals.
* Meets people where they are: Software should be accessible and approachable. It should aim to increase users’ understanding with documentation and clear, simple interfaces. It should offer reduced friction for advanced users.
* Behaves predictably and consistently: Software should aim to minimize surprise and frustration. It should have reasonable performance, and avoid unexpected errors. When there are changes, they should be clear and obvious.

##Delivering code

There are two roles involved in the development process: developers and reviewers. Anyone on the team can serve in these roles for a task, and any given task may have multiple developers and/or reviewers. Reviewers for a specified task should generally not be people who were also developers for that task, unless the whole team was involved in development.

1. The developers write code on a separate branch, independent of other development.
2. Throughout the process, the developers validate the solution, explore any open questions, and make adjustments as necessary.
3. The developers thoroughly test the new code, as well as any adjacent code that may be affected.
4. When finished, the developers submit a pull request for review by the team.
5. The reviewers thoroughly test the new code, as well as any adjacent code that may be affected.
6. The reviewers thoroughly read the code, and submit comments to request fixes or improvements.
7. The developers respond to comments, submitting changes as needed. The comment/response cycle may go through several iterations.
8. When finished, the developers merge the code into the main branch, provided:
9. All comments have been addressed (note that not all comments require changes)
10. The PR has at least one explicit approval

##Deploying code

The team generally deploys services on a continuous basis, as changes are made. This helps to deliver value quickly and efficiently, and also address user-facing problems as soon as they are discovered.

The team utilizes periodic, automatic deployment processes, as well as manual deployment processes, depending on the service.

Team members are generally entrusted with the ability to deploy services on-demand, and given training in doing so judiciously. (TODO: link to training document)

The team uses automation and technological safeguards as appropriate to help ensure that the intended practices are followed.

##Handling emergencies

Emergencies are defined as situations when:

* User value is severely degraded, and
* Not taking action would be substantially more risky or damaging than taking immediate action

For example, suppose that on Saturday morning, a lone teammate is notified of a critical bug in a service that prevents any user from using the system (degraded value). The teammate understands the problem, and is confident that fixing it would be straightforward (low risk). Leaving the system alone would prevent anyone from using it until Monday (more damaging). This qualifies as an emergency situation.

In emergency situations, teammates may make some modifications to the usual processes:

* Teammates may review their own code, instead of seeking external review. This should be done with extra caution, and treated as a real review, not a short-circuit of the review process.
* Teammates may merge code without receiving an approval. This should only be done for simple, highly focused fixes to the problem at hand.
* Teammates may use the manual deploy process to deliver fixes to users.

