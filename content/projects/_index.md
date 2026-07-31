---
title: 'Projects'
date: 
type: landing

# Page is retired: not rendered, not listed, and not reachable by URL.
# Content is kept here so it can be restored by deleting this block (and
# re-adding the nav entry in `config/_default/menus.yaml`).
_build:
  render: never
  list: never
  publishResources: false
cascade:
  _build:
    render: never
    list: never
    publishResources: false

design:
  # Section spacing
  spacing: '3rem'

# Page sections
sections:
  - block: collection
    content:
      title: Projects
      text: This section outlines our **current research focus**. For each topic, you can explore a **brief overview**, review our **related works**,   and discover available **thesis projects**.
      filters:
        folders:
          - projects
    design:
      view: article-grid
      fill_image: true
      columns: 2
      show_date: false
      show_read_time: false
      show_read_more: false
---