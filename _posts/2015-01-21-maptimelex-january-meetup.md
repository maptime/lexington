---
layout: event
category: event
title: maptimeLEX January 2015 Meetup
rsvp: https://www.eventbrite.com/e/going-nuts-with-leafletjs-tickets-15345200909
---

We hope everyone had a great December and that 2015 has gotten off to a fabulous start. Hard to believe there are only 50 weeks left in the year! Anyway, we're having our first meetup of the year on Wednesday, January 21st from 6:45-9:30ish at [Awesome Inc](http://www.awesomeinc.org/).

[![http://www.awesomeinc.org/](http://maptime.github.io/lexington/img/awesomeinc_horizontal.png) ](http://www.awesomeinc.org/)

We're going to be learning about an amazing little JavaScript mapping library called [LeafletJS](http://leafletjs.com/). We'll talk about it more at the meetup, but you can use it to turn your webmap up to 11. And because January 21st is [Squirrel Appreciation Day](http://www.holidayinsights.com/moreholidays/January/squirrelappreciation.htm), we'll celebrate our cute rodent friends by internet mapping them. Look out cats!

![Squirrel eating an acorn](http://maptime.github.io/lexington/img/squirrel_eating_acorn.gif)

Seats are limited so be sure to RSVP on [Eventbrite](https://www.eventbrite.com/e/going-nuts-with-leafletjs-tickets-15345200909).
 


##tl;dr##

- What: Learning about a mapping library called LeafletJS
- When: 6:45-9:30, Wednesday, January 21
- Where: Awesome Inc. Conference Room, 348 E Main St, Lexington, KY 40507
- Who: Anyone who want to make interactive webmaps!
 
In line with the general spirit of maptime, we want this and all our meetups to be welcoming to people of all backgrounds and skill levels. If you've never written a line of HTML, CSS, or JavaScript, come out and we'll be happy to get you going. If you're a savvy developer who wants to learn about some of the particularities of mapping, we want you too! A laptop will be necessary for following along. If you don't have access to one, feel free to contact us and we'll work to hook you up with a computer for the meetup.

If you have any questions or concerns, don't hesitate to drop us an email or contact us via twitter. We look forward to seeing you on 1/21!

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