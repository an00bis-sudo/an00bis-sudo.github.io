---
layout: page
title: Downloads
subtitle: Alle wichtigen Dokumente zum herunterladen
---

{% assign download_files = site.static_files | where: "downloads", true %}
{% for dl in download_files %}
- [{{ dl.basename }}]({{ dl.path }})
{% endfor %}
