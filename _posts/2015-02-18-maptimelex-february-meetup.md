---
layout: event
category: event
title: maptimeLEX February 2015 Meetup
rsvp: https://www.eventbrite.com/e/february-meetup-intro-to-qgis-tickets-15703477524
---

We're happy to announce our February meetup! Please join us Wednesday, Febrauary 18th from 6:45-9:30ish at [CirrusMio](http://http://cirrusmio.com/) when Jessi Breen will introduce us to QGIS.

[![http://cirrusmio.com/](http://maptime.github.io/lexington/img/cirrusmio_logo_full.png) ](http://cirrusmio.com/)

QGIS is a powerful free and open source software (FOSS) GIS application that allows you make create, view, and edit spatial data, create beautiful cartographic creations, and carry out spatial analysis. It is a powerful tool to have in your mapping arsenal and best of all, it's free! Jessi will get us going with the basics of getting spatial data into QGIS and give us peek into its powerful spatial analysis capabilities.  

Seats are limited so be sure to RSVP on [Eventbrite](https://www.eventbrite.com/e/february-meetup-intro-to-qgis-tickets-15703477524).

[![http://www2.qgis.org/en/site/index.html](http://maptime.github.io/lexington/img/QGis_Logo.png) ](http://www2.qgis.org/en/site/index.html)

We also recommend [downloading the latest version of QGIS](http://www2.qgis.org/en/site/forusers/download.html). If you've got Windows, OSX, Linux, or even Android on a tablet, you're good to go!
 


##tl;dr##

- What: An introduction to QGIS
- When: 6:45-9:30, Wednesday, February 18th
- Where: CirrusMio, 154 Constitution St, Lexington, KY 40507
- Who: Anyone interested in learning about QGIS GIS in general
 
In line with the general spirit of maptime, we want this and all our meetups to be welcoming to people of all backgrounds and skill levels. If you've never used or heard of GIS, come out and learn! If you've got your GISP certificate, we want you too! A laptop will be necessary for following along. If you don't have access to one, feel free to contact us and we'll work to hook you up with a computer for the meetup.

If you have any questions or concerns, don't hesitate to drop us an email or contact us via twitter. We look forward to seeing you on 2/18!

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.04746, -84.49253], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'Awesome Inc',
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