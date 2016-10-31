---
layout: default
---

## First Meetup: 15th of December!

The first Meetup will take place the 15th of December, between 7PM and 10PM (local time).

Dashlane will welcome us in their offices, located at the [*21 Rue Pierre Picard, 75018 Paris*](http://www.openstreetmap.org/#map=19/48.88474/2.34489).
The nearest metro station is *Barbès-Rochechouart* (lines 2 and 4).

[Please RSVP on Meetup](https://www.meetup.com/fr-FR/SecParis-Meetup/events/235197208/).

**The call for presentations is OPEN!**

Just drop me a line at [thomas@chauchefoin.fr](mailto:thomas@chauchefoin.fr) or
open a pull request against this repository by adding a
file in the `./talks` folder (follow the `example.md` file).

{% if site.talks.size > 0 %}
Programmed talks:
  <ul>
    {% assign talks = site.talks | sort: 'planned' %}
    {% for talk in talks %}
        {{ talk.planned | date: '%H:%M' }} - <a href="{{ talk.url }}"><i>{{ talk.title }}</i></a> by {{ talk.author }}<br>
    {% endfor %}
  </ul>
{% else %}
  We don't have any talk proposed at the moment.
{% endif %}

## Sponsors

[![Dashlane](./img/dashlane.png)](https://www.dashlane.com/)

[Dashlane](https://www.dashlane.com/) is providing access to their meeting room (capacity 50 people) and some
pizzas and drinks: thanks to them!
