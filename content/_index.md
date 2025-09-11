---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      image:
        filename: header.png
      text: | 
        <span style="font-size: clamp(14px, 2vw, 22px); line-height: 1.4">SBI4C is an interdisciplinary research project that develops new methodologies for parameter inference in large-scale physical simulators, with <span style="color: green; font-weight: bold">climate science</span> as its central application domain. It is primarily funded by the [MIAI cluster](https://miai-cluster.univ-grenoble-alpes.fr/en/) in Grenoble, France.</span>
  
  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 2
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: card
      columns: '3'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
