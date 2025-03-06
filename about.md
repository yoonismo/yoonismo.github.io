---
layout: about
#image: /assets/img/blog/hydejack-9.jpg
description: >
  A boutique Jekyll theme for hackers, nerds, and academics,
  with a focus on personal sites that are meant to impress.
hide_description: true
redirect_from:
  - /download/
---  

# About

<!--author-->

---

## Curriculum Vitae

# {{ site.data.resume.basics.name }}
**{{ site.data.resume.basics.label }}**  
Email: [{{ site.data.resume.basics.email }}](mailto:{{ site.data.resume.basics.email }})  
Website: [{{ site.data.resume.basics.website }}]({{ site.data.resume.basics.website }})

---

## Summary
{{ site.data.resume.basics.summary }}

---

## Skills
{% for skill in site.data.resume.skills %}
- **{{ skill.name }}:** {{ skill.keywords | join: ', ' }}
{% endfor %}

---

## Experience
{% for job in site.data.resume.experience %}
### {{ job.position }} at {{ job.company }}
**{{ job.startDate }} - {{ job.endDate }}**  
{{ job.summary }}

{% endfor %}

---

## Education
{% for edu in site.data.resume.education %}
**{{ edu.studyType }} in {{ edu.area }}** - {{ edu.institution }}  
**{{ edu.startDate }} - {{ edu.endDate }}**

{% endfor %}
