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
  - block: portfolio
    id: projects
    content:
      title: Research Experience
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
        - name: Bioinformatics Analysis
          tag: Bioinformatics Analysis
        - name: Latent Class Analysis
          tag: Latent Class Analysis
        - name: MIMIC-III database
          tag: MIMIC-III database
        - name: Network Meta-Analysis
          tag: Network Meta-Analysis
        - name: Cohort Study
          tag: Cohort Study
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
      view: compact
  - block: collection
    content:
      title: Publications
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
  - block: features
    id: Skills
    content:
      title: Skills
      items:
        - name: R
          description: Throughout the course of conducting bioinformatics analyses and meta-analyses, I attained a comprehensive understanding of the R programming language
          icon: r-project
          icon_pack: fab
        - name: SQL & Navicat
          description: During the analysis of the MIMIC database, I acquired proficiency in using the SQL language and Navicat software
          icon: database
          icon_pack: fas
        - name: STATA & Rev Man
          description: Through engagement in meta-analysis and the analysis of MIMIC database, I have gained proficiency in utilizing the STATA software
          icon: square-poll-vertical
          icon_pack: fas
        - name: SPSS & PASS
          description: In the context of clinical cohort studies, I have acquired proficiency in utilizing the SPSS software
          icon: table
          icon_pack: fas
        - name: Mplus
          description: Throughout the process of latent class analysis, I gained proficiency in utilizing the Mplus software
          icon: m
          icon_pack: fas
        - name:  Cytoscape
          description: During the course of conducting bioinformatics analysis, I learned to use the Cytoscape software
          icon: hubspot
          icon_pack: fab
    design:
      columns: '6'
  - block: experience
    id: Experience
    content:
      title: Internship & rotation
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Rotate in Internal Medicine
          company: Zhongnan Hospital of Wuhan University
          company_url: https://www.znhospital.cn/index.html
          company_logo: ''
          location: Wuhan
          date_start: '2020-09-01'
          date_end: '2023-05-30'
          description: |2-

              * Residency training for 3 years
              * Obtained the certification as a licensed medical practitioner in China
              * Annual Outstanding Resident Physician of Zhongnan Hospital of Wuhan University in 2021
        - title: Internship
          company: Zhongnan Hospital of Wuhan University
          company_url: https://www.znhospital.cn/index.html
          company_logo: ''
          location: Wuhan
          date_start: '2019-06-01'
          date_end: '2020-06-01'
          description: Completed Internship rotations in the fields of Internal Medicine, Surgery, Obstetrics and Gynecology, and Pediatrics
    design:
      columns: '2'
  - block: collection
    id: Leadership
    content:
      title: Leadership & Volunteer Experience
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 6
      # Filter on criteria
      filters:
        folders:
          - Leadership
        author: admin
        category: ""
        tag: ''
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
  - block: accomplishments
    id: Honors & Awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Honors & Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: uploads/2022First_Prize_Scholarship.pdf
          date_end: ''
          date_start: '2022-10-25'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2022 First Prize Graduate Excellent Academic Scholarship of Wuhan University
          url: uploads/2022First_Prize_Scholarship.pdf
        - certificate_url: uploads/2022Outstanding_Graduate.pdf
          date_end: ''
          date_start: '2022-10-25'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2022 Outstanding Graduate of Wuhan University
          url: uploads/2022Outstanding_Graduate.pdf
        - certificate_url: uploads/2022Outstanding_Student_Leader.pdf
          date_end: ''
          date_start: '2022-09-01'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2022 Outstanding Student Leader
          url: uploads/2022Outstanding_Student_Leader.pdf
        - certificate_url: uploads/2021Outstanding-Resident-Physician.jpg
          date_end: ''
          date_start: '2022-01-12'
          description: ''
          organization: Zhongnan Hospital of Wuhan University
          organization_url: https://www.znhospital.cn/index.html
          title: Annual Outstanding Resident Physician of Zhongnan Hospital of Wuhan University in 2021
          url: uploads/2021Outstanding-Resident-Physician.jpg
        - certificate_url: uploads/2021_3rd_Clinical_Thinking_Competition.jpg
          date_end: ''
          date_start: '2021-10-29'
          description: ''
          organization: Zhongnan Hospital of Wuhan University
          organization_url: https://www.znhospital.cn/index.html
          title: Second Prize in the Team Category of the 3rd Clinical Thinking Competition held by Zhongnan Hospital of Wuhan University
          url: https://mp.weixin.qq.com/s/goDfKJD5kAaYDEsXOCWbNw
        - certificate_url: uploads/2021_3rd_EKG_personal1.jpg
          date_end: ''
          date_start: '2021-12-25'
          description: ''
          organization: Zhongnan Hospital of Wuhan University
          organization_url: https://www.znhospital.cn/index.html
          title: Second Prize in the Individual Category of the 3rd ECG Championship held by Zhongnan Hospital of Wuhan University
          url: https://mp.weixin.qq.com/s/p3U6mMwkpAEIn-gQY7WybQ
        - certificate_url: uploads/2021First_Prize_Scholarship.pdf
          date_end: ''
          date_start: '2021-12-27'
          description: ''
          organization: Wuhan University
          organization_url:  https://www.whu.edu.cn/
          title: 2021 First Prize Graduate Excellent Academic Scholarship of Wuhan University
          url: uploads/2021First_Prize_Scholarship.pdf
        - certificate_url: uploads/2020_2nd_EKG_team.jpg
          date_end: ''
          date_start: '2020-12-25'
          description: ''
          organization: Zhongnan Hospital of Wuhan University
          organization_url: https://www.znhospital.cn/index.html
          title: Third Prize in the Team Category of the 2nd ECG Championship held by Zhongnan Hospital of Wuhan University
          url: uploads/2020_2nd_EKG_team1.jpg
        - certificate_url: uploads/2020Outstanding_Bachelor_Graduates.jpg
          date_end: ''
          date_start: '2020-05-27'
          description: ''
          organization: Wuhan University
          organization_url:  https://www.whu.edu.cn/
          title: Outstanding Bachelor Graduates of Wuhan University
          url: uploads/2020Outstanding_Bachelor_Graduates.jpg
        - certificate_url: uploads/2020Photography_Contest_certi.jpg
          date_end: ''
          date_start: '2020-11-27'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: Second Prize in the Wuhan University Photography Contest
          url: uploads/2020Photography_Contest_title.jpg
        - certificate_url: uploads/2019_6th_Clinical_Skills_Competition.jpg
          date_end: ''
          date_start: '2019-12-09'
          description: ''
          organization: Wuhan University school of medicine
          organization_url:  https://wsm70.whu.edu.cn/
          title: Third Prize in the 6th Clinical Skills Competition of the Wuhan University school of medicine
          url: https://wsm70.whu.edu.cn/info/1043/14797.htm
        - certificate_url: uploads/2019First_Prize_Scholarship.jpg
          date_end: ''
          date_start: '2019-12-25'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2019 First Prize Scholarship for Outstanding Students of Wuhan University
          url: uploads/2019First_Prize_Scholarship.jpg
        - certificate_url: uploads/2019Huang_Zhangren.jpg
          date_end: ''
          date_start: '2019-12-24'
          description: ''
          organization: Wuhan University school of medicine
          organization_url: https://wsm70.whu.edu.cn/
          title: 2019 Huang Zhangren Special Scholarship
          url: uploads/2019Huang_Zhangren.jpg
        - certificate_url: uploads/2019merit_student.jpg
          date_end: ''
          date_start: '2019-12-26'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2019 Recognized as a Merit Student by Wuhan University
          url: uploads/2019merit_student.jpg
        - certificate_url: uploads/2019Anatomy_Illustration_picture.jpg
          date_end: ''
          date_start: '2019-04-21'
          description: ''
          organization: School of Basic Medical Sciences
          organization_url: https://wbm.whu.edu.cn/
          title: First Prize in the 3rd Anatomy Illustration Competition held by the School of Basic Medical Sciences of Wuhan University
          url: https://mp.weixin.qq.com/s/-x8f_w8F0V9Cu6QJrQj4bQ
        - certificate_url: uploads/2018Second_Prize_Scholarship.jpg
          date_end: ''
          date_start: '2018-12-26'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2018 Second Prize Scholarship for Outstanding Students of Wuhan University
          url: uploads/2018Second_Prize_Scholarship.jpg
        - certificate_url: uploads/2018Merit_Student.jpg
          date_end: ''
          date_start: '2018-12-25'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2018 Recognized as a Merit Student by Wuhan University
          url: uploads/2018Merit_Student.jpg
        - certificate_url: uploads/2018Internet_Plus.jpg
          date_end: ''
          date_start: '2018-12-25'
          description: ''
          organization: Medical Education Professional Committee of the China Higher Education Association
          organization_url: https://medu.bjmu.edu.cn/cms/show.action?code=publish_4028801e6bf38f43016c3cde03130479&siteid=100000&channelid=0000000055
          title: Outstanding Award in the Second National Internet Plus Smart Simulated Medical Clinical Skills Competition
          url: https://www.gmc.edu.cn/info/1058/13087.htm
        - certificate_url: uploads/2017_Second_Prize_Scholarship.jpg
          date_end: ''
          date_start: '2017-12-25'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2017 Second Prize Scholarship for Outstanding Students of Wuhan University
          url: uploads/2017_Second_Prize_Scholarship.jpg
        - certificate_url: uploads/2017Excellent_Student.jpg
          date_end: ''
          date_start: '2017-12-24'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2017 Recognized as an Excellent Student by Wuhan University
          url: uploads/2017Excellent_Student.jpg
        - certificate_url: uploads/2017Active_Student_Social.jpg
          date_end: ''
          date_start: '2017-09-24'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: Active Participant in Student Social Activities of Wuhan University
          url: uploads/2017Active_Student_Social.jpg
        - certificate_url: uploads/2017_2nd_Anatomy_Illustration_Competition.jpg
          date_end: ''
          date_start: '2017-04-24'
          description: ''
          organization: School of Basic Medical Sciences
          organization_url: https://wbm.whu.edu.cn/
          title: Second Prize in the 2nd Anatomy Illustration Competition held by the School of Basic Medical Sciences of Wuhan University
          url: https://mp.weixin.qq.com/s/jWPBj5x-OUypKCC9DoDA4g
        - certificate_url: uploads/2016Third_Prize_Scholarship.jpg
          date_end: ''
          date_start: '2016-12-25'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2016 Third Prize Scholarship for Outstanding Students of Wuhan University
          url: uploads/2016Third_Prize_Scholarship.jpg
        - certificate_url: uploads/2016Excellent_Student .jpg
          date_end: ''
          date_start: '2016-12-24'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: 2016 Recognized as an Excellent Student by Wuhan University
          url: uploads/2016Excellent_Student .jpg
        - certificate_url: uploads/2016Advanced_Individual_Student_Association.jpg
          date_end: ''
          date_start: '2016-12-23'
          description: ''
          organization: Wuhan University
          organization_url: https://www.whu.edu.cn/
          title: Advanced Individual of Student Association Guidance Center of Wuhan University
          url: uploads/2016Advanced_Individual_Student_Association.jpg
        - certificate_url: uploads/2016Experimental-Skills-Competition.jpg
          date_end: ''
          date_start: '2016-05-23'
          description: ''
          organization: School of Basic Medical Sciences
          organization_url: https://wbm.whu.edu.cn/
          title: Third Prize in the Individual Category of the Inaugural Basic Experimental Skills Competition held by the School of Basic Medical Sciences of Wuhan University
          url: https://wbm.whu.edu.cn/info/1217/4323.htm
        - certificate_url: uploads/2015Debate-Tournament.jpg
          date_end: ''
          date_start: '2015-12-23'
          description: ''
          organization: School of Basic Medical Sciences
          organization_url: https://wbm.whu.edu.cn/
          title: Third Prize in the Freshman Debate Tournament held by the School of Basic Medical Sciences of Wuhan University
          url: uploads/2015Debate-Tournament.jpg
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: hobbies
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        folders:
          - hobbies
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
  - block: tag_cloud
    content:
      title: Key Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        If you have any questions, feel free to leave me a message at any time
      # Contact (add or remove contact options as necessary)
      email: fengyujia@whu.edu.cn
      phone: +86 15971500416
      #appointment_url: 'https://calendly.com'
      address:
        street: 169 Donghu Road
        city: Wuhan
        region: Hubei
        postcode: '430071'
        country: China
        country_code: CHN
      #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      #office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/fngyji276788767'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:live:939772843'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://us05web.zoom.us/j/7203015946?pwd=VBE34Rc51vVzs8K25BnbbTJ6bvLCQp.1'
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
