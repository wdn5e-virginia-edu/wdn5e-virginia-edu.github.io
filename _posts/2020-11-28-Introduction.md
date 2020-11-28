---
layout: post
title: Intro
---

Progressive Web Apps involve javascript and several other standard web technologies:
* *scope* to associate a PWA with its origin and optionally to coordinate several PWAs from the same origin
* PWA-centric *cache* of app assets (the images and other resources needed by the web app)
  * to ensure offline availability
  * in API-accessible storage
  * more configurable than ordinary browser cache
  * programmatically available to javascript, both in the main UI thread and in a
* *service worker* in a separate special-purpose thread
* *worker* threads to offload and separately run other javascript which also might stall the UI
* an event-based *fetch API* to replace AJAX APIs to include 
  * listening for these events, primarily in the _service worker_ as well as 
  * creating these events, primarily in main-thread UI code

Using these, PWA service workers can go beyond simply caching their assets, to proxy main-thread HTTP requests or even service them, providing a local web service for custom use.

Originally an acronym for Accelerated Mobile Pages, AMP improves app performance by
* proscribing worst practices
* prescribing best practices
* providing its own support javascript
* and more performant replacement tags for some HTML element

Initially allowing no app javascript beyond simple UI event handlers,
AMP now allows app javascript
* associated with custom app UI components
* triggered by user actions
* run in separate _worker_ threads

Succeeding amppwa.app posts, sample code, and working apps build upon these ideas.
There may be more PWA than AMP.  I will try for freely usable code.

* Search again every other week or so for new posts here or apps.
* Or to save that bother, [let me know](mail:niebel@virginia.edu) to send you brief mail without ad content at each post or app update.
* In an early upcoming post, I'll try to work web *Notifications and Web Push* into my service worker/s 
  * to make it easier for you to keep tabs on this work

Bill




