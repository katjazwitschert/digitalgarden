---
layout: page
title: Home
id: home
permalink: /
---

# Hallo! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Ich bin Katja Evertz. Ich bin Digitalstrategin und Beraterin für digitale Kommunikation. Dieser digitale Garten ist ein Experiment, ein Archiv und eine Karte meiner Interessen, Notizen und Ideen. [Mehr über mich](https://www.katjaevertz.de/ueber-katja-evertz/) gibt es [auf meiner persönlichen Website}(https://www.katjaevertz.de/).
</p>

Dies ist mein digitaler Garten, in dem ich meine Ideen festhalte und daraus Gedanken und längere Texte wachsen lasse.

Dieser digitale Garten ist ein Work in Progress. Anders als im Blog steht jeder Inhalt hier für sich, nicht chronologisch, sondern vernetzt mit anderen Gedanken und Ideen. 

Ich möchte hier außerdem wichtige Links sammeln und eine persönliche Anlaufstelle für die Inhalte haben, die für mich wichtig sind.

## Einstiegspunkte

[[Das Prinzip der Faltung]]
[[Warum wir Grenzen brauchen]]
[[Zettelkasten]]
[[Digital Gardens]]

## Neueste Notizen

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
