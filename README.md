# Worn proposal

written in collaboration with [@mt5135](https://github.com/mt5135)

## What and Why

Worn is a digital wardrobe tracker that lets users catalog their clothing and log wears, calculating a real cost-per-wear for each item.

Most people have no accurate sense of how much value they get from their clothes. A $200 jacket worn 100 times costs $2/wear; a $20 shirt worn twice costs $10/wear — yet without tracking, the cheap item feels like the smarter buy. This gap between perceived and actual value drives poor purchasing decisions and leaves closets full of underused clothing.

Worn makes cost-per-wear visible. Users log items (photo, price, category) and record wears with one tap, or bulk-log an estimate for existing pieces ("worn ~15 times this year") so the tool is useful immediately, not just after weeks of tracking. Over time, users see clearly which purchases earned their keep, which didn't, and where their clothing spend is actually going.

## For Whom

Worn is for college students who buy clothes regularly but have no real sense of what they're actually getting out of those purchases. Our first users are our own friends and classmates, since they're real people we can onboard, watch use the app, and get honest feedback from all semester.

Students are a good starting point for a few reasons. They're active but budget-conscious buyers, juggling limited income against frequent purchases, so a tool that shows real value per item is actually useful. They're already used to logging things through their phones and taking quick photos, so the core habit (snap a photo, tap to log a wear) isn't a big ask. And because they're people we can talk to in person, we can watch where cataloging feels tedious or confusing and fix it based on real use, not guesswork.

The idea isn't limited to students. Anyone trying to buy more intentionally, cut down on impulse purchases, or just understand their closet better could get value from it. But students are who we'll build for and test with first.

## How

Building your closet: A user adds an item by taking or uploading a photo, then entering basic details: price, category (top, bottom, shoes, outerwear, etc.), and purchase date if known. Items appear in a simple visual closet view, similar to scrolling through a photo gallery.

Logging wears: Each item has a "wear it today" button. Tapping it logs a wear with today's date, no extra steps required. For items already owned before starting to use the app, users can bulk-log an estimate instead of starting from zero, entering something like "worn about 15 times this year" to get a reasonably accurate cost-per-wear right away.

Seeing the numbers. A dashboard shows each item's cost-per-wear and wears-per-week/month updated automatically as new wears are logged. Items are sortable and rankable, so a user can quickly see their best-value pieces (low cost-per-wear) and their least-used ones (high cost-per-wear or zero wears logged). A summary view shows overall closet stats: total spend, average cost-per-wear, and spending broken down by category.

Spotting patterns over time: As data accumulates, users can see trends like which categories they get the most value from, which purchases are collecting dust and might be worth donating, selling, or re-wearing more intentionally.

The overall result is meant to be a simple, ongoing habit. Log a new item when you buy something, tap a button when you wear something, and check the dashboard when debating a new purchase or what clothes to get rid of.

## Scope

We think this fits a team of 4-6 over one semester, big enough to be real but not so big we're setting ourselves up to fail.

The core version, logging items, logging wears, and a cost-per-wear dashboard, doesn't need any scraping, outside APIs, or machine learning. It's all our own data, and the actual work is stuff we know how to do like photo uploads, storing and updating items and wear logs, and some math and sorting for the dashboard. That keeps us from depending on things outside our control, like a scraper breaking or an API changing, and lets us spend our time actually building and polishing the app.

It presents a reasonable challenge in figuring out how bulk-logged estimates should work next to exact daily logs, building a dashboard that tells you something useful, and making logging easy enough that people actually keep doing it are all real problems we'll have to think through.

If we finish the core functionality with time left, there's a clear list of what to add next: outfit suggestions based on stuff you're not wearing, alerts for things you haven't touched in months, or maybe a way to export or share your data. None of that is required for the app to work and be demoable, but it gives us somewhere to go if things go well.
