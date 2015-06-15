---
layout: event
category: event
title: maptimeLEX June 2015 Meetup
rsvp: http://www.eventbrite.com/e/d3js-webmaps-and-you-tickets-17389797352
---

In this [@maptimeLex](https://twitter.com/maptimelex), Rich Donohue ([@rgdonohue](https://twitter.com/rgdonohue)) will (re-)introduce our community to the [D3.js visualization library](http://d3js.org/) and demonstrate its integration into a larger web mapping workflow. Drawing upon Andy Woodruff's ([@awoodruff](https://twitter.com/awoodruff)) excellent [@maptimeBoston](https://twitter.com/maptimeboston) presentation ([http://maptimeboston.github.io/d3-maptime/](http://maptimeboston.github.io/d3-maptime/)), Rich will explain the library's implementation when used to create a simple, interactive web map. He'll then step back to consider where D3 fits within a mapping process using various tools to prepare data, simplify and aggregate geometries, visually render geospatial information within a browser, and build an interface to invite users to more fully engage with the map. Participants will then be supported through a collaborative, workshop-style exercise to make their own interactive maps using D3.

A laptop will be necessary to follow along. If you don't have access to one, please let us know and will get you set up. Although a basic knowledge of HTML, CSS, and/or JavaScript will be helpful, they're not essential. 
 

## tl;dr

- What: D3js, Webmaps, and You
- When: 7:00-9:00, Wednesday, June 24th
- Where: CirrusMio, 154 Constitution St, Lexington, KY 40507
- Who: Like maps? Want to learn how to make them? Then this for you.
 
In line with the general spirit of maptime, we want this and all our meetups to be welcoming to people of all backgrounds and skill levels. If you're more used to desktop GIS with ESRI products or QGIS, come out and learn! If you're JavaScript wizard, we want you too! A laptop will be necessary for following along. If you don't have access to one, feel free to contact us and we'll work to hook you up with a computer for the meetup.

If you have any questions or concerns, don't hesitate to drop us an email or contact us via twitter. We look forward to seeing you on 6/24!

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.04746, -84.49253], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'CirrusMio',
    'description': '154 Constitution St,<br>Lexington, Kentucky<br>40507',
    'marker-color': '#ff8888'
  },
  'geometry': {
    'type': 'Point',
    'coordinates': [-84.49253,38.04746]
  }
}).addTo(map);

marker.eachLayer(function(m) {
    m.openPopup();
});
</script>