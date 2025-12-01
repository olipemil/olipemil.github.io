---
layout: about
title: about
permalink: /
subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Motto. Etc.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>555 your office number</p>
    <p>123 your address street</p>
    <p>Your City, State 12345</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
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


Write your biography here. Tell the world about yourself. Link to your favorite [subreddit](http://reddit.com). You can put a picture in, too. The code is already in, just name your picture `prof_pic.jpg` and put it in the `img/` folder.

Put your address / P.O. box / other info right below your picture. You can also disable any of these elements by editing `profile` property of the YAML header of your `_pages/about.md`. Edit `_bibliography/papers.bib` and Jekyll will render your [publications page](/al-folio/publications/) automatically.

Link to your social media connections, too. This theme is set up to use [Font Awesome icons](https://fontawesome.com/) and [Academicons](https://jpswalsh.github.io/academicons/), like the ones below. Add your Facebook, Twitter, LinkedIn, Google Scholar, or just disable all of them.


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

