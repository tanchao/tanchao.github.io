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

### Jul. 2021

Proficient API designer and Tier-1 Ops master, particularly on *Runtime*/*Platform* service.

### Random notes

* Terminology is an essential important setup for context. People could assume audience are having good enough context and on the same page of understanding the topics and reasoning. But, for audience not familar with the background and history, terminology clarification is the most important step to make the conversation effective and right. Lots of design doc use *Terminology* section to explain lots of abbreviations for different teams, but the key definition we need clarify are from the *Problem Statement*. The key problem area, technical challengies/complexities/blockers etc.
* Variables, more specifically, Variable's Scope. A recent design discussion helped me understand one important dimension to pay attention to is the *System Variable*, we frequently recognize the variables and arguments clearly when we write program methods, we are not at the same level of sensitivity at System level. Here is an existing data pipeline, existing data structure, let me just add a field so I can consume it somewhere elese. NOTE: what's the scope of this data structure? what's the data update frequency? who owns it who promisd the correctness of it? Are you willing to track among the pipeline when you get a bug in future? INSTEAD: could I access the data source directly from my program? so it's a variable defined in my scope and I know who is directly responsible for it instead of "plug" on other solutions.
