---
title: Icons
maturity: draft
control: exclude
items: 
  - name: Profile
    path: src/assets/icons/profile_black.svg
  - name: Calendar
    path: src/assets/icons/calendar_black.svg
  - name: Search
    path: src/assets/icons/search_black.svg
  - name: Back
    path: src/assets/icons/back_black.svg
  - name: Add
    path: src/assets/icons/plus_black.svg
  - name: Clock
    path: src/assets/icons/clock_black.svg
  - name: Maps
    path: src/assets/icons/maps_black.svg
  - name: Edit
    path: src/assets/icons/edit_black.svg
  - name: Close
    path: src/assets/icons/close_black.svg
  - name: Settings
    path: src/assets/icons/settings_black.svg
  - name: Delete Bin
    path: src/assets/icons/delete_bin_purple.svg
  - name: Check
    path: src/assets/icons/check_purple.svg
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