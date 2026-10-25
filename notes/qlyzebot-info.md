I have QlyzeBot blocked in the "Misc" category. I discovered it on my own in my logs in September 2026. See example UA string:

```
Sep 06 18:05:09 46.4.94.214 - - [06/Sep/2026:22:05:09 +0000] "GET /until-we-meet-again-visual-novel-review HTTP/1.1" 301 - "-" "Mozilla/5.0 (compatible; QlyzeBot/1.0; +https://app.qlyze.io/bot)"
```

As I noted in my commit adding it to my block-list <https://codeberg.org/nafnlj/blocklists-for-.htaccess-and-robots.txt/commit/99638c47df7ee55c7510c60a0478da3087b73c9a>, it *appears* to be a German AI answer bot. I generally allow AI answer bots and search. However, the URL it provides in the UA string, <https://app.qlyze.io/bot>, redirects to a sign-in page. Because it appears to promise information but then puts that information behind a sign-in wall, I erred on the side of caution and blocked it. I may reconsider if the company makes it possible to review information about the bot without requiring sign-in.