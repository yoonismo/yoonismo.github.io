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
Website: [{{ site.data.resume.basics.website }}]({{ site.data.resume.basics.website }}) <br>
Resume: [My resume](https://drive.google.com/file/d/1cgfcZZtYk_E52mZruIuSu61PIR2heC0i/view?usp=drive_link)
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
**{{ edu.studyType }} in {{ edu.area }}** - {{ edu.institution }}{% if edu.studyType contains 'Ph.D' or edu.studyType contains 'PhD' %}
{%- assign expected_raw = edu.endExpected | default: edu.endDate -%}
{%- if expected_raw -%}
 {%- comment -%}문자 그대로 'expected'가 이미 들어있으면 중복 방지{%- endcomment -%}
{%- if expected_raw contains 'expected' or expected_raw contains 'Expected' -%}
 ({{ expected_raw }})
{%- else -%}
 ({{ expected_raw }} expected)
{%- endif -%}
{%- endif -%}
{% endif %}

{% endfor %}


