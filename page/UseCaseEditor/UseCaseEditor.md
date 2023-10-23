---
layout: page
title: Use Case Editor
permalink: /UseCaseEditor/
---


# Use Case Editor主要结构：

   The natural language compiler consists mainly of use case descriptions, which we will present in the form of user stories. Users can refine the use case descriptions into four parts when writing requirements:.
1. User Story \ Pre and Post Conditions: This part mainly describes the user story and the pre and post conditions of the user story.
2. Basic Process: This section is mainly presented in the form of EARS, in which the user can describe the current requirement as a user requirement or a system requirement and the order of execution between them.
3. Extended Processes: the main content of this part of the writing, in the current use case, in the case of encountering special circumstances, the system should make how to act.
4. Non-Functional Requirements: This section describes the non-functional requirements of a single user story.

<img src="/imgs/UseCaseEditor-project/UCE2.png" />

## User Story \ Pre and Post Conditions：

   This section takes the form of a basic user story as a <User Persona>, I want to <Complete Activity>, in order to <Realise Value>. Both preconditions and postconditions are optional, and different preconditions and postconditions can be replaced by ". "Spaced out.
The red fields in the case are required and the purple fields are optional.

<img src="/imgs/UseCaseEditor-project/US.png" />

## Basic Process

<img src="/imgs/UseCaseEditor-project/BP.png" />
   This part of the basic EARS form, this part of the overall optional, when the need for an internal description of the use case to fill in, which NUM. after the need to express the current needs of the user needs or system requirements (User / System), in addition to the case of the red field is required, the purple field is optional.
<img src="/imgs/UseCaseEditor-project/BP2.png" />

## Extended Processes

<img src="/imgs/UseCaseEditor-project/EP.png" />
This section uses a basic form of natural language description to supplement the details of the requirements. In addition, the red fields in the case are mandatory and the purple fields are optional , supplementing the details.



### (Method of numbering)
<img src="/imgs/UseCaseEditor-project/EP2.png" />

### (User and System)
<img src="/imgs/UseCaseEditor-project/EP3.png" />

## Non-Functional Requirements
<img src="/imgs/UseCaseEditor-project/NF.png" />

### EARS
   在软件工程中，NL需求文档中可能 出现的一些问题：歧义、模糊性、复杂性、重复、需求的不恰当、不 可测试性。为了消除这些问题，引入了半结构化的自然语言Easy Approach to Requirements Syntax（EARS）。EARS是半结构化自然语言，相对简单，易于学习。EARS是一 种使用五个简单模板编写SRS文档的方法。 
#### Ubiquitous requirements(普遍存在、无处不在的)
没有任何先决条件或触发器。它不会由在系统检测到的事件或处于定义的系统状态而调用，但它是始终处于活动状态。syntax : The (system name) shall (system response)
例子:“The control system shall prevent engine overspeed”控制系统应防止发动机超速

#### Event-driven requirements(事件驱动)
只有当在系统检测到触发事件发生时，系统才有的响应。关键字“when”用于事件驱动的需求。syntax :WHEN (optional preconditions) (trigger) the (system name) shall (system response)
例子:“When continuous ignition is commanded by the aircraft, the control system shall switch oncontinuous ignition”当飞机发出连续点火指令时，控制系统应接通连续点火开关。

#### State-driven requirements(状态驱动)
当系统处于定义的某个状态时，系统才有的响应。syntax : WHILE (in a specific state) the (system name) shall (system response)
例子：“While the aircraft is in-flight, the control system shall maintain engine fuel flow above XXlbs/sec”当飞机在飞行中，控制系统应保持发动机燃油流动在XXlbs /sec 以上.

#### Unwanted behaviour requirements(不想要的行为需求)
涵盖所有不良情况。这包括故障，干扰，与所需用户行为的偏离以及交互系统的任何意外行为。不想要的行为是早期需求遗漏的主要来源，因此需要进行昂贵的返工。使用关键字If和Then来指定不想要的行为。syntax : IF (optional preconditions) (trigger), THEN the (system name) shall (system response) 
例子：“If an invalid credit card number is entered, then the website shall display “please re- enter credit card details.” 如果输入的信用卡号码无效，则网站将显示“请重新输入信用卡详细信息”。

#### Optional feature requirements（可选的特性需求）
在系统中，用于指定特性，用关键字Where表示 syntax : WHERE (feature is included) the (system name) shall (system response)
例子: “Where the control system includes an overspeed protection function, the control system shall test the availability of the overspeed protection function prior to aircraft dispatch.” 例子：控制系统包括超速保护功能的，控制系统应在飞机调度前测试超速保护功能的可用性。

  <img src="/imgs/UseCaseEditor-project/EARS1.png" />
