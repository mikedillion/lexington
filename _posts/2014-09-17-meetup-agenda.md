---
layout: post
title: Agenda for 9/17 Meetup
---
<hr>
#Agenda
1. What is maptime? (Dan Cockayne)
1. Who are you? (Everyone!)
1. ["Anatomy of a Web Map"](http://maptimelex.github.io/anatomy-of-a-webmap/ "anatomy of a webmap slides") (Ryan Cooper + whoever else wants to chime in)
1. maptimeLEX brainstorming (Everyone!)
1. ???
<hr>
And just a reminder of the essentials for the meeting-  
Date: 9/27/14  
Time: 6:45 PM - 8:30 PM  
Location: 
Lexington Public Library, Central Library  
Conference Room B  
140 E Main St,  
Lexington, Kentucky 40507

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