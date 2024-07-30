---
layout: page
title: Leitungsteam
subtitle: Unser Leitungsteam
---



{% for member in site.data.members %}
### {{ member.name }} ({{ member.full_name }})
#### {{ member.functions | join: ', ' }}
![]({{ member.picture }})

---
{% endfor %}
