---
layout: post
title:  "Status of kickConnect"
date:   2024-11-11 12:00:00 -0700
categories: kickConnect
---
## kickConnect v.0.3(Alpha)
The current version released a few weeks back is v0.3 - I finally finished a major component (Scheduler)!  I wanted an experience much like when I schedule meetings.  I wanted to book classes using a visual representation of when those classes would appear on the weekly calendar.  There was <b>A LOT</b> of testing that when into this functionality.  As it stands right now a user can add Existing Classes that were entered in previously (the user is shown a list) as well as New Classes (ones that have NOT been added to the Classes table).  The user can also edit classes that have been added to the scheduler by updating the day, time, reservation and cost!<br>

![Scheduler Screenshot](/assets/images/KC-Scheduler.png)

#### Testing: Playwright
As a developer I have used Selenium for regression testing. A while back I started to hear about Playwright.  I started looking at it last week and HOLY COW IT IS AMAZING!!!  And...  Super simple.  I'm still writing tests, but I can now say the kickConnect NOW HAS TESTS!  What I would like to do is write a test for every component that kickConnect has, then I want to write tests that will "SEED" the database for release purposes.  As the application gets bigger with more features the database is harder and harder to keep clean. So being able to truncate all the data out of the database and then have tests to re-add the data, all while testing to make sure everything works seems like a no brainer.

#### Working on NEW features
I'm working on 3 features right now!  Profiles, Shopify integration and HTML Template Customization.

Profiles is the pre-cursor for the ability to really complete the circle of Events/Classes.  The system allows for the creation for Events, and as discussed above users can now "Schedule" those Events/Classes.  The last step is to "Assign" the Events/Classes to Profiles.

Shopify Integration is in the infant stages of development.  But the idea is I want kickConnect to tie into the Shopify network for e-commerce capabilities.  

The last thing that I'm pretty stoked about is the HTML-Template customization.  One of the requirements I had early on for kickConnect is to allow the functionality to offer HTML Templates for small businesses to host.  This weekend I started work on that.  I'm very excited to show what capability soon!

### What's the Road map...
-Profiles
-Shopify
-HTML-Template Customization
-Component Management
    - Ability to turn on and off components for users
-Member Portal
-Member Tables and Date Input
-Importing existing data 
-Phone Apps
-Communication ability

-AWS Architecture
    - Lambdas
    - API Gateway
    - Containers
    - Deployments
