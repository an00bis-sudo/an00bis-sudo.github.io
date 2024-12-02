---
layout: page
title: Leitungsteam
subtitle: Unser Leitungsteam
---

{% assign ALs = site.data.members | where: "group", "Abteilungsleiter" %}
{% assign wolf = site.data.members | where: "group", "Wolfsstufe" %}
{% assign pfadi = site.data.members | where: "group", "Pfadistufe" %}
{% assign weitere = site.data.members | where: "group", "Weitere" %}

<img src="/assets/pictures/team/leitungsteam.jpg" class=member_img />


# Abteilungsleitung
---
{% for member in ALs %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
{% if member.contact %}
#### [{{ member.contact }}](mailto:{{ member.contact }})
{% endif %}
<img src="/assets/pictures/team/{{ member.name | downcase }}.jpg" class=member_img />

---
{% endfor %}


# Wolfsstufe
---
{% for member in wolf %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
{% if member.contact %}
#### [{{ member.contact }}](mailto:{{ member.contact }})
{% endif %}
<img src="/assets/pictures/team/{{ member.name | downcase }}.jpg" class=member_img alt="{{ member.name}}"/>

---
{% endfor %}


# Pfadistufe
---
{% for member in pfadi %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
{% if member.contact %}
#### [{{ member.contact }}](mailto:{{ member.contact }})
{% endif %}
<img src="/assets/pictures/team/{{ member.name | downcase }}.jpg" class=member_img />

---
{% endfor %}


# Ämter
---
{% for member in weitere %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
{% if member.contact %}
#### [{{ member.contact }}](mailto:{{ member.contact }})
{% endif %}
<img src="/assets/pictures/team/{{ member.name | downcase }}.jpg" class=member_img />

---
{% endfor %}
