---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
      image:
        filename: welcome.jpg
      text: |
        <br>
        
        The **Radboud Respiratory Failure and Mechanical Ventilation Research Group** is a center of excellence for Respiratory Failure and Mechanical Ventilation research, teaching, and practice.
  
  - block: collection
    id: news_1
    content:
      title: Latest News
      subtitle:
      text:
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: news
    design:
      view: card
      columns: '1'

  - block: collection
    id: blog_1
    content:
      title: Blog
      subtitle: 
      text: 
      # Display content from the `content/post/` folder
      filters:
        folders:
          - blog
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      # Choose your content listing view - here we use the `showcase` view
      view: showcase
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: true

  - block: collection
    id: projects_1
    content:
      title: Projects
      subtitle: 
      text: 
      # Display content from the `content/post/` folder
      filters:
        folders:
          - projects
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      # Choose your content listing view - here we use the `showcase` view
      view: showcase
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: true

  - block: people
    id: team_1
    content:
      title: Meet the Team
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - Principal Investigators
          - Researchers
          - Graduate Students
          - Administration
          - Visitors
          - Alumni
      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: true
      show_role: true
      show_social: true

  - block: collection
    id: publications_1
    content:
      title: Latest Publications
      text: |
        {{% cta cta_link="./publications/" cta_text="See all publications→" %}}
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article-journal'

    design:
      view: citation
      columns: '2'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./contact/" cta_text="Contact us →" %}}
    design:
      columns: '1'
---
