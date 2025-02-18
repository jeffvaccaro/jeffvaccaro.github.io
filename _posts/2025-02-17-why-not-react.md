---
layout: post
title:  "Why NOT React?!?!"
date:   2025-02-17 12:00:00 -0700
categories: kickconnect
---

Just to update everyone on my progress with **KickConnect**:
### What's the Road map (as of 01/04/2025)
- ~~Profiles~~ **DONE!**
- ~~Class Assignments~~ **DONE!**
- ~~HTML-Template Customization~~ **V1 DONE!**
- Component Management
    - Ability to turn on and off components for users
- Member Portal
- ~~Member Tables~~ **DONE!**
- Importing existing data 
- Phone Apps ***Just started!***
- Communication ability
- Shopify

- AWS Architecture
    - Lambdas
    - API Gateway
    - Containers
    - Deployments


### Why NOT React?
At work, people often ask me what architecture I prefer. I always respond Angular - then I get a side-eye, and usually, people roll their eyes.

I know that React is all the rage right now. I remember when Angular was all the rage. Folks, it's just another framework! The difference I've seen is that Angular is opinionated, and to be perfectly honest, I like that. I messed around with React, and there was zero structure. You have to be very careful to craft your projects consistently; otherwise, you wind up with a giant mess.

When I started with KickConnect, I knew that I didn't want to spend a ton of time in CSS hell with image creation, pixel sizing, and SCSS vs. CSS, not to mention CSS Grid vs Flexbox etc. I wanted and needed a pre-built UI. At first, I thought I would do it in React to add it to my resume. I purchased my UI and then dove right in - Holy HELL! I've been frustrated in my life before, but I have not been that lost in a project in a VERY LONG TIME! I tinkered and tinkered with the UI codebase for many days (at least a week plus!) until I said, "eff it, I'm going to Angular".

As you know, I've spent the last 5+ years in Angular, so when I found a new UI in Angular, I was writing code within a day! I know I'm familiar with Angular, so that is the main reason for the quickness. I know there can be a certain amount of garbage in any project, but if you do it right, everything is laid out very nicely, and your application is really easy to understand in Angular.

There may be some great things that React does better than Angular. I just saw the nested upon nested files, and the red flags were raised. To be fair, I really did try with React. I looked at the pros and cons, and honestly, I didn't see much of a difference. So after the UI debacle, it was a no-brainer for me.

***Further Thoughts on Angular vs React:***

<b>Scalability:</b> Angular's structure makes it easier to scale larger applications with a consistent coding standard. React, being a library, offers more flexibility, but this can lead to inconsistencies in larger projects.

<b>Performance:</b>  React's virtual DOM can offer performance benefits in certain scenarios, but Angular's two-way data binding can simplify complex forms and data interactions.

<b>Community and Support:</b> Both Angular and React have strong communities, but Angular's full framework offers more built-in support for common scenarios like routing and form handling, whereas React relies on third-party libraries.

### Flutter over React Native
I know neither currently, but I guess I'm team Google! I went with Flutter, and so far, it is pretty nice. I will say that setting up Flutter because of Java was dumb and could be made a boatload easier, but after everything was installed correctly, it does work pretty nice!

***Further Thoughts on Flutter vs React Native:***

<b>Performance:</b> Flutter's use of the Skia graphics engine allows for smooth animations and graphics, often resulting in better performance compared to React Native, which relies on a JavaScript bridge to interact with native components.

<b>Development Speed:</b> Flutter's hot reload feature is a game-changer, allowing developers to see changes instantly. React Native also offers a similar feature, but many developers find Flutter's implementation more seamless.

<b>UI Consistency:</b> Flutter provides a single codebase with consistent UI across both iOS and Android. React Native allows for platform-specific code, which can lead to inconsistencies in the user experience.

<b>Ecosystem:</b> While React Native has been around longer and has a more mature ecosystem, Flutter's ecosystem is rapidly growing with strong support from Google and a passionate community.

There will be more to come on Flutter in the future. Right now, I've written one page in it. There will be more on that later!