---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: skills
  #   content:
  #     title: Skills
  #     text: ''
  #     # Choose a user to display skills from (a folder name within `content/authors/`)
  #     username: admin
  #   design:
  #     columns: '1'
  - block: markdown
    id: news
    content:
      title: News
      text:
        + ***Dec.*** **2023** Gave a talk at [Tencent AI Lab](https://ai.tencent.com/ailab/en/index/), titled: “Beyond Simple Words: Make Machine Communicate like Humans”. Thanks for the invitation!
    
        + ***Dec.*** **2023** Congratulations on our paper [Enhancing Quantitative Reasoning Skills of Large Language Models through Dimension Perception.](https://abbey4799.github.io/publication/quantitative_reasoning/) being accepted to ICDE 2024! 

        + ***Dec.*** **2023** Three papers have been accepted by AAAI 2024! The first paper is [CELLO](https://abbey4799.github.io/publication/cello/), a benchmark for evaluating LLMs'' ability to follow complex instructions systematically. The second paper is [Xiezhi](https://github.com/MikeGu721/XiezhiBenchmark), a comprehensive, multi-disciplinary, auto-updating benchmark for domain knowledge evaluation.  

        + ***April.*** **2023** We released [CuteGPT](https://github.com/Abbey4799/CuteGPT), an open-source conversational language model developed by the Knowledge Works Research Laboratory at Fudan University, Integrated by [FastChat](https://github.com/lm-sys/FastChat).
    
        + ***Mar.*** **2023** Our paper [HAUSER](https://abbey4799.github.io/publication/hauser/) got accepted to ACL 2023!
    
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2023-10-15'
          description: ''
          organization: Intel
          organization_url: ''
          title: Intel Fellowship
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2022-12-15'
          description: ''
          organization: Fudan University
          organization_url: ''
          title: Outstanding Academic Scholarship for Master Students
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2021-06-01'
          description: ''
          organization: Fudan University
          organization_url: ''
          title: Outstanding Graduates in Shanghai
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2020-10-01'
          description: ''
          organization: Fudan University
          organization_url: ''
          title: China National Scholarship
          url: ''
    design:
      columns: '2'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      columns: '2'
      view: citation
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
#      buttons:
#        - name: All
#          tag: '*'
#        - name: Deep Learning
#          tag: Deep Learning
#        - name: Other
#          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
---
