---
title: Getting started
description: Useful infromtion for students and staff that start working in the Robotics Lab.
order: 1
---

# First steps
- Introduce yourself to both your peers as to the staff.
- Request one of the staff members:
    - access to this repository
    - subscription to the robotics-lab Googlegroups mailing list
- Pick a free desk and indicate your choice, as described in [People & Desks](#people--desks).
- Make yourself familiar with the keys to the lab and testlab, the coffee machine, etc. 
- If you have any questions, ask people and, if necessary, update this website with the new/updated information. Go to the [site_maintenance](site maintenance) section for more information on how to update the contents of this site.

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



