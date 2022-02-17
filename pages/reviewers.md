---

title: CfT/CfP Reviewers
layout: event_noheader
permalink: /reviewers/

---

# {{page.title}}
<br>
<div class="keynote-full">
{% for reviewer in site.data.reviewers %}
<hr>
		<div>
		    <a name="{{reviewer.name}}"><img style="background-image: url({{speaker.image | default: 'owasp_logo.png'}});"></a>
		</div>
		<div class='keynote-info'>
			<a href='{{reviewer.url}}'><strong>{{reviewer.name}}</strong></a>
			<br>
			{{reviewer.bio}}
			<br>
            {% if reviewer.social.size > 0 %}
            <br>
            <strong>Social Links:</strong>
            <ul>
            {% for social in reviewer.social %}
                <li><a href='{{social.url}}'><strong>{{social.name}}</strong></a></li>
            {% endfor %}
            </ul>
            {% endif %}
		</div>
{% endfor %}
</div>