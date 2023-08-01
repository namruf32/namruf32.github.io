---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
title: Officers & Committees
permalink: /lcia/governing

classes: wide
sidebar:
  nav: "lcia"
---
<style>
#governance {
  border-collapse: collapse;
  display:table;
  width: 90%;
}

#governance td, #governance th {
  border: 0px solid #ddd;
  padding: 8px;
}

#governance tr:hover {background-color: #ddd;}

#governance th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #D8EBF1;
  color: black;
}

.image {
  margin-top: 10%;
}

.grid-container {
  display: grid;
  grid-template-columns: 50% 50%;
  padding: 10px;
}
</style>

## {{ "now" | date: "%Y" }} LCIA Officers

<div class="grid-container">
  <div class="grid-item">
    <table id="governance">
      <thead>
        <tr>
          <th>Position:</th>
          <th>Officer:</th>
          <th>Contact:</th>
        </tr>
      </thead>
      <tbody>
        {% for officer in site.data.officers %}
        <tr>
          <td><b>{{ officer.position }}</b></td>
          <td><a href = "mailto: {{ officer.email }}">{{ officer.name }}</a></td>
          <td>{{ officer.phone }}</td>
        </tr>
        {% endfor %}
        {% for director in site.data.directors %}
        <tr>
          {% if forloop.index == 1 %}
            <td style="vertical-align:top" rowspan={{ forloop.length }}><b>Directors</b></td>
          {% endif %}
            <td><a href = "mailto: {{ director.email }}">{{ director.name }}</a></td>
            <td>{{ director.phone }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <div class="image">
    <img src="/_lfs/images/community_center.jpg" alt="Community Center" style="width:100%">
  </div>
</div>

## Committees

<div class="grid-container">
  <div class="grid-item">
    {% for committee_hash in site.data.committees.left %}
      {% assign committee = committee_hash[1] %}
        <table id="governance">
          <thead>
            <tr>
              <th><b>{{ committee.name }}</b></th>
            </tr>
            </thead>
              <tbody>
                {% for volunteer in committee.volunteers %}
                  <tr>
                    <td>
                      <a href="mailto: {{ volunteer.email }}">{{ volunteer.name }}</a> {{ volunteer.phone}}
                    </td>
                  </tr>
                {% endfor %}
              </tbody>
        </table>
    {% endfor %}
  </div>
  <div class="grid-item">
    {% for committee_hash in site.data.committees.right %}
      {% assign committee = committee_hash[1] %}
        <table id="governance">
          <thead>
            <tr>
              <th><b>{{ committee.name }}</b></th>
            </tr>
            </thead>
              <tbody>
                {% for volunteer in committee.volunteers %}
                  <tr>
                    <td>
                      <a href="mailto: {{ volunteer.email }}">{{ volunteer.name }}</a> {{ volunteer.phone}}
                    </td>
                  </tr>
                {% endfor %}
              </tbody>
        </table>
    {% endfor %}
  </div>
</div>