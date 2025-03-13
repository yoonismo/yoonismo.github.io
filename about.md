---
layout: about
#image: /assets/img/blog/hydejack-9.jpg   # {{ site.data.resume.basics.name }}
description: >
  A boutique Jekyll theme for hackers, nerds, and academics,
  with a focus on personal sites that are meant to impress.
hide_description: true
redirect_from:
  - /download/
---  

# About

<!--author-->


**{{ site.data.resume.basics.label }}**  
Email: [{{ site.data.resume.basics.email }}](mailto:{{ site.data.resume.basics.email }})  
Website: [{{ site.data.resume.basics.website }}]({{ site.data.resume.basics.website }})
[📄 **Download CV as PDF**](https://drive.google.com/file/d/1D0LfRVO3V96jPtwCT_cXDaK7nVUnwEzP/view?usp=sharing)  
{:.no-hover.no-mark}

---

## Summary
{{ site.data.resume.basics.summary }}

---

## Skills
{% for skill in site.data.resume.skills %}
- **{{ skill.name }}:** {{ skill.keywords | join: ', ' }}
{% endfor %}

---

## Education
{% for edu in site.data.resume.education %}
**{{ edu.studyType }} in {{ edu.area }}** - {{ edu.institution }}  
**{{ edu.startDate }} - {{ edu.endDate }}**

{% endfor %}
