---
layout: post
title: "Beyond the Code: Teaching My Agent to Doubt Itself"
date: 2026-07-27
categories: beyond the code
---

In my last two posts I talked about the macro risks of AI and what it's doing to team velocity. This one is smaller and more personal. It's not a thesis. It's a log of what happened when I actually started building agents myself, in order, mistakes included.

---

## Chocolate First, Obviously

The first agent I ever built had nothing to do with work. I wanted to know when a specific chocolate came back in stock, so I built something to check for me.

For the record: still out of stock. The agent works fine. Apparently, the chocolatiers do not.

It was a small, low stakes project, and that's exactly why it was the right place to start. Clear success condition, nothing riding on it if it broke. If you're thinking about building your first agent, don't start with something important. Start with something you don't mind failing.

---

## Then I Used One to Win an Argument

The second time I reached for an agent, it was for something more specific. Someone told me I had never sent an email about a particular topic. I was fairly sure I had. So I had Claude go dig through my inbox and find it.

It found it. I was right. I had the receipts, literally, and I could point to the exact email, exact date, exact recipients.

That's a small thing, but it's a real thing. It's the kind of task that used to mean twenty minutes of manually scrolling and searching, hoping you remembered the right keyword. Now it's a question you ask and get an answer to. The more useful version of this, the one I'm still refining, looks at recent email and tries to surface what actually needs my attention. Did someone ask me to do something? Research something? Follow up with someone? That's a genuinely useful problem, and it's a good example of what agents are actually good at right now: not doing the work, but telling you which work exists, or in this case, which work already happened.

---

## The Real One: Teaching an Agent to Grade Its Own Confidence

The most complex agent I've built so far started as a simple quality check on our team's work-tracking system.

A lot of tickets get filed without solid acceptance criteria, without clean repro steps, without enough context for someone to actually pick them up and go. So I built an agent to read a ticket and score how well formed it is. Good acceptance criteria, clear description, reproducible steps, that kind of thing. If the ticket is weak, the agent flags it and writes a comment back to whoever filed it explaining what's missing.

That part alone was useful. But it didn't stop there.

The natural next question was: once a ticket is well formed, can the agent look at the actual codebase and figure out whether it understands what needs to change? So I extended it. Now, for well formed tickets, the agent goes into the code, compares what it finds against what the ticket describes, and generates a second confidence score, this time on whether it actually understands the fix.

And from there, it kept evolving. For the narrow set of cases where that second confidence score is high enough, under close supervision, I've started letting the agent draft the actual change.

I want to be clear about what I'm not doing. I am not letting this thing run wild across a codebase fixing whatever it wants. Every step has a human checkpoint, and the checkpoints got more rigorous as I built the system, not less.

**The most interesting thing I've found is that the agent's confidence isn't stable, and that instability is the most useful signal I have.**

One ticket was originally rated at 85% confidence based on the ticket text, but after the agent looked at the code it dropped that to 50%. That drop is the system working correctly. That's the agent telling me "I thought I knew, and then I looked closer, and I don't." I'd rather have an agent that gets less confident when it hits real complexity than one that stays confidently wrong.

So now there are effectively three passes: read the ticket, read the code, then go back and re-check the ticket against what it just learned from the code. Three chances for the confidence score to move, and three chances for a human to catch it before anything ships.

For the narrow set of high confidence cases where the agent does draft a fix, it doesn't stop at the code. It also writes the automated tests to go with it and puts together documentation for QA explaining what changed and how it was tested. If I'm going to trust a change enough to let it near production, I want the proof of that change sitting right next to it, not left for someone else to reconstruct later.

---

## Where I Am Right Now

Still fleshing all of this out. Still cautious, on purpose. The goal isn't to remove myself from the loop, it's to build something that gets a little smarter and a little more honest about its own uncertainty every time I add a check.

If I'm honest, the guardrails were never really about controlling the agent. They're about getting me to a place where I can actually trust it. Confidence is the real goal here, mine, not just the score the agent prints out. The checks are how I earn that. There will always be more to add. This isn't a project with an end state, it's a constant, iterative process, and I expect it to stay that way for a while.

It's a strange thing to say about a piece of software, but the version of this agent I trust most is the one that's willing to change its mind.

If you're building agents into your own workflow, I'd love to hear where you've put your checks, and where you've found the confidence scores lie to you.
