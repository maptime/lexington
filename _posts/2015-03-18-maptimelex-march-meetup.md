---
layout: event
category: event
title: maptimeLEX March 2015 Meetup
rsvp: https://www.eventbrite.com/e/march-2015-meetup-squirrel-revenge-tickets-16047717154
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/rgQKYdT1v5Y" frameborder="0" allowfullscreen></iframe>

Over the past two months, friendly sparring with maptimeBoston has become an all out #maptimewar! maptimeBoston have lobbed [maps](https://twitter.com/maptimeBoston/status/568509010946756608), [graphs](http://www.graphicarto.com/wp-content/uploads/2015/02/maptimewar.png), and [insults](https://twitter.com/awoodruff/status/568154984493268992) at us just to suggest we are weak and that rats are better than squirrels. IT ENDS NOW! 

[![http://cirrusmio.com/](http://maptime.github.io/lexington/img/cirrusmio_logo_full.png) ](http://cirrusmio.com/)
Join us at [CirrusMio](http://http://cirrusmio.com/) on Wednesday, March 18 at 6:45 and take a stand against those Beantown rat wranglers. We'll be using [CartoDB's](http://cartodb.com/) story map platform, [OdysseyJS](http://cartodb.github.io/odyssey.js/), to create rebuttals to maptimeBoston's incessant attacks. We'll also have pizza, coincidentally, courtesy of CartoDB! So, come make a map, fill your belly, and proclaim with your cartobrothers and cartosisters:

<h1 style="text-align:center;font-family:Comic Sans MS, sans-serif;">"Squirrels rule, rats drool!"</h1>

![](http://maptime.github.io/lexington/img/squirrel-king-icon-tease.png)  

Seats are limited so be sure to RSVP on [Eventbrite](https://www.eventbrite.com/e/march-2015-meetup-squirrel-revenge-tickets-16047717154).
 

##tl;dr##

- What: Squirrel Revenge w/ OdysseyJS
- When: 6:45-9:30, Wednesday, March 18th
- Where: CirrusMio, 154 Constitution St, Lexington, KY 40507
- Who: Anyone who wants to learn a simple, effective mapping tool; anyone who wants free pizza; anyone who wants to protect the honor of Lexington and its squirrels against the rat hordes of Boston! 
 
In line with the general spirit of maptime, we want this and all our meetups to be welcoming to people of all backgrounds and skill levels. That includes Bostonians! If you've never used or heard of GIS, come out and learn! If you've got your GISP certificate, we want you too! A laptop will be necessary for following along. If you don't have access to one, feel free to contact us and we'll work to hook you up with a computer for the meetup.

If you have any questions or concerns, don't hesitate to drop us an email or contact us via twitter. We look forward to seeing you on 2/18!

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