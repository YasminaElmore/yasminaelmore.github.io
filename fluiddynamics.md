---
layout: yasmina_default
title: "Fluid Dynamics Portfolio"
description: Projects showcasing fluid dynamics skills
---

{% assign sorted_projects = site.projects_fluid_dynamics | sort: "date" | reverse %}
{% assign current_year = "" %}

{% for project in sorted_projects %}
  {% unless project.path contains '/unpublished/' %}
    {% assign project_year = project.date | date: "%Y" %}
  
    {% if project_year != current_year %}
      {% if current_year != "" %}
      {% endif %}
<br>
## {{ project_year }}
      {% assign current_year = project_year %}
    {% endif %}
  
### [{{ project.title }}]({{ project.url }})
{{project.description}}

---

  {% endunless %}
{% endfor %}