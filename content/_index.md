---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:

  - block: resume-biography
    id: home
    content:
      username: admin
      text: ""
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: background3.png
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: 'About us'
      subtitle: ''
      text: |-
        The research mission of the HERCOLE Lab is to make next-generation ML and AI systems more **understandable** to humans, **resilient** to adversarial attacks, and **decentralized** to edge devices.
    design:
      columns: '1'

  - block: director
    id: team
    content:
      username: director
      title: Lab Director

  - block: students
    content:
      usernames:
        - student1
        - student2
        - student3
        - student4
        - student5
      title: PhD Students

  - block: collaborators
    content:
      usernames:
        - collaborator1
        - collaborator2
        - collaborator3
        - collaborator4
        - collaborator5
        - collaborator6
      title: External Collaborators

  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [50, 0, 0, 0]

  
---
