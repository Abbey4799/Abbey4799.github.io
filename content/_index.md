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
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience dates.
      # Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Intern
          company: ByteDance Seed
          company_url: 'https://seed.bytedance.com/en/direction/llm'
          company_logo: bytedance
          location: Shanghai, China
          date_start: '2024-11-01'
          date_end: ''
          description: |2-
              Topics: Reasoning Model, Long Chain-of-thought. 
              
              Projects: Seed-Thinking-v1.5, Doubao-1.5-pro-AS1-Preview.
        - title: Research Intern
          company: StepFun 
          company_url: 'https://www.stepfun.com/company'
          company_logo: stepfun
          location: Shanghai, China
          date_start: '2024-10-01'
          date_end: '2025-05-15'
          description: |2-
              Topics: LLMs Reasoning, Generative Reward Model
        - title: Student Research Leader
          company: Knowledge Works Lab, at Fudan University
          company_url: ''
          company_logo: fudan
          location: Shanghai, China
          date_start: '2021-03-01'
          date_end: ''
          description: |2-
              Topics: Instruction Following, LLMs Reasoning, Creative Generation
    design:
      columns: '2'
  - block: markdown
    id: news
    content:
      title: News
      text: |
        + ***May.*** **2025** 🎉 Checkout [KORGym](https://arxiv.org/abs/2505.14552), A Dynamic Game Platform for LLM Reasoning Evaluation. 

        + ***May.*** **2025** 🎉 Two papers about how to enhance instruction following have been accepted by ACL 2025 findings! The first paper enhances the [soft contraint following ability of LLMs](https://arxiv.org/abs/2501.04945) and the second paper investigated the [position bias in multi-constraint instruction following](https://arxiv.org/pdf/2502.17204).

        + ***Apr.*** **2025** 🎉 We introduce [Seed1.5-Thinking](https://arxiv.org/abs/2504.13914), capable of reasoning through thinking before responding, resulting in improved performance on a wide range of benchmarks.

        + ***Mar.*** **2025** 🎉 Our Instruction Following Benchmark [CELLO](https://arxiv.org/abs/2309.09150) was used by [Hunyuan-Thinker-1-Preview](https://llm.hunyuan.tencent.com/#/blog/hy-t1) for instruction following evaluation.

        + ***Jan.*** **2025** 🎉 Congratulations on our paper [Think Thrice Before You Act: Progressive Thought Refinement in Large Language Models](https://arxiv.org/abs/2410.13413) accepted by ICLR 2025!

        + ***Nov.*** **2024** 👀 Joined [ByteDance Seed-LLM-Horizon](https://seed.bytedance.com/en/direction/llm) as a research intern to work on reasoning models.

        + ***Aug.*** **2024** 🎉 How to improve LLMs' ability to follow *Complex Instructions*? Congratulations on our paper [From Complex to Simple: Enhancing Multi-Constraint Complex Instruction Following Ability of Large Language Models](https://abbey4799.github.io/publication/constraint/) got accepted to EMNLP 2024 findings!

        + ***May.*** **2024** 👀 Joined [StepFun](https://www.stepfun.com/company) Foundation Model Group as a research intern to work on LLM reasoning research.

        + ***May.*** **2024** 🔔 Gave a talk at [Alibaba Tongyi Lab](https://tongyi.aliyun.com/), titled: "Complex Instruction Following Ability of Large Language Models". Thanks for the invitation!
    
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
          date_start: '2025-03-01'
          description: ''
          organization: First-Class Academic Scholarship for Doctoral Students
          organization_url: ''
          title: Intel Fellowship
          url: ''
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
          title: Venustech Scholarship
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
