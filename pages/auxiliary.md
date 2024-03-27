---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
title: Auxiliary Mission Statement
permalink: /fire/auxiliary

classes: wide
sidebar:
 nav: "fire"
---
<link rel="stylesheet" href="../styles.css">

## Auxiliary Mission Statement
Supporting and Fund Raising for our Community
The Lake Cavanaugh Fire Department Auxiliaries supports the Fire Department by raising funds for equipment and supplies.

## Our Mission
The purpose of the Lake Cavanaugh Fire Department Auxiliary is to support the Fire Department by raising funds for equipment and
supplies not necessarily covered by the Fire Department budget. The auxiliary is instrumental in planning the Annual Open House & Lake Wear Sale, every Memorial Day weekend,and the annual “Once Around Lake Cavanaugh” fun run/walk.

{{ "now" | date: "%Y" }} Auxiliary Meetings are at 10 AM at the fire hall. The LCFDA cordially invites anyone to attend and appreciates new members.

<div class="grid-container">
  <div class="grid-item">
    <table id="auxiliary">
      <thead>
        <tr>
          <th>LCDF Auxiliary Meetings</th>
        </tr>
      </thead>
      <tbody>
        {% for meeting in site.data.lcfd.auxiliary_meetings %}
          <tr>
            <td>{{ meeting.month }} {{ meeting.date }}</td>
          </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
</div>

## {{ "now" | date: "%Y" }} Auxiliary Officers
<div class="grid-container">
  <div class="grid-item">
    <table id="auxiliary">
      <thead>
        <tr>
          <th>Position:</th>
          <th>Officer:</th>
        </tr>
      </thead>
      <tbody>
        {% for officer in site.data.lcfd.auxiliary %}
          <tr>
            <td><b>{{ officer.position }}</b></td>
            <td>{{ officer.name }}</td>
          </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <div class="image">
    <img src="/_lfs/images/auxiliary-01.jpg" alt="LCFDA Meeting" style="height:80%;width:auto">
  </div>
</div>

## Volunteer
Consider volunteering for the Lake Cavanaugh Fire Department Auxiliary. It’s rewarding and doesn’t take as much time as you think. Click here to see a list of our current volunteers.

## Fill the Boot Fundraiser

<div class="image">
  <img align="right" src="/_lfs/images/auxiliary-03.jpg" width="50%" height="auto">
</div>
2020 brought the Covid 19 Pandemic, which changed the Lake Cavanaugh Fire Department Auxiliary’s ability to provide their annual Pancake Breakfast. In years past, this was a major fundraiser. Unable to do this breakfast, more creative ideas were needed to keep our Fire Department funded. Hence, the “Fill the Boot” fundraiser was set into motion. It turned out to be a huge success. Our community came out in force, showing support, respect and gratitude for the men and women who volunteer their time for the good and protection of our residents. It was fun, exciting and as previously stated, very successful. It has now become an annual Labor Day event that everyone looks forward to.
