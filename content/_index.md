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
        <span style="font-size: clamp(14px, 2vw, 22px)">SBI4C is an interdisciplinary research project that develops new methodologies for parameter inference in large-scale physical simulators, with <span style="color: green; font-weight: bold">climate science</span> as its central application domain. It is primarily funded by the <a href="https://miai-cluster.univ-grenoble-alpes.fr/en/" target="_blank" style="text-decoration: none;"><b>MIAI cluster</b></a> in Grenoble, France.</span>

        <div style="text-align: center; margin-top: -0.25;">
          <img src="logos-index.svg" alt="MIAI logo" style="margin-top:0.5em; max-width: 450px; width: 40vw; height: auto; display: inline-block;" />
        </div>

  - block: markdown
    content:
      text: |
        <section class="panel goals-panel">
          <div class="goals-grid">
            <div class="goals-left">
              <h3 class="goals-title">Goals</h3>
              <p>The overarching goal of SBI4C is to extend 
              <a href="https://arxiv.org/abs/2508.12939" target="_blank" rel="noopener"><b>simulation-based inference</b></a>
              methods to large-scale models such as climate simulators that capture complex ocean–atmosphere dynamics. Our main use-case is the important problem of tuning (i.e. calibration) of parametrizations of sub-grid processes in climate models.
              </p>
            </div>
            <div class="goals-right">
              <div class="goal-item">
                <h3>More with less</h3>
                <p style="font-size: large">Design SBI methods that deliver robust results despite few expensive simulator runs.</p>
              </div>
              <div class="goal-item">
                <h3>Better approximators</h3>
                <p style="font-size: large">Tailored SBI architectures beyond off-the-shelf deep models.</p>
              </div>
              <div class="goal-item">
                <h3>Fast surrogates</h3>
                <p style="font-size: large">Leveraging emulators for fast, reliable SBI.</p>
              </div>
              <div class="goal-item">
                <h3>Dissemination</h3>
                <p style="font-size: large">Organization of workshops, summer school, and a hackathon.</p>
              </div>              
            </div>
          </div>
        </section>

  - block: collection
    content:
      title: | 
        <span style="font-size: clamp(14px, 2vw, 28px); font-weight: bold">Latest News</span>
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
