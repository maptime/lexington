---
layout: post
title: October Meeting Recap
author: Ryan Cooper
---

maptimeLEX had its second official meetup on Wednesday, October 15th at Awesome Inc. Before talking about our meetup I just want to give them a a huge thanks to Awesome Inc for donating the space. If you want to learn about Awesome Inc and the cool things they're doing to in Kentucky to get kids coding and fostering the development of startups, [check them out](http://www.awesomeinc.org/).

![Awesome Inc is awesome](http://maptime.github.io/lexington/img/awesomeinc_square.png)

We had another solid showing of 14 this time around. We were also psyched to be a part of a #sextuplemaptime turned #septuplemaptime.

![SEXTUPLEMAPTIME WAS ACTUALLY SEPTUPLEMAPTIME!](http://maptime.github.io/lexington/img/sextuple.gif)

Sorry we missed the memo, maptimeBoulder!

###CartoDB Tutorial

Our October meetup was split into two halves. For the first part I introduced [CartoDB](http://cartodb.com/) using [Chris Henrick's](https://twitter.com/chrislhenrick) (of [maptimeNYC](https://twitter.com/MaptimeNYC)) [tutorial](https://github.com/maptime/cartodb-tutorial). It's not only a really great walk-through of some of the capabilities of CartoDB as a platform, but also the practicality of the examples seemed to get folks asking spatial questions beyond those in the tutorial. It was clear that there was some interest in the myriad capabilities of PostGIS that underlie CartoDB. Indeed, that's a topic for a future maptimeLEX!

After walking through the CartoDB tutorial, the remaining maptimers (a few had to leave early) grouped up for some collaborative mapping to try and get their hands dirty with the tool they'd just learned. The collaborative mapping time was loosely based on [FloatingSheep.org's](http://www.floatingsheep.org/) [IronSheep mapping competition](http://www.floatingsheep.org/2012/01/iron-sheep-has-landed-location.html). Held concurrently with the annual Association of American Geographers conference, IronSheep essentially consists of a thematic pool of geotagged Twitter data, some sort of prompt, and groups of people who have likely neither worked together, nor have the same skill sets. Over a a few short hours each group is meant to create an interesting map (or set of maps) that address the year's theme. [While this kind of event often times results in patently absurd cartographic productions](http://www.slideshare.net/matthewzook/for-website-debriefing-ironsheep-2013), the format worked well for our meetup because it forced people to just try and make something, *anything*. So with all that explaining of why we did this type of collaborative mapping, let's see some results.

###Collaborative Mapping Activity

#####Collaborative Mapping Prompt

Kentucky Proud, the state organization tasked with promoting Kentucky-made products paid millions of dollars to a consulting firm to put together a marketing plan to promote fear-based tourism. After a year of work, the agency came up with a genius plan: 

*Kentucky Scared: In a **Boograss** State of Mind*.

![Kentucky Scared. Marketing at its best](http://maptime.github.io/lexington/img/KentuckyScared-mess.jpg) 

But after getting paid for coming up with the marketing slogan, the agency folded up shop and went for a cocaine fueled binge on a yacht somewhere in the Gulf and never returned. Left without anything but a crappy riff on their existing brand name, maptimeLEX was approached by Kentucky Proud to create some maps to help promote scary tourism in the Bluegrass.

#####Collaborative Mapping Data

All groups had access to a variety of data sets to get them started. Some were your typical base reference data (counties, state outline, etc.), but I also included some datasets somewhat related to the fear theme. All the data can be accessed [here](https://github.com/maptimelex/maptimelex.github.io/tree/master/cartodb-tutorial/data).

#####Collaborative Mapping Results

We had two groups of three and one group of four. Each had about an hour to work together, brainstorm ideas and make some maps. I'll be the first to admit that maybe this was not enough time for it to be a truly group effort in terms of a single final map, but working in groups did allow for people to bounce questions off one another. In that way I think it was a success! Also, maps were made! Here they are (I've included links to the maps on CartoDB as well as our website's page width doesn't do them all justice):

Jessi Breen and her group submitted this map of ghost sightings per county. This was probably the most advanced map as the original ghost sightings count data were at the town/city scale. They used the spatial join technique to aggregate to the county level. Good job, group!

<iframe width='100%' height='600' frameborder='0' src='http://jessicabreen.cartodb.com/viz/2511150c-54cd-11e4-812d-0e4fddd5de28/embed_map' allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
[See it here!](http://jessicabreen.cartodb.com/viz/2511150c-54cd-11e4-812d-0e4fddd5de28/public_map)

Kenny Stancil and his group created a frightening map of graveyard intensity. We all noted how interesting it was that Lexington seemed bereft of graveyards. I noted that the data were from OSM and there's a distinction between tags and geometry for graveyards and cemeteries. At any rate, the map really captures the fire and brimstone landscape of Kentucky's underworld! 

<iframe width='100%' height='600' frameborder='0' src='http://kwstancil.cartodb.com/viz/e8e82e3c-54cf-11e4-84b0-0e018d66dc29/embed_map' allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
[See it here!](http://kwstancil.cartodb.com/viz/e8e82e3c-54cf-11e4-84b0-0e018d66dc29/public_map)

We actually got two maps out of my group, not to brag. One group member, who chose to remain nameless, created this map of bike trails in Lexington with spooky Halloween colors. It serves as a stark reminder to drivers of the ever-present dangers they face by encroaching bicyclism. Scary stuff!

<iframe width='100%' height='600' frameborder='0' src='http://velognome.cartodb.com/viz/771ddfb6-54cc-11e4-812d-0e4fddd5de28/embed_map' allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
[See it here!](http://velognome.cartodb.com/viz/771ddfb6-54cc-11e4-812d-0e4fddd5de28/public_map)

The other map out of our group was this BigBroLex map. OK, I made it, but the group supported me. Anyway, it is a map of the traffic cameras in Lexington, always there to remind you of the state's surveillance. We are made panoptical zombies by the ever-possibly watchful eyes in the sky. 

<iframe width='100%' height='600' frameborder='0' src='http://maptimelex.cartodb.com/viz/0c2bde88-54cc-11e4-8df0-0e4fddd5de28/embed_map' allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
[See it here!](http://maptimelex.cartodb.com/viz/0c2bde88-54cc-11e4-8df0-0e4fddd5de28/public_map)

With the late submission, Andy Schooner gave us this great Colonel Sanders laying in state map. Personally, I love the stained glass aesthetic for the county fill. There's an eery somberness to it. I was moved.

<iframe width='100%' height='600' frameborder='0' src='http://ashooner.cartodb.com/viz/fe56e776-54d0-11e4-957e-0e9d821ea90d/embed_map' allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>
[See it here!](http://ashooner.cartodb.com/viz/fe56e776-54d0-11e4-957e-0e9d821ea90d/public_map)

###Closing Remarks

So that was the maptimeLEX that was. We're shooting to meet Wednesday, November 19th for our next meetup. Jessi Breen is going to be teaching us how to get up and running with postegres and PostGIS. We're solidfying some last details and will have everything posted as soon as possible. Be on the lookout! Until then, happy mapping!
