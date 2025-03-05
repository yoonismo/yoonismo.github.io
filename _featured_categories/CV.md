---
layout: page
title: CV
slug: CV 
#permalink: /cv/
---

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
