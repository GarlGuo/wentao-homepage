---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Developer Lead
          company: [Pathways project, Cornell University](https://pathways.cornell.edu/)
          company_url: ''
          company_logo: pathways
          location: Ithaca, NY
          date_start: '2021-06-01'
          date_end: '2023-05-31'
          description: |2-
              I constructed backend codebases with Flask and MongoDB, designed search algorithms that provided diverse suggestions on course enrollment choices, and iterated search algorithms from students’ feedback. I deployed and maintained the [website](https://pathways.cornell.edu/) to serve 3000 Cornell students. 
      
        - title: CMSX Backend Developer & Tester Lead
          company: [CMS Project, Cornell University](https://www.cs.cornell.edu/Projects/cms/cmsx/)
          company_url: ''
          company_logo: cmsx
          location: Ithaca, NY
          date_start: '2019-09-01'
          date_end: '2022-05-31'
          description: I fixed 10s MySQL and Java production bugs on backend, created 75 and reviewed 76 peer’s pull requests, and supervised new members and held weekly meetings to manage the team. The [website](https://www.cs.cornell.edu/Projects/cms/cmsx/) serves more than 8000 students in over 100 courses in Cornell University..

        - title: Game Development Intern
          company: Tencent
          company_url: ''
          company_logo: qq-mobile
          location: Shenzhen, China
          date_start: '2020-06-15'
          date_end: '2020-08-15'
          description: I programmed game modules in Unity with C#, created tools to accelerate project loading and compilation time, and analyzed the performance of C# libraries on serialization and deserialization.

    design:
      columns: '2'

  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'
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
      buttons:
        - name: All
          tag: '*'
        - name: Machine Learning
          tag: Machine Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
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
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: markdown
    content:
      title: Academic service
      subtitle: ''
      text: |-
        NeurIPS'23, ICLR'24 reviewer
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        I am looking for a PhD position starting in Fall 2024. Please feel free to contact me!
      # Contact (add or remove contact options as necessary)
      email: wg247@cornell.edu
      phone: 607 262 9493
      address:
        street: 120 Valentine Place
        city: Ithaca
        region: NY
        postcode: '14850'
        country: United States
        country_code: US
      directions: Room 3042
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: Twitter
          link: 'https://twitter.com/Twitter'
        - icon: video
          icon_pack: fas
          name: Zoom
          link: 'https://cornell.zoom.us/j/9666296642?pwd=VEtjTTdCeTRtcWxsUmk5NTlMQ1ZuUT09'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
