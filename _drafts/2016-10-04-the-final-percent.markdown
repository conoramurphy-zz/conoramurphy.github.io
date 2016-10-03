---
layout: post
title:  "The final 1% in product : making use of what you already have"
date:   2016-10-03 10:54:00 +0100
categories: Portfolio
---

Sometimes you can only apply a narrative to something after all the actions happen. I've found this recently in figuring out what I want to do in life (help people work and live easier) by looking back at what I've always been doing. In work after my year and a half at Hosted Graphite I looked back and figured out what I was most proud of. And it wasn't any one big feature (though there were a few of them) but the tiny things that make much better use of everyone in the companies work.

Too often we consider the hard work to be the real work. So we build a tough feature to the point that it works well and then quickly run off to firefight the next big feature request on the backlog. As I looked back on the year and a half I realised as I got more confident and my work got better the major differentiator was moving from more "big features" to a desire to join the dots between all the features already deployed.

### 1) Help users understand what they've already paid for ##


Alerting was always a big feature issue for us. Several engineers including me spent months working on it and refining the much more complex interactions that we'd ever had on the site before. So we built and we tweaked. We soft launched and then we hard launched. And the product became more reliable, more usable and more beautiful. A few big customers relied on this heavily quite quickly, but strangely enough there was not a lot of mid level usage (i.e. lots of people using it for 4-10 critical alerts, the use case we most designed for!). We didn't really understand this as it was a top level menu item and it was included in everyones plans. Eventually we paused improving the alerting interface and fixed it by fixing, the home-screen.

The homescreen for our app was always a stop off until you launched Grafana for 99% of use cases. And under that confused use case it was a rather confused jumble of bits and bobs of the admin interface basically.

So I, in a matter of days, quickly knocked up a a few dozen quick iterations for new concept for a homescreen. One based on the top 1/2 tasks the user wanted to achieve but also subtly informing them what they had paid for and not used. Below you can see the before and after.

With this weeks work total in a matter of a month there was an increase to between 50-100 customers actually using the feature for above 1/2 test alerts. This after it had already been out months and had only had less than 10 people using it like this yet. A few days work to get customer reach for what was more than a years combined engineering work.

### 2) Being Proud of our own Work ##

Since it's inception HG had had integrations with 3rd party sites. It's what made it so extra useful over self deployed Graphite/Grafana instances. Yet there was no page that listed all these plugins/add-ons/integrations as they were considered too different, not neat enough to be considered any one of the above.

Yet when we actually took a look at slacks add-ons for example, they were as disparate in functionality. So with that and a few days quick work we had an add-ons page! Better than that, we included things that mightn't be fully considered add-ons but were simple ways to get things like annotations in from different services (github deployments for examples). It didn't matter if it wasn't exactly an add-on (it was just a specifically configured url for that account they could copy and paste), the user would come to that page to see if we had anything like that, so it should be there.

Again, not being unsure of ourselves and proudly showing off all our third party work (accumulated years of engineering work) allows a few days work to benefit so many corners of the project.

### 3) Finally, talk to your users about your old features as well as your new ones

Finally, not a hugely new one to most of you. While email we found was great for new feature rollouts, it was less suitable for spamming the user about old features we have that maybe they haven't used yet, or looked at but it'd better since then.

But we were obviously already tracking what they used. So a few days hacking later and we had soft messaging on the homepage chatting to the user casually (but not overly-friendly) about all the things they hadn't used yet. It's small, unobtrusive and doesn't get in your way whether you use it or not.

### A few days work to make use of years of work

The lesson here for me has been to take genuine joy and pride in your work, and thus spend those few days making sure all those small links you can put in your app can be way more useful than another "big feature" that your customers don't use. It's something I take true joy in implementing and see the affects live within a few days or weeks.
