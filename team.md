---
layout: page
title: Leitungsteam
subtitle: Unser Leitungsteam
---

{% assign ALs = site.data.members | where: "group", "Abteilungsleiter" %}
{% assign wolf = site.data.members | where: "group", "Wolfsstufe" %}
{% assign pfadi = site.data.members | where: "group", "Pfadistufe" %}
{% assign weitere = site.data.members | where: "group", "Weitere" %}

# Abteilungsleitung
{% for member in ALs %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
![](/assets/pictures/team/{{ member.name | downcase }}.jpg)

---
{% endfor %}

# Wolfsstufe
{% for member in wolf %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
![](/assets/pictures/team/{{ member.name | downcase }}.jpg)

---
{% endfor %}

# Pfadistufe
{% for member in pfadi %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
![](/assets/pictures/team/{{ member.name | downcase }}.jpg)

---
{% endfor %}

# Ämter
{% for member in weitere %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
![](/assets/pictures/team/{{ member.name | downcase }}.jpg)

---
{% endfor %}
