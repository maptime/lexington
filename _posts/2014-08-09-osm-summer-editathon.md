---
layout: event
category: event
title: OpenStreetMap Summer Editathon
rsvp: https://www.facebook.com/events/286882241497292/
---

Come help us celebrate OpenStreetMap's 10th birthday by quite literally putting Lexington on the map! Bring an internet ready laptop and we'll show you how to edit the world's largest user-generated map. No experience necessary! Rumor has it there will be cake...

*  When: Saturday, August 9th, 12:00 - 4:00 PM
*  Where: 501 W Sixth St Suite 100, Lexington, Kentucky 40508
*  Who: Anyone! From kids, Millenials, Baby Boomers, the Greatest Generation, and even Gen-Xers! This is a family friendly event and OSM is super easy to edit.
*  Why: It's the 10th birthday of OSM. We should shower it with gifts of edits!

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.059420, -84.491778], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'West Sixth Brewing',
    'description': '501 W Sixth St Suite 100,/nLexington, Kentucky/n40508',
    'marker-color': '#ff8888'
  },
  'geometry': {
    'type': 'Point',
    'coordinates': [-84.491778, 38.059420 ]
  }
}).addTo(map);

marker.eachLayer(function(m) {
    m.openPopup();
});
</script>