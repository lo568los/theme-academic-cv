---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-06-24
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: collection
    id: pubs
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

  - block: portfolio
    id: projects
    content:
      title: Ongoing Projects/Term Projects
      description: Here I describe my current projects and completed term papers which are unpublished and/or are undergoing peer review.
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
        - name: Q.Comp
          tag: QComp
        - name: Q.Info
          tag: QInfo
        - name: Stat Mech/CMT
          tag: Stat and CMT
        - name: Other
          tag: other
        
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  #- block: collection
   # id: featured
    #content:
     # title: Featured Publications
      #filters:
       # folders:
        #  - publication
        #featured_only: true
    #design:
     # columns: '2'
    #view: card
  - block: experience
    id: exp
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research Officer
          company: A*STAR Agency
          company_url: https://www.a-star.edu.sg/
          company_logo: org-astar
          location: Singapore
          date_start: '2025-01-06'
          date_end: ''
          description: |2-
              Working as an undergraduate researcher on quantum error correction. Responsibilities include:

              * Reviewing literature on Floquet codes and code-switching.
              * Analysing code-switching techniques relevant for fault tolerant logical gates in Floquet codes.
        - title: LTVSP Fellow
          company: ICTS Bangalore
          company_url: https://www.icts.res.in/
          company_logo: org-ICTS
          location: Bangalore
          date_start: '2024-08-02'
          date_end: ''
          description: |2-
              Working as an undergraduate researcher on Open Quantum systems. Responsibilities include:

              * Analytical calculations to study different types of Lindbladians
              * Modelling different types of System-Bath interactions in Python and MATLAB
              * Analysing entanglement and transport properties of the steady states
        - title: DAAD-WISE Fellow
          company: MPI Solid State Research
          company_url: https://www.fkf.mpg.de/en
          company_logo: org-MPI
          location: Stuttgart, Germany
          date_start: '2024-05-02'
          date_end: '2024-07-30'
          description: |2-
              Worked on the Research project titled "Emulating Kondo Physics on Quantum Chip". Responsibilities include:

              * Analytical calculations to arrive at a Quantum circuit for Kondo dynamics
              * Modelling different types of Quantum gates and states for running the circuit on
              * Analysing entanglement, spin and Hamiltonian heating properties

        - title: Online grader
          company: IPhO, EuPhO
          company_url: https://www.fkf.mpg.de/en
          company_logo: org-ipho
          location: ""
          date_start: '2024-08-02'
          date_end: '2023-07-30'
          description: |2-
          
              Graded and helped in deciding the final grading scheme for IPhO 2023 and EuPhO 2022, 2023 and 2024 as a paid volunteer. Also assisted in moderation rounds for deciding the final scores of students participating.
    design:
      columns: '2'
  
 
  
  

  - block: accomplishments
    id: certs
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Online Certifications'
      subtitle: Other certifications present on LinkedIn for the sake of brevity
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.credly.com/badges/82f72234-1190-4001-a6f3-c3fa2609e82b/public_url
          date_end: '2024-02-20'
          date_start: '2023-07-25'
          description: |2-
                    * Obtained the Advanced Badge as part of the Quantum Explorers 2023 Cohort
          icon: ibm
          organization: IBM Quantum
          organization_url: https://www.ibm.com/quantum
          title: Qiskit Quantum Explorers 2023-24
          url: ''
        - certificate_url: https://www.credly.com/badges/2e7d68ad-93a6-4a86-a809-0f779aaf4b4e/public_url
          date_end: '2023-07-31'
          date_start: '2023-07-14'
          description: |2-
                    * Got the Quantum excellence badge in Qiskit Global Summer school 2023
          icon: ibm
          organization: IBM Quantum
          organization_url: https://www.ibm.com/quantum
          title: Qiskit Global Summer School 2023-24
          url: ''
      #  - certificate_url: https://coursera.org/share/7d8f458be0e3e248340f5db1ad43f55e
      #    date_end: '2023-10-25'
      #    date_start: '2023-09-25'
      #    description: Understood how to organise ML projects and structure data splits
      #    icon: coursera
      #    organization: Coursera
      #    organization_url: https://www.coursera.org
      #    title: Structuring Machine Learning projects
      #    url: ''
      
      #  - certificate_url: https://coursera.org/share/7cfb3e3b3d062679d71374e9fbfbeab7
      #    date_end: '2023-09-25'
      #    date_start: '2023-08-25'
      #    description: Worked on implementing techniques like regularization on pet python projects
      #    icon: coursera
      #    organization: Coursera
      #    organization_url: https://www.coursera.org
      #    title: Improving Deep Neural Networks, Hyperparameter Tuning, Regularization and Optimization
      #    url: ''
      #  - certificate_url: https://coursera.org/share/04290b9899b5076f96163b8134d0372b
      #    date_end: '2023-08-25'
      #    date_start: '2023-07-25'
      #    description: Studied the basics concepts of neural Networks and Deep Learning
      #    icon: coursera
      #    organization: Coursera
      #    organization_url: https://www.coursera.org
      #    title: Neural Networks and Deep Learning
      #    url: ''
        
       
    design:
      columns: '2'

  - block: markdown
    id: gallery
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Contact details, if you wish to enquire about anything. I will respond in about 3-4 days upon receiving your message.
      # Contact (add or remove contact options as necessary)
      email: soumyadeepsarma3@gmail.com
      #phone: 888 888 88 88
      #appointment_url: 'https://calendly.com'
      #address:
       # street: 450 Serra Mall
       # city: Stanford
       # region: CA
       # postcode: '94305'
       # country: United States
       # country_code: US
      #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      #office_hours:
       # - 'Monday 10:00 to 13:00'
       # - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      #coordinates:
      #  latitude: '37.4275'
      #  longitude: '-122.1697'  
     # contact_links:
      #  - icon: twitter
       #   icon_pack: fab
        #  name: DM Me
         # link: 'https://twitter.com/Twitter'
        #- icon: skype
         # icon_pack: fab
          #name: Skype Me
         # link: 'skype:echo123?call'
        #- icon: video
         # icon_pack: fas
         # name: Zoom Me
         # link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      #form:
       # provider: netlify
       # formspree:
       #   id:
       # netlify:
          # Enable CAPTCHA challenge to reduce spam?
      #  captcha: false
    #design:
     # columns: '2'
---
