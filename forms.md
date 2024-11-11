---
forms:
  - to: abteilung@pfadithierstein.ch
    subject: Badespass
    redirect: /
    form_engine: formspree
    placeholders: false
    fields:
      - name: Vorname
        required: true
        input_type: text
      - name: Nachname
        required: true
        input_type: text
      - name: Pfadiname
        required: false
        input_type: text
      - name: Anmeldebestätigung
        required: true
        input_type: checkbox
        placeholder: Ich nehme am Anlass teil
      - name: Was ich noch mitteilen möchte
        required: false
        input_type: textarea
        required: false
      - name: Absenden
        input_type: submit
        required: true
---

{% if page.forms[0] %}
{% include form.html form="1" %}
{% endif %}
