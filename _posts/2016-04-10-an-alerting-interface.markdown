---
layout: post
title:  "From ideation to launching an alerting interface"
date:   2016-10-03 10:54:00 +0100
company: Hosted Graphite
categories: PM, Design
---
### Problem

As a graphing company customers were always seeing issues shown by their graphs that they wanted to know about when they happened again i.e. some form of alerting. This was by far the most pressing and requested feature for over a year and competitors ananlysis showed that it was both necessary and a market opportunity, for example AWS's was extremely limited and this could be a useful differentiator.

#### Responsibilities

All the UX design, visual design and front-end engineering.

#### Technology

Django, HTML, SCSS, JS, ES6, Jquery

#### JTBD (Jobs To Be Done)

We set out some example JTBD to focus our improvements on the areas that matter most.

* When I see a worrying spike in my graphs, I want to know when that happens again.
* When I'm in the middle of an incident and alerts are raining in; I want to be able to shut up alerts so I can get work done without worrying about forgetting to turn them back on.

### The solution

#### The beta

I sketched out both an ideal use case and edge cases for the design. The ideal use case (i.e. someone using it for it's full potential) is someone only alerting on the most valuable information for a high number of their metrics.This would only be a minimal number of alerts as you can use wildcards (\*) to expand metrics to include all similar cases. The less than ideal case was someone creating hundreds of alerts that were similar in logic. The interface had to stand up to both basic requirements, however we did everything we could to encourage the former. It involved several months of iteration and working with the backend engineers but we launched an initial beta (an MVP) to a few valued customers who were generous with feedback.

<div class="centre-contents">
  <span class="img-title">Wireframes and designs we started building on</span>
</div>
![Sketches showing what short of Alerting interface]({{ site.baseurl }}/assets/alertWireframes.png)

<div class="centre-contents">
  <span class="img-title">Designing out a "sentence building" alert UI (1)</span>
</div>
![Designing out a "Sentence Building" Alert UI 1]({{ site.baseurl }}/assets/alertConversationUI.png)

<div class="centre-contents">
  <span class="img-title">Designing out a "sentence building" alert UI (2)</span>
</div>
![Designing out a "Sentence Building" Alert UI 2]({{ site.baseurl }}/assets/alertConversationUI2.png)

#### The refinement and moving beyond a beta

2 months after the Alerting beta we reached the point where critical patches and imporvements were complete and we had some space to refine what we had. I re-analysed any feedback and testing we'd solicited off willing customers and analysed what type of Alerts were actually being used. The feedback was mainly usability tweaks which we duly took on board and implemented if they aligned with other use cases. In analysing what companies actually used their alerts for it turned out that well over 80% of the alerts created were a simple "above a threshold" alert.

We immediately integrated the usability feedback and focused the complex alert creation form on the top use cases, i.e. include defaults where for most fields the input would be left untouched 80% of the time.

After this work we arrived at the end of the MVP project and it was moved out of beta. The results of the feedback period are seen below.

<div class="centre-contents">
  <span class="img-title">Creating an Alert and then pausing it</span>
</div>
![A gif about creating an Alert and Pausing it]({{ site.baseurl }}/assets/alertCreate.gif)

<div class="centre-contents">
  <span class="img-title">Rather than stating the error we show how to fix it</span>
</div>
![Errors Showing how to fix the problem]({{ site.baseurl }}/assets/alertError.png)

#### Helping users to actually use our alerting funcitonality

A few big customers relied on alerting quite quickly, but there was not a lot of mid level usage (i.e. people using it for 4-10 critical alerts, what we considered it most useful for). It was a top level menu item, everyone was included in the mail campaigns for it and it was included in everyone's payment plans and it covered a very commonly requested feature, so why weren't they using it? I created a theory that people didn't realise they had already paid for it.

Eventually we paused improving the alerting interface and we fixed this bigger issue by tackling... the home-screen.

The home screen for our app was, for 99% of use cases, a minor stop off point until you launched the app. And under that confused purpose it was a jumble of bits and bobs of the admin interface. So, in a bid to get something tested quickly, I knocked up a a few dozen quick iterations for new concept for a home screen. The top row of the homescreen is now focused on informing them what they have paid for and used, this includes indicating that they already have paid for alerts they have not used.

<div class="centre-contents">
  <span class="img-title">Home screen row showing what you've used as part of your subscription</span>
</div>
![Homescreen Row Showing What You've Used]({{ site.baseurl }}/assets/alertHomeScreen.png)

In a matter of a few weeks there was an increase from just a few big customers to nearer 50-100 medium customers as well using alerting regularly. So the homescreen alterations stayed and refined further.
