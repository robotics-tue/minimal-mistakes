---
title: Site Structure
layout: page_with_toc
description: This post describes the structure of the robotics.tue.nl website
---

# Introduction

This section describes how this website is structured and gives guidelines to maintain it.

This website has been created with [Github pages](https://pages.github.com)and is hosted on [github.com](http://www.github.com). It uses [Jekyll's platform](https://jekyllrb.com/) to transform text files into HTML websites. This allows the users to focus on the content, rather than on the site's source code. Pages are written in the very simple Markdown language (but can also be HTML files).

# Site Structure

The website contains the following sections: [About](/about), [Repositories](/repositories), [Tutorials](/tutorials), [Publications](/publications), [Robotics Lab](/robotics_lab) and <a href="">Site Maintenance</a>. These sections are added to the navigation bar by their inclusion in the [data/navigation.yml](https://github.com/robotics-tue/robotics-tue.github.io/blob/master/_data/navigation.yml) file. Each section is described by a list entry composed of a `title` and an `url`. To add or remove a section from the navigation bar, add or remove the corresponding entry of the file. _Note that this doesn't automatically add or remove a page, it only adds or removes the entry in the navigation bar._

The most important files and directories are displayed below in a directory tree diagram. Each file / directory is followed by a short description.

```
- robotics-tue.github.io
  |--   _data                     # contains yml files with data
         |--  navigation.yml            # list of titles & urls for the nav bar      
         |--  robotics_lab_members.yml  # list of members of the robotics lab
  |--   _pages                    # contains md files with content
  |--   _posts                    # contains md files with posts
  |--   _maintenance              # contains md files for the maintenance section
  |--   _tutorials                # contains md files for the tutorials section
  |--   images                    # 
  |--   _config.yml               # configuration file for the website
  |--   index.html                # main index file
  |--   index_maintenance.html    # maintenance index file
  |--   index_publications.html   # publications index file
  |--   index_repositories.html   # repositories index file
  |--   index_tutorials.html      # tutorials index file
```


## Index Files

The main page of the website is `index.html`. When navigating to this website, this is the first page you see.

Each section also has an index file with followin naming convention `index_<section_name>.html`, e.g. `index_maintenance.html` for this section. Both the main index as the section index HTML files are located in the root directory of the repository (i.e. `/`).

The reason for having an index file per section is to be able to loop over the different pages of each section with the aid of the [liquid template language](https://shopify.github.io/liquid/). In the case of the [Tutorials](/tutorials) section, for example, there is an index file (`index_tutorials.html`) that serves as compilation site for each of the different tutorials. The subpages of these tutorials are located in the `_tutorials/` directory. The `index_tutorials.html` site loops over the titles of each of the tutorials to display them. More about these for loops below.

## Content

As mentioned above, each section contains an index page that refers to its different subpages. These subpages are located in a directory that has the following naming convention: `_<section-name>`, e.g. `_tutorials`. These subpages are written in Markdown format (see [Markdown Quick Guide](/tutorials/markdown-quick-guide)). It is in these pages where content can be added.

Although these files are written in HTML, they contain _Front Matter_, i.e. a preamble with key-value pairs that defines
