---
title: Markdown Quick Guide
---
Below you will find a quick reference guide for writing pages in Markdown. A more extense tutorial can be found at [www.markdowntutorial.com](www.markdowntutorial.com)

# Headers
```
# This is an <h1> tag
## This is an <h2> tag
####### This is an <h7> tag
```

# Emphasis
```
*This text will be italic*
_This will also be italic_
**This text will be bold**
__This will also be bold__
*You **can** combine them*
```

# Blockquotes
```
As Grace Hopper said:
> I’ve always been more interested
> in the future than in the past.
```

# Lists
## Unordered
```
* Item 1
* Item 2
 * Item 2a
 * Item 2b
```

## Ordered
```
1. Item 1
2. Item 2
3. Item 3
 * Item 3a
 * Item 3b
```

# Images
To include an image, upload it to the repository and reference to its location.
```
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)
```

# Links
```
http://github.com - automatic!

or

[GitHub](http://github.com)
```

# Code
## Inline Code
```
`write monotype characters within backticks`
```

## Code Blocks
````
```python
function test() {
 console.log("look ma’, no spaces");
}
```
````

# Equations
Equations are rendered by [Mathjax](https://www.mathjax.org/) to SVGs. Equations can be either inline or displayed. The Markdown syntax for these equation types is given in the table below.

| Equation type         | Code              | Example           |
| -------------         |:-------------:    | -----:            |
| Inline equation       | `\\(...\\)`       | `\\( M = Ax\\)`   |
| Displayed equation    | `\\[...\\]`       | `\\[ M = Ax\\]`   |
| Displayed equation    | `$$...$$`         | `$$ M = Ax$$`     |

# Tables
You can create tables by assembling a list of words and dividing them with hyphens `-` (for the first row), and then separating each column with a pipe `|` :

```
First Header | Second Header
------------ | -------------
Content cell 1 | Content cell 2
Content column 1 | Content column 2
First Header Second Header
Content cell 1 Content cell 2
Content column 1 Content column 2
```

# Tasks List
```
- [x] this is a complete item
- [ ] this is an incomplete item
- [x] @mentions, #refs, [links](),
**formatting**, and <del>tags</del>
supported
- [x] list syntax required (any
unordered or ordered list
supported)
```

# Issue Reference
```
#1
github-flavored-markdown#1
defunkt/github-flavored-markdown#1
```

# Backslash Escapes
Markdown allows you to use backslash `\` escapes to generate literal characters which would otherwise have special meaning in Markdown's formatting syntax, e.g. to show the asterisk character, you would type `\*`.

Markdown provides backslash escapes for
the following characters:
```
\ backslash
` backtick
* asterisk
_ underscore
{} curly braces
[] square brackets
() parentheses
# hash mark
+ plus sign
- minus sign (hyphen)
. dot
! exclamation mark
```

# Emojis :+1:
```
:+1:
:sparkles:
:camel:
:tada:
:rocket:
```
