---
layout: post
title: "Beyond the Code: The Brain in the Application"
date: 2026-08-03
categories: beyond the code
---

A friend and I were talking recently about what AI has actually changed in development. We’re not starting at `step[0]` anymore. We’re starting at `step[10]`, moving straight past the manual heavy lifting to focus on architecture, context, and intent.

That new starting line changes how we maintain software, too. When developers tell me, *"If you vibe code, somebody behind you is going to have to debug your vibe-coded slop,"* they're missing the point. It won’t be a person combing through generated syntax line by line. It’ll be AI, directed by a person, analyzing the code, understanding it, and fixing it.

Software engineering is changing, the same way furniture making changed once factories and machine tools took over what used to be entirely hand work. Furniture is still around. It's just not built the old way anymore-not for most people. That's the direction software is headed, too.

A year ago I wrote that full-stack devs weren't going anywhere. I still believe that. What's changed is how much clearer I am now about what *"not going anywhere"* actually requires.

---

## The Brain in the Application

It started with a Copilot subscription hooked up to VS Code. I pointed it at an application I'd written by hand and just started poking at it, seeing what it could do. Some sections were genuinely hard-tricky UI, messy logic I wanted cleaned up-and I wanted to see if it could actually help with those, not just autocomplete a line here and there. I wasn't vibe coding. I was having it help me.

Then I started describing whole features instead of lines. I'd tell it what I wanted, and it would build it. The first time that worked, I remember thinking, *okay, that's cool, but it doesn't match the style I wrote the rest of the code in.* So I told it that. Next round, it rewrote the feature to match my style. That was a real moment for me. It wasn't just generating code; it was adapting to how I work.

Wanting to understand what was actually happening under the hood took me past VS Code tools and into the world of Hugging Face and Ollama. Honestly, I didn't know what I was doing at first. I had to learn how to install Ollama directly into my own application, how to call the different local models, what tokens even were, and the limits of running everything on CPU versus GPU. It was a lot of new information all at once, and it was a little overwhelming at first.

Then I vibe coded my first local LLM application, just to see how it worked. When I looked at the actual prompt it was passing, the lightbulb went off. I realized this was exactly what I'd been doing with Copilot every day-polishing an email, asking it about something I didn't understand. Same thing, I just hadn't seen it stripped down like that before.

There's a *brain* sitting inside the application. Not a tool bolted on the side. A partner I could hand real, complex problems off to, and it would go further than I expected on its own. That's when it started to snowball. It changed how I thought about AI generally-not a bolt-on sitting next to the code, but something that could actually see the application, understand it, and make real changes to it. That's the perspective I brought back to my team.

---

## Watching the Lightbulbs Go On

When we decided as a team to actually bring AI into how we work, we started together, as a group, running through prompt engineering exercises. We were amazed by what it could do.

Once I let developers start applying it on their own, I noticed something. I'd had six months on this, and if I'm honest, I probably sounded the same way six months earlier. The most common reaction was something like, *"Well, this is how I'd do it,"* or *"This is how I want to use it."* It stopped at what was familiar instead of pushing to find out what else was possible.

So I kept pushing:
* *Feed it a screenshot.*
* *Be more explicit about what you actually want.*
* *Use your words, be verbose.*
* *Fail quickly, and move on instead of getting stuck.*

Then we hit a project where we genuinely didn't know if AI could handle it, and we weren't sure how to even approach it. There was some hesitation at first, since it wasn't how we'd normally have gone about it. But the project needed to move, so I said, *"Let's just try it."*

I won't get into the specifics, but we experimented, pushed the boundaries, and some things worked far beyond what we expected. Other things didn't work at all. Failing quickly let us adjust fast, and each round got a little better than the last, until we'd gotten a large portion of the project done in a matter of weeks-work that would have taken months, maybe years, the old way.

---

## Where I'm Actually At

That win felt good. It also sat right next to something I hadn't fully worked through yet.

Here's the part I'm still working through: I used to be a developer. It was my identity for a long time. Watching the thing you built your career on turn into more of a hobby than a job description is a strange feeling, even when you believe it's the right direction.

Now I'm the guy in management trying to figure out how my team should actually use this, trying to stay safe and practical, trying to keep people in real, meaningful roles while the old silos stop making as much sense as they used to. It's less about who owns the frontend or the backend now, and more about how well you interact with AI, how well you test what it hands you, and whether you're strong enough to look at the output and say, *"No, that's not right,"* and go back and hammer at it again.

There are still moments I catch myself second-guessing a dev's approach, wondering if I'd have gone about it differently. I don't always have a better answer ready when that happens. I'm figuring this out alongside my team, not two steps ahead of them.

If you're a leader going through the same thing-trying to reorganize how your team works, trying to figure out what to hire for, what to teach, what to let go of-I'd genuinely like to hear where you're at with it. I don't think anyone has this fully solved yet, and I'm suspicious of anyone who claims they do.
