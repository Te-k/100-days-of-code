# 100 Days Of Code - Log

### Day 1: January 17th, 2017

**Today's Progress**: I developed a [script](https://github.com/Te-k/analyst-scripts/blob/master/misp/yaraxcheck.py) to check sample hosted in MISP with yara rules. I had to add the [download feature](https://github.com/Te-k/python-misp/commit/dd7e56e2bb612618d0d74f27241c36e3180e1674) to [python-misp](https://github.com/nbareil/python-misp) for this.

**Thoughts:** Lot of motivation, but I am not learning that much when doing such script (I have already used python-misp and python-yara a lot)

**Code:**

* [python-misp](https://github.com/Te-k/python-misp)
* [yaraxcheck.py](https://github.com/Te-k/analyst-scripts/blob/master/misp/yaraxcheck.py)
* [idea](https://github.com/Yara-Rules/rules/issues/152)

### Day 2: January 18th, 2017

**Today's Progress**: I added client side password strength estimation using [zxcvbn](https://github.com/dropbox/zxcvbn) in OpenOversight. I learned how to do [rainbows](https://jsfiddle.net/oLz2hgxp/)

**Thoughts:** I hate CSS

**Code:**

* [commit](https://github.com/Te-k/OpenOversight/commit/0b3f17ededcb0d223a160bdbad67f03e4d2909be)

**Docs**:

* [Password Strength meter](https://css-tricks.com/password-strength-meter/)
* [HTML5 Meter element](https://css-tricks.com/html5-meter-element/)

### Day 3: January 19th

**Today's Progress**: I started to rewrite my HTTP scanner with more ideas, it need a bit more work but it will be functional soon (although some ideas I have will be hard to implement)

**Code:** Not published yet, hope to have a v1 tomorrow

### Day 4: January 20th

**Today's Progress**: Damn it seems harder than I thought, there are much more options and the code seems more tricky. HTTPs is a mess and request does not allow to get the certificate ([Issue here](https://github.com/kennethreitz/requests/issues/3826) and it will be a mess to parse the certificate anyway. All this is Trump's fault

**Code:** Grrr

### Day 5: January 21th

**Today's Progress**: I had some comments on my commit to [python-misp](https://github.com/nbareil/python-misp/pull/4#discussion_r97195404), so I improved the code as proposed, and did a new [pull request](https://github.com/nbareil/python-misp/pull/5). Then did a bunch of work on httpscan, it is crazy that there is no urllib in python allowing to do an HTTP request and get the certificate at the same time. I finally did another request using socket and ssl to have the cert.

**Code:**

* python-misp : [improve attribute download](https://github.com/Te-k/python-misp/commit/73cf9657bef2c13cc3a7215caffa5098fe187769)
* analyst-tools: [update python-misp and adapt yaraxcheck](https://github.com/Te-k/analyst-scripts/commit/697aff90cdb68210e55665ea6a311ba6ca9f4091)

### Day 7: January 23th

**Today's Progress:** I implemented the requests done by redshitzero on OpenOversight [here](https://github.com/lucyparsons/OpenOversight/pull/168). Everything was easy to do, I hope the code will be integrated soon

**Code:** [here](https://github.com/lucyparsons/OpenOversight/pull/168/commits/58679fb7efd952de4838ac0a468ff9a82ecdae0b)

### Day 8 : January 24th

**Today's progress:** Wanted to play with Twitter API but got lost in dirty discord API tests. Will do better tomorrow

### Day 9: January 25th

**Today's progress:** played with gophish to improve my http scanner with phishing kit signatures. Now I have to write signature system :p. Edit: I actually implemented the signature code this night

### Day 11: January 27th

**Today's progress:** Improved and cleaned code of the scanner

**Code**:

* [you can provide a specific signature file for test](https://github.com/Te-k/analyst-scripts/commit/f0ac6efdfff1abf83dd7a5f41c2bc4a22500bce6)
* [replace print by logger](https://github.com/Te-k/analyst-scripts/commit/5770cf0af71393ae3fb901eee01704e5be84e5e0)
* [Add output](https://github.com/Te-k/analyst-scripts/commit/a5e6aa84c12b7b2864e800048b4f2b1fde54abef)
* [cleaning code](https://github.com/Te-k/analyst-scripts/commit/01d21c9e62acd6f41421545a210fd82524a4be0c)

### Day 12: January 28th

**Today's progress:** Did a bit of work on the scanner but quite boring now, and not useful yet, we'll see later to finish it. SSL makes me crazy. Continued to learn Go.

**Code**:

* [Not much](https://github.com/Te-k/analyst-scripts/commit/81c0c83b345191c05928ed1824e0de0424f51ab4)

### Day 14: January 30th

**Today's progress:** Started to play again with Twitter, but it appears that you need a database if you wanna store this, so started to play with mongo engine, and then you also need a cool cli, so I started to look for sub command tools... Never ending quest and I have an ugly partially working code. Will do better tomorrow

### Day 15: January 31th

**Today's progress:** Continued to work on Twitter stuff. I have tosolve this issue with plugins before anything else, and I think that I have find a cool idea. We'll see if it works tomorrow. Oh also, I finally published [pyregripper](https://github.com/Te-k/pyregripper) (which acknowledge the fact that I won't work on it anymore likely).

### Day 11: February 1st

**Today's progress:** Finally managed to have a clear subcommand code for the twitter stuff. Import in the database seems to work, I have to do more tests. Great !

### Day 12: February 2nd

**Today's progress:** Some work done on Twitter to import stuff in mongoengine, still some work to get everything together

### Day 15: February 5th

**Today's progress:** It has been a long week, but I have done some more work with Twitter API. I hate that rate limit

### Day 16: February 6th

**Today's progress:** First useful commands on trickybird, everything seems to work well. I Still have to create more commands and make everything working all together.

### Day 17: February 7th

**Today's progress:** Nothing fancy, but I finally finished my PR for OO, here is the [code](https://github.com/Te-k/OpenOversight/commit/cfa39cb9f58362b4c947d973102a9231aadec9fe)

### Day 22: February 12th

**Today's progress:** Hard to keep up the challenge last week, I will have to do more than 100 days I guess. Today more work on twitter, but I should really work on some interesting example, it would be more fun

### Day 23: February 13th

**Today's progress:** Back on goose check, Javascript is a mess but it starts to work. Still a bit of work, then I will have to clean all that code.

### Day 28: February 18th

**Today's progress:** I know, I know, it was hard this week, but today I am travelling and I like coding in random airports. I have done some cool stuff on the Twitter tool, now I have to fix this damn bugs with tweepy and improve graphics. Almost releasable, still a bit of work !

### Day 29: February 19th

**Today's progress:** It is late but I did it, this Twitter stuff starts to work quite well. Still a bit of work here and there and then play with it

### Day 30: February 20th

**Today's progress:** Done some javascript today, I still hate that language but I get better at making it working. I am still avoiding any design I can but at one point or the other, it will be definitely needed :(

### Day 31: February 21st

**Today's progress:** Ah so cool, now that everything works almost well, it is really easy to biuld new commands, I like it !

### Day 32: February 22nd

**Today's progress:** I did some other stuff today, but I have finally published some tools I developed some years ago to test web servers : https://github.com/Te-k/analyst-scripts/tree/master/httptest

### Day 33: February 23rd

**Today's progress:** Again some twitter done, the tool is working qute well, I still need to do some stuff with it
