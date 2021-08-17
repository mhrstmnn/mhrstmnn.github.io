---
title: "Michael Horstmann<br><a href='https://github.hrstmnn.de'> @mhrstmnn</a>"
description: "<a href='https://horstmann-development.de' target='blank' id='link-hd'>→ Horstmann Development 👨🏻‍💻</a>"
---

## Posts

<ul>
  {% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>

## Links

<table id="links-table">
  <tr>
    <td><ul><li><a href="https://github.com/mhrstmnn" target="blank">GitHub</a></li></ul></td>
    <td><ul><li><a href="https://open.spotify.com/user/m.horstmann" target="blank">Spotify</a></li></ul></td>
  </tr>
  <tr>
    <td><ul><li><a href="https://twitter.com/mhrstmnn" target="blank">Twitter</a></li></ul></td>
    <td><ul><li><a href="https://www.reddit.com/u/mhrstmnn" target="blank">Reddit</a></li></ul></td>
  </tr>
  <tr>
    <td><ul><li><a href="https://www.instagram.com/mhrstmnn" target="blank">Instagram</a></li></ul></td>
    <td><ul><li><a href="https://tumblr.hrstmnn.de" target="blank">Tumblr</a></li></ul></td>
  </tr>
  <tr>
    <td><ul><li><a href="https://unsplash.com/@mhrstmnn" target="blank">Unsplash</a></li></ul></td>
    <td><ul><li><a href="https://threema.id/ZA5C68WH" target="blank">Threema</a></li></ul></td>
  </tr>
  <tr>
    <td><ul><li><a href="https://t.me/mhrstmnn" target="blank">Telegram</a></li></ul></td>
    <td><ul><li><a href="mailto:m@hrstmnn.de" target="blank">Mail</a></li></ul></td>
  </tr>
</table>
<br>

**OpenPGP-Keys**
  - <a href="https://keys.openpgp.org/search?q=mhorstmann%40posteo.de" target="blank">Posteo</a>
  - <a href="https://keys.openpgp.org/search?q=m%40hrstmnn.de" target="blank">m@hrstmnn</a>
  - <a href="https://keys.openpgp.org/search?q=michael%40horstmann-development.de" target="blank">Horstmann Development</a>

<script>
  if (!(navigator.userAgent.indexOf("Mobi") > -1)) {
    // desktop
    const content = document.querySelector("#content");
    content.style.display = "inline-block";
    const container = document.createElement("div");
    container.style.display = "flex";
    container.style.justifyContent = "center";
    container.style.alignItems = "center";
    container.appendChild(content);
    document.body.appendChild(container);
  }
</script>
