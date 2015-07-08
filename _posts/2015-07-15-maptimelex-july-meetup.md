---
layout: event
category: event
title: maptimeLEX July 2015 Meetup
rsvp:http://www.eventbrite.com/e/maptimewet-tickets-17683478761
---

For our July meetup we're going to be having a change of venue and format. We'll be meeting Wednesday, July 15th at 7:00PM at Third Street Stuff. The theme for the night is maptimeWET. More specifically, we'll be talking water and maps! Guerrilla Cartography, the folks behind the volunteer-driven Food: An Atlas have returned with a new call for proposals, this time on the theme of water. For this meetup we'll be getting together to brainstorm a maptimeLEX map proposal for the forthcoming Water: An Atlas. Proposals are due September 1st, but it's not too early to play Marco Polo with that next big cartographic idea. So come join and let's sea what we can come up with!

A laptop will be helpful, but not necessary this time around. If you don't have access to one, but would like to use one, please let us know and will get you set up. 
 

## tl;dr

- What: maptimeWET!
- When: 7:00-9:00, Wednesday, July 15th
- Where: Third Street Stuff, 257 N Limestone, Lexington, KY 40507
- Who: ALL!
 
In line with the general spirit of maptime, we want this and all our meetups to be welcoming to people of all backgrounds and skill levels. 

If you have any questions or concerns, don't hesitate to drop us an email or contact us via twitter. We look forward to seeing you on 6/24!

<div id='map' class='row8 fill-blue col12 map space-bottom2'></div>
<script>
var map = L.mapbox.map('map', 'maptastik.j354k5k8')
    .setView([38.04746, -84.49253], 17);

var marker = L.mapbox.featureLayer({
  'type': 'Feature',
  'properties': {
    'title': 'Third Street Stuff',
    'description': '257 N Limestone,<br>Lexington, Kentucky<br>40507',
    'marker-color': '#ff8888'
  },
  'geometry': {
    'type': 'Point',38.04940538.04746]
  }
}).addTo(map);

marker.eachLayer(function(m) {
    m.openPopup();
});
</script>