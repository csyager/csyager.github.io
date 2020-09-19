---
layout: post
title:  "Delta Sig Rush Site"
date:   2020-06-04 01:45:00 -0400
categories: project
---

<div class="" style="float: left; margin-bottom: 2%; width: 50%; margin-right: 2%; border-style: solid">
    <div id="carousel" class="carousel slide" data-ride="carousel">
        <div class="carousel-inner">       
            <div class="carousel-item active">
                <a href="/assets/images/deltasigrush/index.png"><img class="d-block w-100" src="/assets/images/deltasigrush/index.png"></a>
            </div>
            <div class="carousel-item">
                <a href="/assets/images/deltasigrush/rushee_signin.png"><img class="d-block w-100" src="/assets/images/deltasigrush/rushee_signin.png"></a>
            </div>
            <div class="carousel-item">
                <a href="/assets/images/deltasigrush/current_rushees.png"><img class="d-block w-100" src="/assets/images/deltasigrush/current_rushees.png"></a>
            </div>
            <div class="carousel-item">
                <a href="/assets/images/deltasigrush/rushee.png"><img class="d-block w-100" src="/assets/images/deltasigrush/rushee.png"></a>
            </div>
            <div class="carousel-item">
                <a href="/assets/images/deltasigrush/voting.png"><img class="d-block w-100" src="/assets/images/deltasigrush/voting.png"></a>
            </div>
            <div class="carousel-item">
                <a href="/assets/images/deltasigrush/results.png"><img class="d-block w-100" src="/assets/images/deltasigrush/results.png"></a>
            </div>         
        </div>
        <a class="carousel-control-prev" href="#carousel" role="button" data-slide="prev">
          <i class="fa fa-chevron-left" style="font-size:36px; color: black"></i>
          <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carousel" role="button" data-slide="next">
          <i class="fa fa-chevron-right" style="font-size:36px; color: black"></i>
          <span class="sr-only">Next</span>
        </a>
    </div>
</div>

Going into my fourth year, one of the biggest yearly difficulties I faced was rush voting.  This is a process that can take legitimately up to 6 hours in each of the four rounds of voting, most of which occur on weeknights where the brothers have class the next day.  Rush is an essential process for a fraternity, as our existence and financial security rest solely on our ability to recruit new members.  While we had a system in place to track people coming through the door, it was clear to me that our system could be improved.

Notably, there was no electronic system in place for voting.  This was by and large the biggest time sink in the entire process.  Voting is usually conducted by raise of hand or by placing votes in a bag.  This process was not efficient, and was one that I felt I could help optimize.  Challenges involved were making sure that every brother was able to access the site, that their votes and interactions with the rushees would be counted distinctly and attributed to their user accounts, and combining various technologies to make sure that we were tracking essential information on each of the rushees, including a picture of themselves that they take at the door and their contact information.  To do this, I used the Django framework, because I was familiar with it through my coursework, and because it handles a lot of the user account stuff natively.  This meant that I would be able to get a lot done without spending too much time on the little things.

Insofar as meeting the stated goals of the project, the application was a big success.  Our tedious voting process was sped up a lot, and rush was conducted more efficiently all around.  There were also lessons learned though, and certainly room for improvement.  On one of the first nights of voting, we had a big problem with how long the site was taking to load, because we hadn't tested it with so much data in the database before.  As it turns out, I had mistakenly saved a pretty sizable chunk of useless data that was originally stored when rushees took their pictures on the first night.  When many rushees were being loaded at once, this created a huge bottleneck on our process.  Fortunately, after a few hours of looking over the code I diagnosed the problem and fixed it before our next round of voting, but I learned an important lesson along the way about scaling when handling redundant data.

Because the project worked so well for rush, I was asked if we could expand it to handle other fraternity functions, like our social events.  This expansion of functions is a project that I'm still working on, and have adapted into my GreekLink project that I talk about in another post.  But it's been a lot of fun building this system for a group of my friends, which have been like a microcosm of a userbase.  The project taught me a lot about soliciting requirements and working with a nontechncial "client" of sorts, and I hope that the site I built can continue to be useful for our chapter.