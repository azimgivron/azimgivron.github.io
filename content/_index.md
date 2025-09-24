---
# Leave the homepage title empty to use the site title
title: ''
date: 2025-09-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My PhD'
      subtitle: ''
      text: |-
        Matrix completion using deep neural networks via advanced optimization techniques This research aims to develop a matrix completion framework incorporating both Euclidean and non-Euclidean methodologies to effectively capture complex data structures. 
        
        Nonsmooth regularization techniques, such as the $\ell_1$-norm and nuclear norm, are integrated to promote sparsity and low-rank structure in the reconstructed matrices. To address the resulting optimization challenges, advanced smoothing strategies—specifically proximal gradient methods and forward-backward splitting—are employed.
        
        By combining deep modeling with robust mathematical optimization, the proposed approach is designed to enhance imputation accuracy, particularly in the presence of irregular and high-dimensional data. The method will be validated on real-world datasets from recommendation systems and biomedical domains, such as rare diseases and gene prioritization, demonstrating improved performance over traditional techniques.
    design:
      columns: '1'
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: blog
    content:
      title: Latest Blog Posts
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
