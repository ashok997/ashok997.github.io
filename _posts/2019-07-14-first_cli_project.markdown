---
layout: post
title:      "First CLI Project"
date:       2019-07-14 16:52:54 +0000
permalink:  first_cli_project
---


For the first project of our programming class we were asked to build our very own CLI (Command Line Interface) project. Another requirement of the project was to scrape any website for data and to fulfil this requirement I decided to scrape a website to scrape information about the players from Manchester United FC. I had always been a fan of Manchester United FC so building a project about the team I supported was an easy decision.

Even before I started writing a single line of code, my progress was halted by an issue. While I was setting up the project environment I encounter an issue which I had not seen. I asked for help and our technical coach Michael, help me find the way aroung that issue. Feeling overjoyed I started adding lines of codes to my project. But, there was yet another issue! I had decided I would scrape the official page (https://www.manutd.com/) only to discover that the page was very difficult to scrape, I was getting nothing. I panicked and called for help again!! Again Michael, helped me find a similar site that was scrapable, so I settled with this site: (https://www.premierleague.com/clubs/12/Manchester-United/squad). 
After, that I was able to progress without any major issues. I had few issues here and there but again our coach was there to give me the right direction.

One of the interesting issue I had to overcome was getting rid of non-ascii character  and nromalize them for the player url. For example, one of the player was named 'Alexis Sánchez' and that 'á' was throwing an error. I had no idea how to overcome that issue so I asked for help, only this time I looked somewhere else, namely google. I came across interesting solution and decided to use it. 
```
attr('href').unicode_normalize(:nfkd).encode('ASCII', replace: '')
```
I had never seen that method earlier but it got the job done for me. Slowly and steadily, I was able to finish my project but the end result was not pretty.  The code I had ended up with was big lump of disorganized lines of codes. So, my final hurdle was to refactoring the codes. While doing that, I actaully broke my program couple of times but was able to get it back without much hassle. At the end I was able to finish my project on time.
