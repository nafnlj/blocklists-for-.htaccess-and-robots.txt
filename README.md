# My .htaccess and robots.txt blocklists

This repository contains .htaccess and robots.txt rules I use on The New Leaf Journal (https://thenewleafjournal.com/) and The Emu Café Social (https://social.emucafe.org/).

I had previously used a slightly modified version of the very good ai.robots.txt lists (https://github.com/ai-robots-txt/ai.robots.txt). However, because my own blocking goals are a bit different than ai.robots.txt, I decided to start maintaining my own lists based on their .htaccess/robots.txt style.

My initial lists were based on ai.robots.txt, my observations of New Leaf Journal's server logs, and researching agents and bots on https://knownagents.com/agents.

In general, I try to block AI training bots/scrapers while allowing traditional search indexing and AI "search" (such as it is). My lists also include other bots and crawlers that I consider suspect or unwanted for one reason or another.

I have also included my modifications to the USER AGENT section of Jeff Starr's indispensible 8G Firewall (https://perishablepress.com/8g-firewall/). I removed user agents that are handled by my modified version of the ai.robots.txt rules and I removed a few UAs that I either address through my own robots.txt directives or that I do not want to block as a general matter.

My lists are free to use as is or with modifications. For whatever it is worth, I think my lists may be a good starting point for any webmaster whose blocking goals are in line with my own, but I would encourage anyone to go through my list carefully and make any necessary modifications before putting to use in a production site.

Readers may also be interested in my "Notes" folder, which consist of small markdown files with thoughts on various bots/scrapers, some of which are not on my block lists.
