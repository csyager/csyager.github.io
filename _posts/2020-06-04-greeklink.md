---
layout: project
title:  "GreekLink"
date:   2020-06-04 01:45:00 -0400
categories: project
carousel:
    - image: /assets/images/greeklink/greeklink_screenshot.png
    - image: /assets/images/greeklink/list_active_screenshot.png
    - image: /assets/images/greeklink/resources_screenshot.png
    - image: /assets/images/greeklink/settings_screenshot.png
---

GreekLink is a software project a few friends and I have been working on.  At my fraternity chapter, we traditionally spend a lot of time conducting rush voting.  It's a huge hassle, having to vote on every person that walks through the doors, with each of the four rounds of voting taking usually between 3 and 6 hours.  We used a web application designed by an alumni that wasn't particularly user-friendly, and was in need of some improved tools to increase productivity.

To fix these issues, I volunteered to redesign the site, with the primary goal being that we could conduct voting electronically.  In the past, voting was conducted by either a show of hands or the placing of chips in a bag.  These processes both took a matter of minutes to conduct, and my goal was to reduce this operation to a matter of seconds.  To do this, I designed a highly interactive web application using the Django python framework.  The site was deployed using Heroku, and managed everything involved in rush, from the scheduling of events to rushees signing in at the door to track attendance to the voting itself.  When it came time to conduct voting, rushees were pulled from our database of people who had attended the events, and users could place their votes on their phones.

While there were a few hiccups to work through as we pushed the boundaries of how much load the application could handle from time to time, it eventually got to a point where things were running really smoothly.  So smoothly, in fact, that we decided to expand the site to include features for planning and managing social events throughout the semester.  This got my friends and I thinking, and we reached the conclusion that we could create a one-stop-shop for all of the people-management, planning, and communication that goes into running a Greek organization and sell the product for profit.  Thus, GreekLink was born.

While it is still a work in progress, many of the systems that were thrown together haphazardly for the initial product that my fraternity used have been deeply refined and polished.  We've been looking into elastic hosting options that will allow us to scale out to meet the needs of mulitple Greek organizations, and will hopefully even be able to facilitate communication amongst the community through our application.  This project has been a lot of fun, and I'm excited to see where it will go next.