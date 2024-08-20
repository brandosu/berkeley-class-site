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
<!--
[Extensions](https://docs.google.com/forms/d/e/1FAIpQLScuJXqPqocHgYd1SLx2GryGVUhcA6_OzDtYZvbhek3La65KxA/viewform){: .btn .btn-extensions}
-->
[Office Hours Queue](https://oh.data8.org/){: .btn .btn-officehours}
[Jump to Current Week](#week-{{ site.current_week }}){: .btn .btn-currweek}

{% for module in site.modules %}
{{ module }}
{% endfor %}
