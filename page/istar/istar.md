---
layout: page
title: Goal2UCM
permalink: /istar/
---

## Goal2UCM
### iStar Metamodels
In istar2.0, Actor is divided into two types: role- the abstract description of the behavior of social Actors in a specific environment or field. Agent- an Actor with concrete entity representation.

Actors are often interrelated. In ISTAR 2.0, two different types of connections are defined.
Is-a: represents the concept of generalization / specialization in ISTAR 2.0. Only Role can be specialized as Role, or general Actor specialized as general Actor.
Participants-in: represents any type of association between two Actors, not generalization / specialization. This association is not limited by the type of Actor.

The target elements are elements required by the Actor. Therefore, they have different types and are the core of ISTAR 2.0. Connected with an Actor in the aggregate relation “wants”, it indicates what the Actor wants. In this section, we will explain four types of target elements:
Goal: the state that Actor wants to achieve, and there is clear achievement standard.
Quality: the attribute that Actor wants to achieve to some extent.
Task: refers to the action that Actor wants to implement, usually to achieve a goal.
Resource: the physical entity or information entity that the Actor needs to execute a task.

Dependency is the dependency relationship between an actor and intentional elements. This section describes the relationship between these five parameters. However, the Depender and Dependee in a dependency relationship should not be the same actor:
Depender: An Actor that depends on a certain “dependum” to provided.
Dependermt: it is the target element in “depender”, which explains the reason for the existence of dependency.
Dependee: it is an Actor that should provide “dependum”.
Dependeelmt: it is the target element in “dependee”, which explains how the “dependee” Intends to provide the dependency.
Dependeelmt: it is the target element as a dependency object.

Refinement relationship links Goal and Task hierarchically. Refinement is an n-element relationship that associates a parent object with one or more child objects. The target element can only be the parent element in at most one optimization relationship. And: represents the logical AND relationship, with at least two or more child elements. Or: represents the logical OR relationship and has at least one child element.

Contribution represents the impact of the Intentional Elements on quality. Quality itself cannot provide a contribution.
Make: the source provides sufficient positive evidence for the satisfaction of the target.
Help: the source provides weak positive evidence for the satisfaction of the target.
Hunt: the evidence provided by the source is insufficient to prove that the target is satisfied (or denied).
Break: the source provides sufficient evidence to prove that the target is satisfied (or denied).

Qualification relationship can associate quality with other target elements (task, goal, or qesource). It can limit other target elements.

Neededby relationship links a task to a qesource, indicating that participants need resources to perform the task.


**iStar Metamodel：**
![image](https://user-images.githubusercontent.com/49606429/134271842-f02e85a4-03e3-4dfb-b02f-40bc453e1c97.png)

### UML Metamodels

In this article, we will mainly use the UseCasaModel part to explain. The UseCaseModel is also divided into two parts. The first part is the use case diagram. The main elements here are Actor and UseCase. These two elements are connected by uc to obtain the basic use case diagram. The second part is the system sequence diagram. This part is mainly composed of Interaction and some elements that have an aggregation relationship with it. They are Message, Execution, and Combined Fragment respectively. They describe when a use case enters the system sequence diagram, the beginning of each Task, the end, and the cycle and selection process that may exist in between.
