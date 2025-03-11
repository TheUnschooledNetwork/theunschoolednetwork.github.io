---
title: Virtual Meetup Events
date: 2025-03-09 7:00:00 -500
categories: [Unschooling, Meetups]
tags: [Bitcoin, Lightning, Meetup]
pin: true
---

<link href='https://cdn.jsdelivr.net/npm/fullcalendar@5.10.1/main.min.css' rel='stylesheet' />
<script src='https://cdn.jsdelivr.net/npm/fullcalendar@5.10.1/main.min.js'></script>
<script>
    document.addEventListener('DOMContentLoaded', function() {
        var calendarEl = document.getElementById('calendar');
        var calendar = new FullCalendar.Calendar(calendarEl, {
            initialView: 'dayGridMonth',
            height: 'auto',
            eventDisplay: 'block',
            events: [
                {
                    title: 'TUBM 1: The Road to Wider Adoption',
                    start: '2025-03-28T19:00:00',
                    url: '/posts/Virtual-Meetup-Events/#tubm-1-the-road-to-wider-adoption'
                }
            ],
            eventDidMount: function(info) {
                info.el.setAttribute('title', info.event.title);
            }
        });
        calendar.render();
    });
</script>
<div id='calendar'></div>


## TUBM 1: The Road to Wider Adoption

Join the inaugural edition of [TUBM](/posts/The-Unschooled-Bitcoiners-Meetup/)

#### Meetup agenda:

- Video Presentation / Discussion
- Tutorial walk-through: Buying Non-Custodial Bitcoin in Canada
- Tutorial walk-through: getting started with Lighting Network
- Discussion/questions period

#### Date: March 28th
#### Time: 7:00PM - 8:00PM
#### [Join Now](https://hivetalk.org/join/TheUnschooledBitcoiner)