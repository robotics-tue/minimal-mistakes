---
---

This is a list of the student teams.
<hr>
<ul >
    {% for member in site.data.student_teams %}
    <h2>{{member.team_name}}</h2>
        <strong>Description</strong>: <i>{{member.description}}</i> <br>
        <strong>Website</strong>: {{member.website}} <br>
        <strong>Repository</strong>: <a href="{{member.repository}}">{{member.repository}}</a> <br>
        <strong>Wiki</strong>: <a href="{{member.wiki}}">{{member.wiki}}</a>
        <strong>Members</strong>: {{member.members}} <br>
    <hr>
    {% endfor %}
</ul>

Modifications to this content can be done in [this](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_data/student_teams.yml) `yaml` file.
