---
layout: post
title:  "Trick2g Site Project Documentation"
date:   2018-12-12 15:54:37 +0800
---


#### Goal: Making a site that integrate trick2g's youtube channel as well as twitch.tv channel, so people can come to this site and watch both feeds at the same time.

## Version 1
* Embed youtube videos as well as twicth.tv section into my site.
* Project Repo is [here](https://github.com/zhouxiang19910319/trick2g_site)

## Version 2 (**on work**)
* Re-wrote everything in the javascript file, using vanilla javascript (ES6) to pull data from youtube's server, feeds off those data into the DOM. ✅
* Add in the trick2g youtube comments quote section into the site. ✅
* Project Repo is [here](https://github.com/zhouxiang19910319/trick2g_site_2)

## Features Pending to be added in Version 3?
1. Make the youtube playlist section an infinite scroll one. Utilizing `nextPageToken` as well as `prevPageToken` ?? 
2. Remove bootstrap(hence jQuery) and use CSS grid to re-build the UI.
3. Gives users the ability to log in using their own twitch.tv account as well as youtube account. (is this really necessary?)
4. Make the quote machine a random quote machine.✅
5. Utilize netlify's platform convert this to a serverless site. Hence store the API key in a safer place.