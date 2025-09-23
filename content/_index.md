---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/CV_English.pdf
    design:
      css_class: dark
      background:
        color: "#006C84"
        # Add your image background to `assets/media/`.
        # filename: stacked-peaks.svg
        # filters:
        #   brightness: 1.0
        # size: cover
        # position: center
        # parallax: false

  - block: collection
    id: publications
    content:
      title: Publications
      text: ""
      filters:
        folders:
          - publication
        publication_types: 
          - ["2"]
    design:
      view: citation


  - block: collection
    id: working-papers
    content:
      title: Working Papers
      text: ""
      filters:
        folders:
          - working
        publication_types: 
          - ["2"]
    design:
      view: citation

  - block: collection
    id: work-in-progress
    content:
      title: Work in progress
      text: ""
      filters:
        folders:
          - current
      citation:
        link: false 
    design:
      view: citation
---
