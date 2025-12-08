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
        about: 'About Me and Why I Built This Website'
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
        This thesis investigates the integration of advanced smoothing strategies—most notably proximal gradient methods and forward–backward splitting—into modern deep learning architectures and generative modeling frameworks. The central objective is to exploit these optimization techniques to improve stability, convergence behavior, and interpretability in high-dimensional learning problems.

        The methodological contribution lies in adapting classical operator-splitting schemes to neural models, enabling controlled regularization and structured sparsity while preserving expressiveness. These techniques allow complex models to incorporate domain-specific priors through proximal operators, facilitating more robust training in settings where data are noisy, incomplete, or inherently constrained.

        The practical relevance of this work spans multiple areas in computational biology and biomedical data science. In gene prioritization, the proposed methods aim to improve the ranking of candidate genes by enforcing biologically meaningful structures and smoothing noisy association signals. In drug discovery, the same framework supports more reliable generative models for molecular design by promoting physically consistent representations and reducing the instability often observed in traditional generative training regimes.
    design:
      columns: '1'
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: ''
  #     filters:
  #       folders:
  #         - publications
  #       exclude_featured: false
  #   design:
  #     view: citation
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
