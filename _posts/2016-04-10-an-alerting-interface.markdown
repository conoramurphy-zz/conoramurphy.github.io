---
layout: post
title:  "From Ideation to Launch : An Alerting Interface"
date:   2016-10-03 10:54:00 +0100
categories: Portfolio
---
### Problem

As a graphing company people were always seeing interesting problems in their graph they wanted to be told about if they happened again. This was by far the most pressing and requested feature for over a year.

#### Responsibilities

All the UX design, visual design and front-end engineering.

#### Technology

Django, HTML, SCSS, JS, ES6, Jquery

#### JTBD (Jobs To Be Done)


"When I see a worrying spike in my graphs, I want to know when that happens again".


"When I'm in the middle of an incident and alerts are raining in, I want to be able to quickly pause alerts so I can get work done."

### The Solution

#### The Beta

The set both an ideal use case and edge cases for the design. The ideal use case (i.e. someone using it for it's full potential) is someone only alerting on the most valuable information for a high number of their metrics. In the ideal case this would only be a minimal number of alerts as you can use wildcards (\*) to expand metrics to include all similar cases. The less than ideal was someone creating hundreds of alerts. The interface had to stand up to both basic requirements. It involved several months of iteration and working with the backend engineer but we launched an initial beta several months after starting the project.

![Sketches showing what short of Alerting interface]({{ site.baseurl }}/assets/alertWireframes.png)
<div class="centre-contents">
  <span class="img-title">Wireframes and Designs we started building on</span>
</div>

![Designing out a "Sentence Building" Alert UI 1]({{ site.baseurl }}/assets/alertConversationUI.png)
<div class="centre-contents">
  <span class="img-title">Designing out a "Sentence Building" Alert UI (1)</span>
</div>

![Designing out a "Sentence Building" Alert UI 2]({{ site.baseurl }}/assets/alertConversationUI2.png)
<div class="centre-contents">
  <span class="img-title">Designing out a "Sentence Building" Alert UI (2)</span>
</div>

#### The Refinement

We set a refinement point for 2 months after the Alerting Beta release. At this point I re-analysed any feedback and testing we'd solicited off willing customers and analysed what type of Alerts were actually being used. The feedback was mainly usability tweaks which we duly took on bored and implemented if they made sense with other use cases. In terms of the analysis of what the companies actually used it turned out that well over 80% of the alerts created were a simple "above a threshold" alert.

This allowed us to both integrate the usability information and focus the form on the top use cases, i.e. include defaults where for most fields would be left untouched 80% of the time.

After this work we arrived at the end of the MVP project and it was moved out of beta. The results are seen below.

![A gif about creating an Alert and Pausing it]({{ site.baseurl }}/assets/alertCreate.gif)
<div class="centre-contents">
  <span class="img-title">Creating an Alert and then pausing it</span>
</div>

![Errors Showing how to fix the problem]({{ site.baseurl }}/assets/alertError.png)
<div class="centre-contents">
  <span class="img-title">Rather than stating the error we show how to fix it</span>
</div>

#### Helping users to start Using Alerting

A few big customers relied on this quite quickly, but strangely enough there was not a lot of mid level usage (i.e. people using it for 4-10 critical alerts, what we considered it most useful for). It was a top level menu item, everyone was included in the mail campaigns for it and it was included in everyones payment plans and it was bloody useful, so why weren't they using it! So the And the product became more reliable, more usable and more beautiful, but the usage never changed. People just weren't setting up that first alert. Eventually we paused improving the alerting interface and we fixed this bigger issue by tackling... the home-screen.

The homescreen for our app was always a stop off until you launched Grafana for 99% of use cases. And under that confused purpose it was a jumble of bits and bobs of the admin interface. So, in a bid to just get something tested quickly, I knocked up a a few dozen quick iterations for new concept for a homescreen. The top row of this is now focused on informing them what they had paid for and used.

![Homescreen Row Showing What You've Used]({{ site.baseurl }}/assets/alertHomeScreen.png)
<div class="centre-contents">
  <span class="img-title">Homescreen row showing what you've used as part of your subscription</span>
</div>

After this few days of work, in a matter of a few weeks there was an increase from a few big customers to nearer 50-100 medium customers  using the feature properly as well.
