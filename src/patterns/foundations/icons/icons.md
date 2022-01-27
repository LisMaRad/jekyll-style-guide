---
title: Favicons
maturity: draft
control: exclude
items: 
  - name: Favicon 16x16
    path: src/assets/favicon_package/favicon-16x16.png
  - name: Favicon 32x32
    path: src/assets/favicon_package/favicon-32x32.png
  - name: Android Chrome Favicon 192x192
    path: src/assets/favicon_package/android-chrome-192x192.png
  - name: Android Chrome Favicon 512x512
    path: src/assets/favicon_package/android-chrome-512x512.png
  - name: Monochrome Style 150x150
    path: src/assets/favicon_package/mstile-150x150.png

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