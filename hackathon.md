---
title: Symphony 2019 London Hackathon
description: What Went Down At Credit Suisse's Offices in Canary Wharf
image: assets/images/hackathon.jpg
layout: post
menu: true
---

# Hackathon

On 12th September, Symphony ran the 2019 London Hackathon at Credit Suisse’s offices in Canary Wharf.  I was lucky enough to attend as part of the Deutsche Bank team.

As one-half of DB's Symphony Practice, I was very keen to get a team together to attend this - not really to win so much as just to have an experience of a hackathon. It’s not something I’d done before, and this seemed like a good place to start.  Rather than spanning a whole 24-hour period as some do, this was constrained by the 9-5 working day.  Lunch and dinner were promised, and it looked like a good opportunity to meet with some other Symphony developers working in London.

## The Team

The first problem was getting a team together.  Obviously, Mark and I from the Symphony Practice could attend, but we’d be rather short handed.   A week before the event, I’d tried all sorts of channels and was coming up with nothing.  But then a week before, Liam came on-board as a totally-new-but-willing-to-learn Symphony developer and offered his services.  And then just a day before the hackathon started, Ivan, an experienced bot developer, offered his services to the team.  We were ready to go!

## The Problem

It’s really important to make sure that you have a firm idea of what you’re doing before going into any hackathon. You don’t want to waste your fairly short time limit coordinating the team on what to do.  We had a fairly good idea of something to build:  we had some clients in the fixed income team that wanted to pass around and edit a table of bond details between themselves.  This sounded like a pretty good use-case:  how about instead of just a table of bonds, we built some functionality to pass around, edit and then sign-off on any table?  

This seemed like a really useful Symphony use-case, and something not actually built into the platform… but at the same time, it would require building a Symphony app, which was a lot more work than building a bot.  In order to make this possible, I set us up with a Linode to run our app on, and cloned a starter project into github that we could collaborate on.  

## The Day

We started badly.  Our Linode was not accessible via the Credit Suisse wifi network, so we ended up using an iPhone hotspot.  However, by lunch we’d managed to get some useful stuff done:   a basic table-editing page, and On-Behalf-Of posting of the table into a chat room.  

But then we started to think about the demo:  how would we present this?  We’d like to show some people interacting in a back-and-forth, changing the table as they went.  So Liam got to work and started building a bot that would be able to post a table of bonds into a chat room.

Late into the afternoon, most things were working ok:  approvals were looking good, and the table was displaying nicely in the chat. But we still had some major bits of functionality not working right:  it was hard to get the table data back out of the chat room and into the editor.

Also, our github project was looking like a battleground.   Some bits of code interfered with others.  We couldn’t reliably run the whole thing in a single process as the bot and the app didn’t work together.  Ivan suggested refactoring it, but with mere hours left, there was no guarantee that we’d get that finished in time.   

So, we fudged the rest of it (hard-coding in bits of data) and hoped no-one would notice.  (They didn’t)

## The Presentation

There were maybe 15 teams at the hackathon, and to keep things interesting, each team had 5 minutes to explain and present their work.    We were up 4th, which meant at least we could get things over with.  While team 2 was doing their demo, I ran through what I was going to present… only to find the bot wasn’t responding!  

Some quick nudges to Liam later meant we got that up and running on his laptop, and things were just about ready.  

But 5 minutes was really too short a time to explain what we’d been building, and demonstrate it.  We hit the time barrier hard.  It was entertaining, but perhaps confusing.  Most importantly, the demo worked and our pride remained intact.

## The Result

Well, we didn’t win.   What makes a useful business use-case and a winning hackathon idea turn out to be two entirely different things.   The latter must be something immediately appealing, can be explained in less than thirty seconds and doesn’t tax the audience to understand something new.  We weren’t building that!

But on the other hand, we got to take home a piece of functionality that we can build on and deploy at DB.  It was incredibly stressful to code agains a tight hackathon deadline, so I don’t think I want to do another one, but to have experienced one was well worth it.