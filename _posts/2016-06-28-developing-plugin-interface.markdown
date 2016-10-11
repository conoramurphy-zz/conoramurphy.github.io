---
layout: post
title:  "Moving from Integrations to Plugins"
date:   2016-09-28 16:54:00 +0100
categories: Product
---

### Problem

The company had built up an extended library of plugins and options for integrating with third party services. These were of varying complexity from a simple configured url endpoint to a whole suite of software for integrating with AWS. However they were collected in different places like the docs for the configured URL, an integrations page for the biggest ones and the alerting interface for endpoints you can send alerts to.

We also did not have a lot of spare time to fix this.

#### Responsibilities

The idea, feature list, UX, visual design and frontend engineering.

#### Technology

Django, HTML, SCSS, JS, ES6, Jquery

#### JTBD (Job To Be Done)

"When setting up my account, I want to understand what services I can integrate with so I can see my data faster."

### Design and Implementation

This was completely under my prerogative and thus I quickly spent a day knocking up dozens of rough options and discussing them with my work mates and getting their feedback.

After this round I quickly focused on the core use case of exposing all the different work we've done to as wide an audience as possible and making it responsive and clean. I focused on a card based interface and we had the design for the alerting page done which was similar. So I stuck to that and just made it as clear as I could what everything did.

#### Language Change

The first thing I had to do was convince our team that broadening of our conservative definition of an "add-on" was needed. Previously we only referred to somethings as a data source and other things as alerting notification sources etc. and they were all on different pages on the site and in documentation. After referring to the the broadness in functionality of Heroku and Slack add-ons as comparisons we were able to move a lot more things under the umbrella of add-ons. This allowed not only the navigation to be simpler but also allow our team to be more confident and clear when talking to customers and when writing documentation.

#### Results

![Add Ons Before Change]({{ site.baseurl }}/assets/addOnsBefore.png)
<div class="centre-contents">
  <span class="img-title">Data Sources Before Change</span>
</div>

![Sketches showing what short of Alerting interface]({{ site.baseurl }}/assets/addonsFinished.png)
<div class="centre-contents">
  <span class="img-title">Add Ons After Change</span>
</div>
