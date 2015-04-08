---
layout: event
category: event
title: maptimeLEX April 2015 Meetup
rsvp: https://www.eventbrite.com/e/geospatial-analysis-w-turfjs-tickets-16509164355
---

Mike Dillion will introduce [TurfJS](http://turfjs.org/), a powerful, new JavaScript library for doing geospatial analysis in the browser. We'll be meeting at 6:45 PM on Wednesday, April 15th at [CirrusMio](http://cirrusmio.com/) (154 Constitution St). 

[![http://cirrusmio.com/](http://maptime.github.io/lexington/img/cirrusmio_logo_full.png) ](http://cirrusmio.com/)

Grow the buffest buffers, aggregate point data to the hexiest hex-bins, and find the centroid you're looking for all without expensive, resource-intensive GIS software. Mike will show us how to set up a TurfJS project, give us a look at some of its most useful functions, and how to use TurfJS for some nifty spatial analysis! While a basic understanding of GIS and JavaScript concepts won't hurt, newbies of all stripes are welcome. RSVP on [Eventbrite](https://www.eventbrite.com/e/geospatial-analysis-w-turfjs-tickets-16509164355) and let's tread the greener pasture together and learn TurfJS! 
 

## tl;dr

- What: Geospatial Analysis with TurfJS
- When: 6:45-9:00, Wednesday, April 15th
- Where: CirrusMio, 154 Constitution St, Lexington, KY 40507
- Who: Anyone who wants to learn a new way to do simple to complex geospatial analysis in their browser using JavaScript!
 
In line with the general spirit of maptime, we want this and all our meetups to be welcoming to people of all backgrounds and skill levels. If you're more used to desktop GIS with ESRI products or QGIS, come out and learn! If you're JavaScript wizard, we want you too! A laptop will be necessary for following along. If you don't have access to one, feel free to contact us and we'll work to hook you up with a computer for the meetup.

If you have any questions or concerns, don't hesitate to drop us an email or contact us via twitter. We look forward to seeing you on 4/15!

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