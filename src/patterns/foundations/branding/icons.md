---
title: Icons
maturity: draft
control: exclude
items: 
  - name: Profile
    path: src/assets/icons/profile_black.png
  - name: Calendar
    path: src/assets/icons/calendar_black.png
  - name: Search
    path: src/assets/icons/search_black.png
  - name: Back
    path: src/assets/icons/back_black.png
  - name: Add
    path: src/assets/icons/plus_black.png
  - name: Clock
    path: src/assets/icons/clock_black.png
  - name: Maps
    path: src/assets/icons/maps_black.png
  - name: Edit
    path: src/assets/icons/edit_black.png
  - name: Close
    path: src/assets/icons/close_black.png
  - name: Settings
    path: src/assets/icons/settings_black.png
  - name: Delete Bin
    path: src/assets/icons/delete_bin_purple.png
  - name: Check
    path: src/assets/icons/check_purple.png
---
<style>
.set {
  display: flex;
  flex-wrap: wrap;
  margin: 0 -1rem;
  margin-top: 0;
  padding: 0;
  list-style: none;
}
li {
  flex: 1 0 20%;
  margin: 1rem;
}
.image {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  min-width: 280px;
  height: 300px;
  background-color: whitesmoke;
  border: 1px solid whitesmoke;
  margin-bottom: 1rem;
}
img {
  max-height: 100%;
}
p {
  margin: 0;
}
</style>

<ul class="set">
{% for item in page.items %} 
  <li>
    <div class="image"><img src="{{ site.baseurl }}/{{ item.path }}"/></div>
    <p class="header">{{ item.name }}</p>
    {% if item.path %}<p>{{ item.path }}</p>{% endif %}
  </li>
{% endfor %}
</ul>