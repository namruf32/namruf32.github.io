---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
title: Lake Cavanaugh Fire Department Volunteers
permalink: /fire/members

classes: wide
sidebar:
  nav: "fire"
---
<style>
.grid-container {
  display: grid;
  grid-template-columns: 30% 30% 40%;
  padding: 10px;
}

.space {
  padding-top: 50%;
}
</style>

## {{ "now" | date: "%Y" }} Trained Emergency Responders

<div class="grid-container">
  <div class="grid-item">
    <table>
      {% for volunteer in site.data.lcfd.volunteers_left %}
        <tr>
          <td>
            <b>{{ volunteer.name}}</b><br>
            {{ volunteer.role }}
          </td>
        </tr>
      {% endfor %}
    </table>
  </div>
  <div class="grid-item">
    <table>
      {% for volunteer in site.data.lcfd.volunteers_right %}
        <tr>
          <td>
            <b>{{ volunteer.name}}</b><br>
            {{ volunteer.role }}
          </td>
        </tr>
      {% endfor %}
    </table>
  </div>
  <div class="grid-item, space">
    <img src="/_lfs/images/lcfd_thanks.jpg" alt="Thanks LCFD" style="width:100%">
  </div>
</div>