---
layout: event
category: event
title: maptimeLEX November 2014 Meetup
rsvp:
---

It's time for the second meeting of maptimeLEX. Last month's meetup downtown at the Lexington Public Library was a wonderful time. This month, we'll be moving a little bit east on Main Street to Awesome Inc's headquarters. Like last time, we'll begin in the conference room at 6:45.

We'll begin with a walk-thru of a cool web mapping platform called CartoDB. With our newly minted web mapping skills, we're going to engage in some fun group mapping modeled after the [IronSheep competition](http://www.floatingsheep.org/2013/06/the-maps-of-ironsheep-2013.html) developed by [FloatingSheep](http://www.floatingsheep.org/). Within groups of 2-3, we'll work to produce creative web maps in the spirit of the Halloween season. maptimeLEX will provide some data to get you going, but feel free to bring your own along with you if you'd like! We'll come back together at the end for lightning talks during which each group will have just a short amount of time to present their map. It should be a magnificent macabre mapping menagerie! 

A couple of things to make sure you can have the best experience at this meetup:


1. Space is limited so make sure you RSVP on [Eventbrite](https://www.eventbrite.com/e/maptimelex-october-meetup-tickets-13426040649).
2. You'll want to [sign up for a free CartoDB account](http://cartodb.com/). They have a pretty generous free plan that will be more than sufficient for what we'll be doing. 
2. Bring a laptop.  If you don't have access to one, let us know (maptimelex@gmail.com) and we'll be happy to work with you to get a hold of one for the evening.

### The Essentials ###
*  When: Wednesday, October 15th, 6:45 - 9:30 PM
*  Where: Awesome Inc, 348 E Main St, Lexington, Kentucky 40507
*  What: CartoDB and frightening mapping fun!['Boo!'](img/ghost.gif)
*  Who: Anyone with an interest in maps. All skill levels and backgrounds welcome!

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.042015, -84.492637], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'Awesome Inc',
    'description': '348 E Main St,<br>Conference Room <br>Lexington, Kentucky<br>40507',
    'marker-color': '#ff8888'
  },
  'geometry': {
    'type': 'Point',
    'coordinates': [-84.492637, 38.042015 ]
  }
}).addTo(map);

marker.eachLayer(function(m) {
    m.openPopup();
});
</script>