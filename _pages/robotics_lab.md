---
title: Robotics Lab
permalink: /robotics_lab/
layout: tutorials_layout
---
# Getting started in the robotics lab
- Announce your presence to both your peers as to the staff.
- Request access to this repository to one of the staff members.
- Pick a free desk and indicate your choice as described in [People & Desks](#people--desks)
- Get yourself subscribed on the robotics-lab Googlegroups mailinglist (ask Wouter Houtman about this)
- Make yourself familiar with the keys to the lab and testlab, the coffee machine, etc. If you have any questions, ask people and put the additional info on this Wiki!
- Ask Thea for acces to the lab.

# People & Desks

The following table indicates which desks are assigned to whom. A map of the distribution of the desks can be found below.

In order to assign a (free) desk to yourself, modify the following file: [robotics_lab_members.yml](https://github.com/robotics-tue/robotics-tue.github.io/blob/master/_data/robotics_lab_members.yml).

<table style="table">
    <tr>
        <th>Desk</th>
        <th>Name</th>
        <th>E-mail address</th>
        <th>Function</th>
        <th>Project</th>
    </tr>
    {% for member in site.data.robotics_lab_members %}
    <tr>
        <td>{{member.desk}}</td>
        <td>{{member.name}}</td>
        <td>{{member.email}}</td>
        <td>{{member.function}}</td>
        <td>{{member.project}}</td>
    </tr>
    {% endfor %}
</table>

{% include image name="desk_distribution_map.png" caption="caption" %}




# Robotics Lab Printer
Students and Employees who work in the Robotics Lab can make use of the Robotics Lab printer. Intallation instructions can be found [here](/tutorials/printer).

