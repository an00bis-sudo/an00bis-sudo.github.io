---
layout: page
title: Downloads
subtitle: Alle wichtigen Dokumente zum herunterladen
---

# Jahresprogramm
Eine Übersicht aller Termine. Weitere Einzelheiten zu den anstehenden Anlässen findet ihr im aktuellen Quartalsprogramm (QP).
### [Download](/assets/downloads/Pfadi_Jahresprogramm.pdf)

# Quartalsprogramm (QP)
Für jedes Jahresquartal erscheint ein sogenanntes QP, welches weitere Infos zu allen Anlässen im aktuellen Quartal enthält.
Auch Anmeldeformulare für spezielle Events und Lager werden dem QP beigelegt.
### [Download](/assets/downloads/Pfadi_QP.pdf)

# Anmeldeformular
Die Pfadi gefällt dir und do möchtest dem Verein offiziel Beitreten? Dann fülle bitte dieses Formular aus und schick es uns via Mail an [abteilung@pfadithierstein.ch](mailto:abteilung@pfadithierstein.ch), oder bring es ausgedruckt an einem Pfadinachmittag mit.
### [Download](/assets/downloads/Pfadi_Anmeldeformular.pdf)

# Allgemeine Infos
Dieses Dokument enthält eine Sammlung der wichtigsten Infos für den Pfadialltag. Seid ihr neu in der Pfadi, empfehlen wir euch unbedingt dieses zu lesen.
### [Download](/assets/downloads/Pfadi_Allgemeine_Infos.pdf)

# Kulturlegi Fact-Sheet
Merkblatt zur Kulturlegi. Kinder und Jugendliche, welche im Besitz einer Kulturlegi sind, erhalten bei Pfadiabteilungen im ganzen Kanton Aargau 50% Rabatt auf Lagerbeiträge und Mitgliederbeiträge.
### [Download](/assets/downloads/Pfadi_Kulturlegi.pdf)

{% comment %} removed for now
---

# Alles
{% assign download_files = site.static_files | where: "downloads", true %}
{% for dl in download_files %}
- [{{ dl.basename }}]({{ dl.path }})
{% endfor %}
{% endcomment %}
