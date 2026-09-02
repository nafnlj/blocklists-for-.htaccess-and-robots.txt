# My .htaccess and robots.txt blocklists

This repository contains .htaccess and robots.txt rules I use on The New Leaf Journal (https://thenewleafjournal.com/) and The Emu Café Social (https://social.emucafe.org/).

The main rules are modified from the excellent ai.robots.txt project on GitHub (https://github.com/ai-robots-txt/ai.robots.txt). My lists are smaller and I have adopted a policy of trying to prevent AI training while allowing AI "search" (such as it is). I have also added a few AI and non-AI crawlers that I identified as unwanted and do not (yet?) appear on the ai.robots.txt lists. The ai.robots.txt .htaccess rules are designed to work with robots.txt in that they allow blocked crawlers to access robots.txt. This is good since it prevents well-behaved crawlers that follow robots.txt from spamming the site with 404s (I noted Amazon's bots as one example here). Thus, I also include robots.txt rules consistent with my .htaccess directives. My robots.txt rules also include an additional crawl-delay list for bots not in the original or my modified blocklists.

Finally, I included my modifications to the USER AGENT section of Jeff Starr's indispensible 8G Firewall (https://perishablepress.com/8g-firewall/). I removed user agents that are handled by my modified version of the ai.robots.txt rules and I removed a few UAs that I either address through my own robots.txt directives or that I do not want to block as a general matter.

I am only including .htaccess because that is what I use for my two WordPress sites. However, both ai.robots.txt and Jeff Starr's 8G Firewall are available for various server configurations, so my edits can be adapted to whatever you may be using.

At the moment, I have not published detailed explanations of my edits, but I may do so in the future. Feel free to create an issue if you have questions or suggestions. The Codeberg version of this repository (https://codeberg.org/nafnlj/blocklists-for-.htaccess-and-robots.txt) is canonical.