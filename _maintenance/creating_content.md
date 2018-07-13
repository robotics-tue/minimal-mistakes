---
title: Creating or Modifying Content
description: Quick guide to creating or modifying content
---

Adding or modifying content in this website is very easy. Pages are written in Markdown format (a quick guide on Markdown syntax can be found [here](/tutorials/markdown_quick_guide)). Each file is assigned to its corresponding section by storing it in the section's directory.

| Section               | directory     |
| ---                   | ---           |
| About | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_about](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_about) |
| Repositories | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_repositories](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_repositories) |
| Publications | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_publications](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_publications) |
| Research Projects | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_research_projects](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_research_projects) |
| Courses | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_courses](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_courses) |
| Tutorials | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_tutorials](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_tutorials) |
| Robotics Lab | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_robotics_lab](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_robotics_lab) |
| Student Teams | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_student_teams](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_student_teams) |
| Site Maintenance | [https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_site_maintenance](https://github.com/robotics-tue/robotics-tue.github.io/tree/master/_site_maintenance) |

# Front Matter
Each Markdown file has to be initiated with a preamble called 'Font Matter'. This is a section that is defined in between two sets of tripple dashed (i.e. `---`). Within the front matter *key-value* pairs are stored that can be read by the HTML generator. An example is shown below:
```
---
title: My first tutorial
layout: page_with_toc
description: How to write a tutorial
order: 2
---
```
In this front matter, the title will be displayed in the page. The `layout` value `page_with_toc` indicates that a table of contents will be generated, based on the headers of the Markdown file. Within the `description` key a description can be given about the page content. The key `order` can be used to order the titles in the main page of the section. In [/robotics_lab](/robotics_lab), for example, it is nice to have `Getting started` at the beginning of the list.


# References to a site
To refer to a specific site, just write the path to the Markdown file, without the leading underscore, e.g. 
```
[reference name](/tutorials/markdown_quick_guide)
```
 to create a link to the Markdown quick guide tutorial.


