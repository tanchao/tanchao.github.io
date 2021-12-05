---
layout: post
title: supertan's tech strategy
subtitle: who matters in which domain by how at what level
author: tanchao
date: 2021-07-31 16:10:10 +0800
categories: supertan
tags: supertan
---

This should be a WIP document for a while, a recent learning told me to keep climbing towards the peak without distractions, and I realized that I don't even have a solid target, so this document is trying to initial, improve and finalize my tech focus.

### Nov. 2021
* Automation at different levels, learning from "Resolve MV Conflict": 1. ask experienced SDE; 2. write a wiki on HowTo; 3. write a script GodianKnot.fix-mv-conflict; 4. integrate with code.amazon and permission to automate run updates on its own. 
  * the process, at the end, is to simulate and automate "the manual process" to solve the prolem as much as possible
* AH told me "stay ahead" so that to discover what's missing
* YS told me "own end to end" so that to solve the problem completely
* S3 stories show that "stick to highest standard at one dimension" so that it could arrive a beyond expectation stage

### Oct. 2021
* Dataflow velocity and cost could be a good design dimension to evaluate
* Design for flexibility 
** I have a plan B, why not go with plan B directly?
* Listen to Customers, but, Think ahead and offer beyond their voice. "One more thing" by Steve Jobs.

### Sep. 2021

* Security and Privacy is a concern for all existing online services
* Realtime abuse detection

### Aug. 2021

Thirdparty developer platform owner
  * effective API design (and internal system consistent maintenance following the design)
  * platform operation (boundary between infra vs partner with proper permission group configuration and operational excellence over proper granularity)
  * developer metrics monitoring and improvement (customer oriented platform)
  * feedback mechanism 
  * better sandbox (isolate side affects)

### Jul. 2021

Proficient API designer and Tier-1 Ops master, particularly on *Runtime*/*Platform* service.

### Random notes

* Terminology is an essential important setup for context. People could assume audience are having good enough context and on the same page of understanding the topics and reasoning. But, for audience not familar with the background and history, terminology clarification is the most important step to make the conversation effective and right. Lots of design doc use *Terminology* section to explain lots of abbreviations for different teams, but the key definition we need clarify are from the *Problem Statement*. The key problem area, technical challengies/complexities/blockers etc.
* Variables, more specifically, Variable's Scope. A recent design discussion helped me understand one important dimension to pay attention to is the *System Variable*, we frequently recognize the variables and arguments clearly when we write program methods, we are not at the same level of sensitivity at System level. Here is an existing data pipeline, existing data structure, let me just add a field so I can consume it somewhere elese. NOTE: what's the scope of this data structure? what's the data update frequency? who owns it who promisd the correctness of it? Are you willing to track among the pipeline when you get a bug in future? INSTEAD: could I access the data source directly from my program? so it's a variable defined in my scope and I know who is directly responsible for it instead of "plug" on other solutions.
* Focus. Stay focus is really hard, with multitasking it's harder. Not only from work but also from family, too. List the tasks with specifics and time bounded, makes it easier to narrow down the focus list. Then self-awareness whenever the attention switch. Another awareness is are we trying to solve the problem exceed the expectation, is there a value to do that?
* API
>The best APIs are usable, secure, available, fast and cheap at the same time. When necessary, we make intentional trade-offs in usability or cost to improve security, availability or performance. We strive to find a solution which satisfies all concerns.

