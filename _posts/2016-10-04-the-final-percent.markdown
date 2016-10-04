---
layout: post
title:  "The final 1% in product : making use of what you already have"
date:   2016-10-03 10:54:00 +0100
categories: Portfolio
---

I've decided to write reflections on my time in the job I left a few months ago (Hosted Graphite, my first post-college job). Architects often say "I don't know what I think till I've seen what I've drawn", swap in written for drawn and that's what I'm trying to do here. To think about what worked and what didn't, on what I got right and what I lacked. It's the start of an ongoing effort to both poke holes and fun in my thinking then and now. And hopefully come out with a better understanding of how we work, and often don't. Or at least thats the bullshit mission statement.

One of the biggest changes over the year and a bit was how my perception of real work changed. When I started I seemed to consider the hard engineering and design work to be the only real work that was going on. Though I probably just didn't have the confidence and data to trust my deeper instincts. So I spent time building big "release features" and then when I wanted to mess around for a few hours I'd do the what-I-considered silly work, the three PR's a day kind of tasks. However I think it's often these tiny things that made better use of my time and of everyone in the companies work. As I got more confident I grew the deep desire to stop constantly building new big release features and preferred joining the dots between all the features already deployed.

### 1) Help users understand what they've already paid for

Alerting was always a big feature request for HG. Several engineers including me spent months and months working on it and refining the complex code and interface interactions. So we built and we tweaked, we soft launched and then we hard launched.  A few big customers relied on this quite quickly, but strangely enough there was not a lot of mid level usage (i.e. people using it for 4-10 critical alerts, what we considered it most useful for). It was a top level menu item, everyone was included in the mail campaigns for it and it was included in everyones payment plans and it was bloody useful, so why weren't they using it! So the And the product became more reliable, more usable and more beautiful, but the usage never changed. People just weren't setting up that first alert. Eventually we paused improving the alerting interface and we fixed this bigger issue by tackling... the home-screen.

The homescreen for our app was always a stop off until you launched Grafana for 99% of use cases. And under that confused purpose it was a jumble of bits and bobs of the admin interface. So, in a bid to just get something tested quickly, I knocked up a a few dozen quick iterations for new concept for a homescreen. One half based on helping the user get to top 1 or 2 tasks they wanted to achieve but also the top row constantly informing them what they had paid for and used. Below you can see the before and after.

With this, probably 5-7 days of work, in a matter of a few weeks there was an increase from a few big customers to nearer 50-100 medium customers  using the feature properly as well. A few days work to get customer reach for what was more than a years combined engineering work, this is what reinforced the knowledge that time spent on the little things was often the best way to spend a few days.

### 2) Being proud of our own work

If you're actually proud of your work then you should be as confident as the biggest players are!

Since it's inception HG has had lots of self built integrations with 3rd party sites. Yet there was no page that listed all these plugins/add-ons/integrations as they were considered too disparate in functionality to be considered any one of the above.

Yet when we actually took a look at Slacks' or Herokus' add-ons for example, they were as disparate in functionality as ours! They just had the confidence to group them anyway as it's just easier for customers. It didn't matter if it wasn't exactly an add-on, the user would come to that page to see if we had anything like that, so it should be there. So... a few days later we launched an add-ons page! Although this was not a new engineering feature it gave the whole company a language and confidence to be clear to our customers of what we build and what we support. This showed off so many corners of HG (and accumulated years of engineering work) with just a few days frontend hackery.

### 3) Finally, talk to your users about your old features as well as your new ones

Soon after the add-ons page project, I realised there was lots of useful older work, including add-ons, that people might want to use but have never considered looking for. While email was great for new feature rollouts, it was less suitable for spamming the user about these older features.

We were obviously already tracking what customers used and even sometimes what they probably should be using. So a few days hacking later and we had soft messaging on the homepage chatting to the user casually (but not overly-friendly) about all the things they hadn't used yet. It's small, doesn't get in your way and uses the tone of "you've already paid for this very useful thing"; not sales-y but helpful.

### Give precedence to refinement rather than new features

The lesson here for me has been to have joy in my work, thus I'll truly desire as many of the customers use as much of it as I can. And from the data you can often see these small links are more useful than another "big feature" that most of your customers don't find. Most of this can of course be found worded differently in "Lean X" or whatever, but learning a lesson yourself beats just reading about it 20 times.
