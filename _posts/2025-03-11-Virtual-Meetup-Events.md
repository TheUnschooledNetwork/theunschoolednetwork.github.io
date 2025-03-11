---
title: Virtual Meetup Events
date: 2025-03-09 7:00:00 -500
categories: [Unschooling, Meetups]
tags: [Bitcoin, Lightning, Meetup]
pin: true
---

<style>
    /* Light Theme */
    @media (prefers-color-scheme: light) {
        .fc {
            background-color: var(--color-bg); /* Background color of the calendar */
            color: var(--color-text); /* Default text color */
        }
        .fc .fc-toolbar {
            background-color: var(--color-bg); /* Toolbar background color */
            color: var(--color-text); /* Toolbar text color */
        }
        .fc .fc-daygrid-day {
            background-color: var(--color-bg); /* Day cell background color */
            border: 1px solid var(--color-border); /* Day cell border color */
        }
        .fc .fc-daygrid-day-number {
            color: var(--color-primary); /* Day number color */
        }
        .fc .fc-event {
            background-color: var(--color-accent); /* Event background color */
            color: var(--color-bg); /* Event text color */
        }
        .fc .fc-event:hover {
            background-color: var(--color-accent-hover); /* Event background color on hover */
            color: var(--color-bg); /* Event text color on hover */
        }
    }

    /* Dark Theme */
    @media (prefers-color-scheme: dark) {
        .fc {
            background-color: var(--color-bg-dark); /* Background color of the calendar */
            color: var(--color-text-dark); /* Default text color */
        }
        .fc .fc-toolbar {
            background-color: var(--color-bg-dark); /* Toolbar background color */
            color: var(--color-text-dark); /* Toolbar text color */
        }
        .fc .fc-daygrid-day {
            background-color: var(--color-bg-dark); /* Day cell background color */
            border: 1px solid var(--color-border-dark); /* Day cell border color */
        }
        .fc .fc-daygrid-day-number {
            color: var(--color-primary-dark); /* Day number color */
        }
        .fc .fc-event {
            background-color: var(--color-accent-dark); /* Event background color */
            color: var(--color-bg-dark); /* Event text color */
        }
        .fc .fc-event:hover {
            background-color: var(--color-accent-hover-dark); /* Event background color on hover */
            color: var(--color-bg-dark); /* Event text color on hover */
        }
    }
</style>

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
                    url: '/posts/Virtual-Meetup-Events/#TUBM-1',
                    color: 'var(--color-accent)', // Background color
                    textColor: 'var(--color-bg)' // Text color
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

<a name="TUBM-1"></a>
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