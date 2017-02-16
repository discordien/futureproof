---
layout: page
title: Tor
image: assets/images/onion.jpg
description: The Onion Router Protocol
---

# Overview

The Onion Router (colloquilally known as Tor) originated as a project out of the United States Naval Research Laboratory. It is widely assumed that Tor system is used by state actors, activists, privacy advocates, and petty criminals. While the system is not perfect (see later notes on risks), it can vastly improve only privacy if used with certain considerations in mind.

Tor provides a means of obfuscating the originating source of traffic on the public Internet. It does this by breaking up the various network streams, bouncing them around within the Tor network, and finally connecting to the destination server through what is known as an exit node. While Tor is used to provide an aspect of privacy when surving the public Internet, it also provides a framework for hidden services. This is done by an internal DNS system using the TLD of `.onion`. While these connections are still bounced around through the Tor network, the traffic never _leaves_ the network. All communications happen within Tor.

The EFF has some good writeups on how to use Tor.

* [Windows](https://ssd.eff.org/en/module/how-use-tor-windows)
* [macOS](https://ssd.eff.org/en/module/how-use-tor-mac-os-x)

These are some sample hidden services. Note that you will need to be connected to Tor _and_ be using a compatible browser for these links to work.

* [Facebook](http://facebookcorewwwi.onion/) provides a hidden service for use of the social network in regions where such activities are frowned upon.
* [Grams](http://grams7enufi7jmdl.onion/) is basically Google but for generally illegal material.
* ["USSR home computer tape rip"](http://25dxotevqkqyhqgj.onion/) is a site where someone uploaded FLAC of an old data containing Soviet audio tape they found. And a contact form.
* Buzzfeed [SecureDrop](http://6cws3rcwn7aom44r.onion/)
* New York Times [SecureDrop](http://nytimes2tsqtnxek.onion)
* [The Internet Archive](http://archivecrfip2lpi.onion/)

# Risks

The core problem with Tor seems to still be that there is a limited number of exit nodes. Combining this with the fact that state actors are widely assumed to be running a large number of exit nodes and we end up in a situation where it is conceptually possible to match up traffic with the original user. Another risk, which has been actively exploited by law enforcement agencies, is hidden service sites which load resources from the public internet. The FBI used this tactic in [2013](https://www.wired.com/2013/09/freedom-hosting-fbi/) as part of the takedown of the original [Freedom Hosting](https://en.wikipedia.org/wiki/Freedom_Hosting).
