---
layout: about
title: about
permalink: /
subtitle: Tayebati Postdoctoral Fellow at MIT

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---


<style>
    .image-container {
        position: relative;
        display: inline-block;
    }

    .image-hover {
        transition: opacity 0.3s ease;
        display: block;
    }

    .image-container:hover .image-hover {
        opacity: 0.3;
    }

    .image-hover:hover {
        opacity: 0.3;
    }

    .overlay-text {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%; 
        display: flex; 
        justify-content: center;
        align-items: center;
        color: black;
        font-size: 16px;
        font-weight: bold;
        opacity: 0;
        pointer-events: none; 
        /*pointer-events: auto;  Ensures the div can receive click events */
        transition: opacity 0.3s ease;
    }

    .image-container:hover .overlay-text {
        opacity: 1;
        pointer-events: auto;
    }

    /* New navigation styling */
    .main-navigation {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        margin: 30px 0;
        justify-content: center;
    }

    .nav-card {
        border: 2px solid #ddd;
        border-radius: 12px;
        padding: 25px;
        flex: 1;
        min-width: 250px;
        max-width: 320px;
        transition: all 0.3s ease;
        background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
        text-align: center;
    }

    .nav-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        border-color: #2c5aa0;
        background: linear-gradient(135deg, #ffffff 0%, #f8f9fa 100%);
    }

    .nav-card h3 {
        margin-top: 0;
        margin-bottom: 15px;
        font-size: 1.3em;
    }

    .nav-card h3 a {
        text-decoration: none;
        color: #2c5aa0;
        display: block;
    }

    .nav-card h3 a:hover {
        color: #1a365d;
    }

    .nav-card p {
        color: #666;
        margin-bottom: 15px;
        font-size: 0.95em;
    }

    .nav-features {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
        justify-content: center;
    }

    .nav-features span {
        background: #e3f2fd;
        color: #1565c0;
        padding: 6px 12px;
        border-radius: 16px;
        font-size: 0.8em;
        font-weight: 500;
        border: 1px solid #bbdefb;
    }

    .nav-card:hover .nav-features span {
        background: #2c5aa0;
        color: white;
        border-color: #2c5aa0;
    }

    /* API links styling */
    .api-links {
        background: #f1f8ff;
        border: 1px solid #c0d3eb;
        border-radius: 8px;
        padding: 12px 20px;
        margin: 15px 0 30px 0;
        text-align: center;
        font-size: 0.9em;
    }

    .api-links a {
        color: #0366d6;
        text-decoration: none;
        font-weight: 500;
        margin: 0 5px;
    }

    .api-links a:hover {
        text-decoration: underline;
        color: #0253ba;
    }

</style>

Ph.D. Materials Science and Engineering and Scientific Computing at University of Michigan
B.S. Physics at Idaho State University

I am a postdoc working at MIT with Prof. Tess Smidt and Prof. Jeffery Grossman to build better representations of quantum materials data. This increases our chemical understanding of materials properties while improving machine learning architectures for simplified training.

My scientific interests center around decoding complicated quantum simulations into chemically intuition frameworks to reveal the covalent, ionic, and metallic bonds which conspire to shape in material properties.

During my PhD, I creating the toolkit Crystal Orbital Guided Iteration To atomic-Orbitals (COGITO). 
This combined the devleopment of novel algorithms to parse DFT wavefunctions into an adaptable, maximally unique atomic basis with a powerful user inferface to visualization bonding and charge transfer in crystals. 
For more information, check out the [COGITO website](https://olipemil.github.io/cogito-website/) or the [COGITO paper](https://arxiv.org/abs/2511.19725). 
COGITO was created in the [Sun group](https://whsunresearch.group/) and [Kioupakis group](https://kioupakisgroup.engin.umich.edu/) at University of Michigan.



<div class="main-navigation">
    <div class="nav-card">
        <h3><a href="{{ site.baseurl }}/tutorial/"> Tutorial</a></h3>
        <p>Step-by-step guide to using COGITO</p>
        <div class="nav-features">
            <span>Installation</span>
            <span>Basic Usage</span>
            <span>Advanced Analysis</span>
        </div>
    </div>

    <div class="nav-card">
        <h3><a href="{{ site.baseurl }}/api/"> API Documentation</a></h3>
        <p>Complete reference for all COGITO functions</p>
        <div class="nav-features">
            <span>COGITO Core</span>
            <span>Post-processing</span>
            <span>Visualization</span>
        </div>
    </div>

    <div class="nav-card">
        <h3><a href="{{ site.baseurl }}/examples/"> Examples</a></h3>
        <p>Interactive Jupyter notebook examples</p>
        <div class="nav-features">
            <span>Workflows</span>
            <span>Tutorials</span>
            <span>Use Cases</span>
        </div>
    </div>
</div>

