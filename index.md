---
layout: page
title: Home / Lectures
nav_order: 1
description: Listing of course modules and topics.
currWeekNumber: 1
---

{: .mb-2 }
Ferdowsi University of Mashhad, TBA
{: .mb-0 .fs-6 .text-grey-dk-000 }


<div>
{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
  <div class="role">
    {% for staffer in instructors %}
    {{ staffer }}
    {% endfor %}
  </div>
</div>

{: .highlight }
> Welcome to the Course!


<a name="lectures"></a>
## Lectures

{% for module in site.modules %}
{{ module }}
{% endfor %}

