---
---

This is a list of the research projects. Note that some projects may have a private repository
<hr>
<ul >
    {% for member in site.data.research_projects %}
    <h2>{{member.project_name}}</h2>
        <strong>Description</strong>: <i>{{member.description}}</i> <br>
        <strong>Members</strong>: {{member.members}} <br>
        <strong>Students</strong>: {{member.students}} <br>
        <strong>Repository</strong>: <a href="{{member.repository}}">{{member.repository}}</a> <br>
        <strong>Wiki</strong>: <a href="{{member.wiki}}">{{member.wiki}}</a>
    <hr>
    {% endfor %}
</ul>


Modifications to this content can be done in [this](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_data/research_projects.yml) `yaml` file.