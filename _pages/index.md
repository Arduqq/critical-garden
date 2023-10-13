---
layout: page
title: Home
id: home
permalink: /
---

# This [is/is not] Hyperreality. Status: **CRITICAL**

  These are the mind demons one (or just Artur) fights when trying to understand Critical Theory. This is a Digital ~~Dungeon~~ Garden [as presented by Caulfield](https://hapgood.us/2015/10/17/the-garden-and-the-stream-a-technopastoral/) to let my thoughts claim virtual space.

<strong>(P)lots of Thoughts</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
