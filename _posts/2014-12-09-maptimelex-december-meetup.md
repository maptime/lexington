---
layout: event
category: event
title: maptimeLEX December 2014 Meetup
rsvp: https://www.eventbrite.com/e/december-meetup-tickets-14835295769
---

Jessi Breen is going to be walking us through the first steps of building a geostack. What does this mean? We're gonna be downloading OSM data, styling it in TileMill and making some tiles!

Make sure you take care of the pre-meetup installs. The steps are outlined in Eric Theise's ["Let's Talk about Your Geostack" slides](http://erictheise.github.io/geostack-deck/#/). Additionally, you'll need to install [Virtual Box](https://www.virtualbox.org/) and [Vagrant](https://www.vagrantup.com/).

Space is limited so make sure you RSVP on [Eventbrite](https://www.eventbrite.com/e/december-meetup-tickets-14835295769).

As usual, you'll need to bring a laptop.  If you don't have access to one, let us know (maptimelex@gmail.com) and we'll be happy to work with you to get a hold of one for the evening.

### The Essentials ###
*  When: Tuesday, December 9th, 6:45 - 9:30 PM
*  Where: Awesome Inc, 348 E Main St, Lexington, Kentucky 40507
*  What: Building a geostack: Part I
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