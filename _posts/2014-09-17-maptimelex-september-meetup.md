---
layout: event
category: event
title: maptimeLEX September Meetup
rsvp: https://www.eventbrite.com/e/maptimelex-september-meetup-tickets-12944367953
---

We'll be holding our first official meetup at the Lexington Public Library, Central Library, Conference Room B. We'll be starting at 6:45 PM with an opening presentation about maptime followed by introductions and a primer on the anatomy of a webmap. Bring your laptop and be ready to do some mapping! Whether you're a map nerd who wants to learn about how all the cool webmaps you use work, a developer looking to explore the exciting geo-realm, or something else entirely, this meetup will be for you. We look forward to seeing you there!

*  When: Wednesday, September 17th, 6:45 - 8:00 PM
*  Where: Lexington Public Library, Central Library, Conference Room B, 140 E Main St, Lexington, Kentucky 40507
*  Who: Anyone with an interest in maps!
*  Why: This is a great chance to learn about the webmaps while also engaging with folks from different backgrounds who have an interest in the world of webmaps too.

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.045717, -84.496713], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'Lexington Public Library, Central Library',
    'description': '140 E Main St,<br>Conference Room B<br>Lexington, Kentucky<br>40507',
    'marker-color': '#ff8888'
  },
  'geometry': {
    'type': 'Point',
    'coordinates': [-84.496713, 38.045717 ]
  }
}).addTo(map);

marker.eachLayer(function(m) {
    m.openPopup();
});
</script>