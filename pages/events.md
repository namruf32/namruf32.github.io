---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Events Spotlight
layout: category
#taxonomy: events
permalink: /events/

classes: wide
sidebar:
  nav: "events"
---
<style>
table, td, th {
  border: 0px solid black;
  font-size: 20px;
  padding: 0px;
}

table {
  border-collapse: collapse;
  width: 100%;
}

#date {
  text-align: center;
  font-weight: bold;
  font-size: 24px;
  padding-right: 30px;
}

#event {
  font-weight: bold;
  font-size: 36px;
}

#event_end {
  border-bottom: 1px solid black;
  padding-bottom: 100px;
}
}
</style>

<table>
  {% for event in site.data.events %}
    <tr>
      <td id="date" ><i class='fas fa-calendar-alt'></i></td>
      <td id="event"><a href = "{{event.link}}">{{ event.event }}</a></td>
    </tr>
    <tr id="event_end">
      <td id="date">{{ event.date }}</td>
      <td>{{ event.description }}</td>
    </tr>
  {% endfor %}
</table>