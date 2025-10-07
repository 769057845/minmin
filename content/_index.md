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

  #- block: features
  # content:
  #    title: Skills
  #    items:
  #      - name: Model：SWAT model,  MIKE model
  #        description: ''
  #        icon: chart-line
  #        icon_pack: fas
  #      - name: Software：R, ArcGIS, SPSS, Origin, PS
  #        description: ''
  #        icon: r-project
  #        icon_pack: fab
  #      - name: Hobbies：Backpacking, Running, Traveling
  #        description: ''
  #        icon: camera-retro
  #        icon_pack: fas
  - block: experience
    content:
      title: Academic Performance
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Master of Hydrology and Water Resources
          company: GPA：3.80/4.00      Rank：1/96
          company_url: ''
          company_logo: org-gc
          location: Beijing Normal University
          date_start: '2021-09-01'
          date_end: '2024-07-01'
          description: |2-
              Major courses:

              * Water Quality Model and Simulation: A+ (Grade: 96/100)
              * Application and Development of Spatial Analysis Technology in Environment: A+ (Grade: 96/100)
              * Science of Hydrology and Water Resources: A (Grade: 94/100)
              * Environmental Forensics: A (Grade: 94/100)
              * Comparison of Environmental Issues between China and America: A+ (Grade: 95/100)
        - title: Bachelor of Geographical Science
          company: GPA：4.25/5.00   Rank：1/84
          company_url: ''
          company_logo: org-x
          location: Hunan Normal University
          date_start: '2017-09-01'
          date_end: '2021-07-01'
          description: |2-
              Major courses:

              * Meteorology and Climatology: A+ (Grade: 95/100)
              * Soil Geography: A+ (Grade: 95/100)
              * Geology and Geomorphology: A+ (Grade: 95/100)
              * Economic Geography: A (Grade: 94/100)
              * Professional English: A+ (Grade: 97/100)

          
    design:
      columns: '2'
  - block: collection
    id: featured
    content:
      title: Recent Publications
      text: ''
      count: 8  
      offset: 0
      order: asc     
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: Experiences
    content:
      title: Experiences
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
      order: asc
    design:
      # Choose a layout view
      view: compact
      columns: '2'

  - block: portfolio
    id: conference
    content:
      title: Conference Presentations
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
        - name: All;
          tag: '*'
        - name: Baosteel
          tag: Baosteel
        - name: Environmental Forum Award
          tag: Environmental Forum Award
        - name: World Geography Conference 
          tag: World Geography Conference 
        - name: Summer camp
          tag: Summer camp
        - name: River and Lake Ecological Forum
          tag: River and Lake Ecological Forum
        - name: Profile
          tag: Profile
         
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    id: gallery
    content:
      title: Gallery
      subtitle: I had a clearer vision of my strengths—personal drive, ability to make coherent and realistic decisions, unafraid to expand my comfort zone to embrace and discover new things about myself—that would make me a viable Ph.D. candidate.
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
 # - block: collection
 #  id: featured
 #   content:
 #     title: Featured Publications
 #     filters:
 #       folders:
 #         - publication
 #       featured_only: true
 #   design:
 #     columns: '2'
 #     view: card
 # - block: tag_cloud
 #   content:
 #     title: Popular Topics
 #   design:
 #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        After four years of rigorous study in geographical science during my B.S., three years of strict scientific research and lab training in environmental science and hydrology during my M.S., I am pursuing my studies toward a Ph.D. in 2025 Fall in the United States.
      # Contact (add or remove contact options as necessary)
      email: yangzm@mail.bnu.edu.cn
      phone: +86-18813185182
      address:
        street: No.19, Xinjiekouwai St, Haidian District
        city: Beijing
        postcode: China
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://www.facebook.com/profile.php?id=61573795989438'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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
