-> ON REFRESH
collector  POST -- is initiated by main.min.js -- identified PX file -- the big boy 
bugsnag POST -- may be of importance
6 POST -- Based on stripe, might be important -- does canvas fingerprinting - doesn't matter. Refferer is not goat, its stripe (in request headers)
*random letters and numbers* POST -- seems to track cookie, probably not important
Events POST -- has some info it sends, might be important
Forwarding POST -- probably not important

-> COLLECTOR NOTES
- gets plugins, navigator, screen data, touchpoints, platform, language, product sub, app version, geolocation, mimetypes, build ID, color depth, battery, hardware concurrency, device pixel ratio, local storage

-> BUGSNAGS.JS
- line 200 -- mentions bugsnags js
- line 1269 -- sets user agent tostring()
- line 1320 -- creates fingerprint ID, mentioned its likely not going to generate the same fingerprint 
- line 1327 -- cuid might be something to look at?
- line 2009 -- there's a JSON payload that keeps appearing
- line 2123 -- sets user agent with nav. along with language stuff -- good info in debug
- line 4179 -- gets webgl vendor, canvas, ect. Maybe it matters

-> MAIN.MIN.JS
- line 890-894 -- nav properties very beginning
- line 2429 -- first mention user agent
- line 2778 -- timing stuff, might track timer per actions
- line 3381 -- nav plugins
- -  line 3453 -- function yc(t) motherload, massive nav and window property grabber 
- line 3551 -- function kc(t) checks for all browser automations
- line 4040 -- goes into webgl and canvas 

-> MAIN.MIN.JS PAYLOAD POINTS OF INTEREST
- - t is the payload
- - n is pushing stuff to t
- line 3502 -  

- line 3351 -- t is passed into the finction, and its found that its packed with values
- line 3472 -- pushing more stuff in there for t 
- line 3485 -- t is definately what yuoi are looking for, 
- line 3593 -- puts a lot more data in t
- line 4045 -- webgl rendering





-> functions to look at  
dE
rE
EE
mE
hE






- 1272 seems interesting find


- normally reads only to like 2483 it seems
