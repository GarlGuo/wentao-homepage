---
# Leave the homepage title empty to use the site title
title:
date: 2025-1-21
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  
  - block: collection
    id: papers
    content:
      title: Recent Papers
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering papers](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
    design:
      columns: '2'
      view: citation

  - block: experience
    id: experience
    content:
      title: Research Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Assistant
          company: Prof. Beidi Chen, Carnegie Mellon University
          company_url: ''
          company_logo: cmu
          location: Remote
          date_start: '2023-06-01'
          date_end: '2024-05-22'
          description: I worked on [efficient sparse fine-tuning of LLMs with zeroth-order optimization methods](https://openreview.net/pdf?id=pW4MmsnVRq). 

        - title: Research Assistant
          company: Prof. Christopher De Sa, Cornell University
          company_url: ''
          company_logo: cornell
          location: Ithaca, NY
          date_start: '2021-06-01'
          date_end: '2023-05-31'
          description: I worked on (distributed) example orderings that produced the [CD-GraB](https://openreview.net/pdf?id=ISRyILhAyS) and [GraB](https://proceedings.neurips.cc/paper_files/paper/2022/file/3acb49252187efa352a1ae0e4b066ced-Paper-Conference.pdf) paper, and efficient high-precision floating-point arithmetic for hyperbolic representation learning as [MCTensor](https://arxiv.org/pdf/2207.08867.pdf) and [HTorch](https://github.com/ydtydr/HTorch).
  
        - title: Research Assistant
          company: Prof. Thorsten Joachims, Cornell University
          company_url: ''
          company_logo: cornell
          location: Ithaca, NY
          date_start: '2022-06-01'
          date_end: '2023-02-01'
          description: I worked on the [ranking with slot constraints](https://dl.acm.org/doi/pdf/10.1145/3637528.3672000) problem.

  # - block: experience
  #   content:
  #     title: Engineering Experience
  #     # Date format for experience
  #     #   Refer to https://wowchemy.com/docs/customization/#date-format
  #     date_format: Jan 2006
  #     # Experiences.
  #     #   Add/remove as many `experience` items below as you like.
  #     #   Required fields are `title`, `company`, and `date_start`.
  #     #   Leave `date_end` empty if it's your current employer.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - title: Developer Lead
  #         company: Pathways project, Cornell University
  #         company_url: ''
  #         company_logo: pathways
  #         location: Ithaca, NY
  #         date_start: '2021-06-01'
  #         date_end: '2023-05-31'
  #         description: |2-
  #             I designed search algorithms that provided diverse suggestions on course enrollment choices, constructed the backend codebase with Flask and MongoDB, and iterated search algorithms from students' feedback. I deployed and maintained the [Pathways website](https://pathways.cornell.edu/) to serve 3000 Cornell students. 
  
  #       - title: CMSX Backend Developer & Tester Lead
  #         company: CMSX Project, Cornell University
  #         company_url: ''
  #         company_logo: cmsx
  #         location: Ithaca, NY
  #         date_start: '2019-09-01'
  #         date_end: '2022-05-31'
  #         description: I fixed tens of production system bugs in Java and MySQL, contributed more than 11,000 lines of code, reviewed 76 peer's pull requests, and supervised new members and held weekly meetings to manage the team. The [CMSX website](https://www.cs.cornell.edu/Projects/cms/cmsx/) serves more than 8000 students in over 100 courses in Cornell University.

        # - title: Game Development Intern
        #   company: Tencent
        #   company_url: ''
        #   company_logo: qq-mobile
        #   location: Shenzhen, China
        #   date_start: '2020-06-15'
        #   date_end: '2020-08-15'
        #   description: I programmed game modules in Unity with C#, created tools to accelerate the loading time of Visual Studio projects, and benchmarked the performance of C# libraries on serialization and deserialization.

  # - block: portfolio
  #   id: others
  #   content:
  #     title: Ongoing Projects
  #     filters:
  #       folders:
  #         - project
  #     # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  #     default_button_index: 0
  #     # Filter toolbar (optional).
  #     # Add or remove as many filters (`filter_button` instances) as you like.
  #     # To show all items, set `tag` to "*".
  #     # To filter by a specific tag, set `tag` to an existing tag name.
  #     # To remove the toolbar, delete the entire `filter_button` block.
  #     buttons:
  #       - name: All
  #         tag: '*'
  #   design:
  #     # Choose how many columns the section has. Valid values: '1' or '2'.
  #     columns: '1'
  #     view: showcase
  #     # For Showcase view, flip alternate rows?
  #     flip_alt_rows: false

  - block: markdown
    content:
      title: Academic services
      subtitle: ''
      text: |-
        NeurIPS'23, ICLR'24, ICML'24, KDD'24, Journal of DMLR, NeurIPS'24, ICLR'25 reviewer
    design:
      columns: '2'

  - block: collection
    content:
      title: Teaching Experience
      filters:
        folders:
          - teaching
    design:
      columns: '2'
      view: compact

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Please feel free to contact me!
      # Contact (add or remove contact options as necessary)
      email: wg0420@princeton.edu
      # phone: 607 262 9493
      address:
        city: Princeton
        region: NJ
        postcode: '08540'
        country: United States
        country_code: US
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: Twitter
          link: 'https://twitter.com/WentaoGuo7'
        - icon: video
          icon_pack: fas
          name: Zoom
          link: 'https://princeton.zoom.us/my/wentaog'
      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
---
