---
title: Icons
maturity: draft
control: exclude
items: 
  - name: Small
    path: src/assets/images/icon-64x64.png
  - name: Small1
    path: src/assets/images/icon-64x64.png
  - name: Small2
    path: src/assets/images/icon-64x64.png
  - name: Small3
    path: src/assets/images/icon-64x64.png
  - name: Small4
    path: src/assets/images/icon-64x64.png
  - name: Small5
    path: src/assets/images/icon-64x64.png
  - name: Small6
    path: src/assets/images/icon-64x64.png
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