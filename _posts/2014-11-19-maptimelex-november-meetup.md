---
layout: event
category: event
title: maptimeLEX Decembe 2014 Meetup
rsvp: https://www.eventbrite.com/e/gitting-to-know-you-getting-to-know-all-about-git-tickets-14153588765
---
![](https://raw.githubusercontent.com/maptime/lexington/gh-pages/img/maptimelex_20141119_card1.png)

We're going to be doing something a little different for November's. Instead of a maptimeLEX-only event, the meetup is being cross-promoted to other tech groups in Lexington, including [LexLadiesCode](http://lexladiescode.org/). Past maptimeLEX attendee [Mike Dillion](http://mikedillion.com/) ([CirrusMio](http://cirrusmio.com/)) is going to be giving an introduction to some of the key concepts behind [git](http://git-scm.com/), a revision control system, and the popular software, [Github](https://github.com/). While, the discussion won't be just about maps, Github offers lots of support and features that make it a great tool for hosting spatial data. You can even use it to make your own website to present your cartographic masterpieces! It all starts at 6:00 PM on Wednesday, November 19th at the [Plantory](http://plantory.org/). Space is limited so be sure to [RSVP on Eventbrite](https://www.eventbrite.com/e/gitting-to-know-you-getting-to-know-all-about-git-tickets-14153588765). We hope to see you there!

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.059522, -84.492316], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'The Plantory',
    'description': '501 W6th St,<br>Ste 250 <br>Lexington, Kentucky<br>40508',
    'marker-color': '#ff8888'
  },
  'geometry': {
    'type': 'Point',
    'coordinates': [-84.492316, 38.059522 ]
  }
}).addTo(map);

marker.eachLayer(function(m) {
    m.openPopup();
});
</script>
