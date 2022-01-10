---

title: Event Registration
layout: event_noheader
permalink: /register/

---

## Registration 
{% if site.data.event-details.registration_open %}
### Registration is open via (this link)[{{site.event-details.registration_url}}]

{% else %}
<br>
### Registration is not yet open. Please return later.
<br>
{% endif %}

{% if site.data.event-details.registration_open %}
{% comment %}
{% include registration_form.md show_dietary_restrictions="false" primary_color="#0079a7" %}
{% endcomment %}

{% endif %}


Questions? [events@owasp.com](mailto:events@owasp.com?subject=Event%20Example%20Inquiry)
