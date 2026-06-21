---
layout: post
title: "The risks to AI as I see it"
date: 2026-06-21 10:00:00 -0700
categories: general
---

Everyone is asking what AI will do *to us*. Almost no one is asking what we’re doing *to AI* , and the risks we’re creating as we rush head-first into automation. I’ve leaned heavily into AI myself, and I’ll say the quiet part out loud: the version of software engineering we grew up with is gone. Something new is emerging, and it’s moving faster than most organizations can absorb.

As I watch this transition unfold from inside an engineering leadership role, three risks stand out.

---

There’s a lot of debate about whether AI will “take your job.” From what I’ve seen, the honest answer is yes , at least for a significant portion of white-collar roles. The adoption curve is nothing like the industrial revolution. This is happening in quarters, not decades.

The deeper risk isn’t just job loss. It’s the structural strain on the systems that keep society running. Governments rely heavily on payroll taxes from high-earning knowledge workers. If companies aggressively automate those roles, that revenue evaporates. Policy ideas like UBI sound clean on paper, but the fiscal gap they’d need to fill is enormous.

There’s also a popular belief that blue-collar jobs are “safe” because AI can’t swing a hammer. But that ignores basic economics. White-collar workers fund blue-collar demand. If a $180k PM loses their job, they’re not remodeling their kitchen. Multiply that across an industry and you get:

* **Less demand** for contracting and skilled trades  
* **A sudden influx** of laid-off workers entering trade schools  
* **Oversupply** in a shrinking market  
* **Downward pressure** on wages and stability  

Everything is connected. When one tier collapses, the others feel it.

---

## 2. The First-Quarter Budget Burn  
### *Vendor Lock-In and Unmonitored AI Spend*

A pattern is emerging across the industry: companies burn through their entire annual AI budget by Q1 because they scaled too fast without understanding token and compute economics.

The bigger danger is architectural. Entire verticals are building products that are essentially wrappers around a single foundation model. When your business depends on one engine (Claude, GPT, Gemini, whatever), you’ve surrendered all pricing power. If that provider raises prices, you either:

* **Eat the margin loss**, or  
* **Pass the cost** to customers who are already tightening budgets  

That’s not a strategy. That’s a trap. Vendor lock-in isn’t new, but the speed and depth of dependency in the AI era is unprecedented. Companies are building on sand without realizing it.

---

## 3. Security at AI Speed  
### *Bad Actors Don’t Wait for Governance*

Security teams move on quarterly roadmaps. Attackers move on minutes.

Bad actors are already using AI to automate vulnerability discovery at a pace human teams can’t match. The organizations most at risk aren’t the highly regulated giants , they have guardrails, audits, and paranoia baked in. The danger is in the mid-market:

* **Boundary Issues:** Teams rushing AI into production without data boundaries  
* **Data Leaks:** Shadow-AI usage leaking sensitive information  
* **Lack of Audits:** AI-generated code deployed without verification  
* **Exploit Mutation:** Attackers using LLMs to mutate exploits faster than patch cycles  

The weakest link won’t be a Fortune 100. It’ll be the company that adopted AI for speed without adopting the security discipline to match it.

---

## Looking Forward

I don’t pretend to have the macro-economic answers. But I do see the operational reality up close: AI is accelerating the volume of work, not reducing it. Leading an engineering team through this transition has made one thing clear: we need new tools, new processes, and new ways of thinking to manage the velocity we’ve unleashed.

This will likely become a multi-part series as I continue mapping what’s breaking, what’s working, and what leaders need to prepare for as AI reshapes the industry in real time.