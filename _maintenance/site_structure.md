---
title: Site Structure
description: This post describes the structure of the robotics.tue.nl website
---
# Introduction

This section describes how this website is structured and gives guidelines to maintain it.

This website has been created with [Github pages](https://pages.github.com)and is hosted on [github.com](http://www.github.com). It uses [Jekyll's platform](https://jekyllrb.com/) to transform text files into HTML websites. This allows the users to focus on the content, rather than on the site's source code. Pages are written in the very simple Markdown language (but can also be HTML files).

# Site Structure

The website contains the following sections: [About](/about), [Repositories](/repositories), [Tutorials](/tutorials), [Publications](/publications), [Robotics Lab](/robotics_lab) and <a href="">Site Maintenance</a>. These sections are added to the navigation bar by their inclusion in the [data/navigation.yml](https://github.com/robotics-tue/robotics-tue.github.io/blob/master/_data/navigation.yml) file. Each section is described by a list entry composed of a <texttt>title</texttt> and an <texttt>url</texttt>. To add or remove a section from the navigation bar, add or remove the corresponding entry of the file. _Note that this doesn't automatically add or remove a page, it only adds or removes the entry in the navigation bar._

## Index Files

The main page of the website is <texttt>index.html</texttt>. When navigating to this website, this is the first page you see.

Each section also has an index file with followin naming convention <texttt>index_<section_name>.html</texttt>, e.g. <texttt>index_maintenance.html</texttt> for this section. Both the main index as the section index HTML files are located in the root directory of the repository (i.e. <texttt>/</texttt>).

The reason for having an index file per section is to be able to loop over the different pages of each section with the aid of the [liquid template language](https://shopify.github.io/liquid/). In the case of the [Tutorials](/tutorials) section, for example, there is an index file (<texttt>index_tutorials.html</texttt>) that serves as compilation site for each of the different tutorials. The subpages of these tutorials are located in the <texttt>_tutorials/</texttt> directory. The <texttt>index_tutorials.html</texttt> site loops over the titles of each of the tutorials to display them. More about these for loops below.

## Content

As mentioned above, each section contains an index page that refers to its different subpages. These subpages are located in a directory that has the following naming convention: <texttt>_<section-name></texttt>, e.g. <texttt>_tutorials</texttt>. These subpages are written in Markdown format (see [Markdown Quick Guide](/tutorials/markdown-quick-guide)). It is in these pages where content can be added.

Although these files are written in HTML, they contain _Front Matter_, i.e. a preamble with key-value pairs that defines
