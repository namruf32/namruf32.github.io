---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
title: Lake Cavanaugh Fire Department
permalink: /fire/

classes: wide
sidebar:
  nav: "fire"
---
<style>
#training {
  border-collapse: collapse;
  width: 100%;
}

#training td, #training th {
  border: 0px solid #ddd;
  padding: 8px;
}

#training tr:hover {background-color: #ddd;}

#training th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #D8EBF1;
  color: black;
}

</style>
## Trained Emergency Responders
Our experienced emergency responders at Lake Cavanaugh are here to help with medical and fire emergencies.

### About the Fire Department
Volunteer Firefighter/EMT’s spend considerable personal time each year training for and responding to emergency incidents. These friends and neighbors drop whatever they’re doing — night or day, holiday’s, bad weather or good — to respond to the community’s emergencies. It’s reassuring to know when you or a loved one is having a medical emergency; is in a car wreck, or your house is on fire, that trained, experienced, volunteer emergency responders will be there in a matter of minutes.

### Volunteer
Consider volunteering for the Lake Cavanaugh Fire Department. It’s rewarding and doesn’t take as much time as you think. Not everyone has to carry a fire hose into a burning house; anyone over 18 can contribute to the emergency response effort. Please stop by the Lake Cavanaugh Fire Station during one of our drill nights at 6:00 pm or call Scott Lemke 360-303-3997. Click here to see a list of our current volunteers.

### {{ "now" | date: "%Y" }} Drill Schedule

<table id="training">
  {% for training in site.data.lcfd.training_schedule %}
  <tr>
    <th style="text-align: center">{{ training.month }}</th>
    <th class="title"></th>
  </tr>
    <td style="text-align: center"><b>{{ training.first_training_date }}</b></td>
    <td>{{ training.first_training }}</td>
  <tr>
    <td style="text-align: center"><b>{{ training.second_training_date }}</b></td>
    <td>{{ training.second_training }}</td>
  </tr>
  {% endfor %}
</table>

### Events
Take advantage of our big summer events, like the Fire Department Open House, Fill the Boot, and the Once Around Lake Cavanaugh Fun Run. Check out the Events Calendar for a list of current events around the lake.

### Tips for Fire Safety
* Always check the Fire Marshal Website for the most up to date burn ban information
* Green flashing lights on a vehicle indicate a volunteer is responding to a call
* Spring is the time to replace smoke detector batteries
* Remember that the roads are narrow, so be careful when parking along them
* After the snowy winter, make sure your address sign is visible from the road this also might be a good time to clean and inspect your chimney