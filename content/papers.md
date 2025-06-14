---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "10rem"

sections:

  - block: library
    content:
      title: Publications
      text: ""
      count: 65535
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  
---
