Amazon [describes Amzn-SearchBot](https://developer.amazon.com/amazonbot) as follows:

> Amzn-SearchBot is used to improve search experiences in Amazon products and services. By permitting Amzn-SearchBot access to your website, your content is eligible to appear in search experiences such as Alexa.  If robots.txt files don’t mention Amzn-SearchBot but allow other search bots, Amzn-SearchBot will crawl in accordance with the robots.txt directives given to other search bots.  Amzn-SearchBot does not crawl content for generative AI model training. 

I allow Amzn-SearchBot on my two sites because (1) it is not used for AI training; (2) it respects robots.txt; and (3) it may allow my work to turn up in certain Amazon searches (unlikely, but I would not want to abandon the Alexa owners out there).

Unfortunately, I discovered that Amzn-SearchBot has two flaws. Firstly, it can be a bit aggressive. Secondly, it is incomprehensibly stupid. But it does obey robots.txt, albeit it does not follow crawl-delay. I implemented the following robots.txt rules on The New Leaf Journal to control its crawling behavior:

```
User-agent: Amzn-SearchBot
Disallow: /?
Disallow: /feed
Disallow: /feed/
Disallow: /*feed
Disallow: /*feed/
Disallow: /category/
Disallow: /page/
Disallow: /tag/
Disallow: /wp-content/
Disallow: /wp-json/
Disallow: /2020/
Disallow: /2021/
Disallow: /2022/
Disallow: /2023/
Disallow: /2024/
Disallow: /2025/
Disallow: /2026/
```

Lest sometime thinks that I just threw the kitchen sink at Amzn-SearchBot, I will have you know that I implemented all of those rules based on its actual crawling behavior. I am not including these rules in my repo because they are site-specific, but for anyone who wants to allow Amzn-SearchBot, I would recommend studying its crawling behavior and "focusing" it through robots.txt rules.