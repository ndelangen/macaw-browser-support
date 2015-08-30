Macaw Browser Support 'matrix'
==============================

by: norbert de Langen,
state: draft

Why this document
-----------------
Macaw cannot possibly support every release of every browser. Even when limiting to just the 'major' browsers and the 'latest few' releases there are still too many differences in the browsers to implement any design with 100% accuracy or feature coverage.

What can we support?
--------------------
For a long time, it's been the rule to support "all major browser's last 2 versions". Sometimes with exceptions made for some browsers like Internet Explorer.

But with the usage of mobile (and tablet) exploding, the browser market has fragmented significantly. Meaning statements like "supporting android" actually mean having to test a multitude of browsers on possibly hundreds of devices.

Not supporting these devices at all, because they are not "major" browsers should be out of the question, when added up they represent at significant portion of all visits.

What should we support?
-----------------------
Every visitor should be able to get to the content of the site. Unless there is no real content, a message like "your browser is not supported", is just plain terrible for users.

It is acceptable to present a notification to the user that they are not getting the best experience in thei current browser.

How will we support everything?
-------------------------------
We will introduce a tiered support system, based on browser features.

The lowest tier will be the absolute bare minimum, little to no "nice to have"-features, no animations/transitions etc. Designs will not be pixel-perfect implemented.

There can be any number of intermediate tiers.

The highest tier will be implemented pixel-perfect, with all features required by agreed upon.

What features can cause tier-switches?
--------------------------------------
A huge number of variables can be at play in determining the browser tier. This is an incomplete list:

* javascript support
* media-queries support
* css(features) support
* javascript(features) support
* vector image support
* html5 media support
* cookies blocked
* connection speed
* ...

Exceptions
----------
If there's a specific desire for browser-X on device-Y to be in a specific tier (usually the highest tier), special exceptions can be made.

It's essential to know this requirement at the start of the project

Please mind that this is extra work and can really impose a negative performance, and maintenance penalty.

So what tiers are there for Project-Z?
--------------------------------------
It depends.