---
layout: page
title: Home
description: Listing of course modules and topics.
nav_order: 1
permalink: /
---

# Data 8: Foundations of Data Science 📊

{: .mb-2 }
UC Berkeley, Fall 2024
{: .mb-2 .fs-6 .text-grey-dk-000 }

[Ed](https://edstem.org/us/courses/59844/discussion/){: .btn .btn-ed}
[Gradescope](https://www.gradescope.com/courses/798344){: .btn .btn-gradescope}
[Lecture Recordings](https://bcourses.berkeley.edu/courses/1535365/external_tools/90481){: .btn .btn-bcourses}
[Textbook](https://inferentialthinking.com/chapters/intro.html){: .btn .btn-textbook}
[Jump to Current Week](#week-{{ site.current_week }}){: .btn .btn-currweek}

{% assign announcements = site.announcements | where: "week", site.current_week | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}

{% assign mods = site.modules | where: 'class', 'Berkeley' %}
{% assign active-mods = '' | split: '' %}

{% for mod in mods %}
  {% if mod.status == 'Active' %}
    {% assign active-mods = active-mods | push: mod %}
  {% endif %}
{% endfor %}

{% for module in active-mods %}
  {{ module }}
{% endfor %}
