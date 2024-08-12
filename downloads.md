---
layout: page
title: Downloads
subtitle: Alle wichtigen Dokumente zum herunterladen
---


# Jahresprogramm
Eine Übersicht aller Termine. Weitere Einzelheiten zu den anstehenden Anlässen findet ihr im aktuellen Quartalsprogramm (QP).
## [Download](/assets/downloads/Pfadi_Jahresprogramm.pdf)

# Quartalsprogramm (QP)
Für jedes Jahresquartal erscheint ein sogenanntes QP, welches detailierte Infos zu den Anlässen im aktuellen Quartal enthält.
Auch Anmeldeformulare für spezielle Events und Lager werden dem QP beigelegt.
## [Download](/assets/downloads/Pfadi_QP.pdf)

# Anmeldeformular
Die Pfadi gefällt dir und do möchtest dem Verein offiziel Beitreten? Dann fülle bitte dieses Formular aus und schick es uns via Mail an [abteilung@pfadithierstein.ch](mailto:abteilung@pfadithierstein.ch), oder bring es ausgedruckt an einem Pfadinachmittag mit.
## [Download](/assets/downloads/Pfadi_Anmeldeformular.pdf)

# Allgemeine Infos
Dieses Dokument enthält eine Sammlung von wichtigen Infos, die es für den Pfadialltag zu wissen gilt. Seid ihr neu in der Pfadi, empfehlen wir euch unbedingt dieses zu lesen.
## [Download](/assets/downloads/Pfadi_Allgemeine_Infos.pdf)

{% assign download_files = site.static_files | where: "downloads", true %}
{% for dl in download_files %}
- [{{ dl.basename }}]({{ dl.path }})
{% endfor %}
