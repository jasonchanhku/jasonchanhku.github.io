---
title: "My Portfolio"
layout: splash
permalink: /portfolio/
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/unsplash-image-2.jpg
  cta_label: "More About Me"
  cta_url: "https://jasonchanhku.github.io/about/"
excerpt: "Welcome to my website where you will discover more about me and my professional projects alongside detailed documentations
of how I executed them from start to finish."
intro: 
  - excerpt: "# Professional Projects"
feature_row:
  - image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "UFC MMA Predictor"
    excerpt: "The world's first web app to predict winners of upcoming UFC MMA fights"
    url: "https://github.com/jasonchanhku/UFC-MMA-Predictor"
    btn_label: "View Project"
    btn_class: "btn--primary"  
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Financial Engineering"
    excerpt: "Capstone project where I structured, priced, and modeled returns of a complex product"
    url: "https://github.com/jasonchanhku/FINENG"
    btn_label: "View Project"
    btn_class: "btn--primary"
  - image_path: /assets/images/unsplash-gallery-image-3-th.jpg
    title: "Sic-Bo Betting"
    excerpt: "Implemented a Martingale strategy to ensure guaranteed profits on simulations"
    url: "http://nbviewer.jupyter.org/github/jasonchanhku/jupyternotebooks/blob/master/Macau%20%E5%A4%A7%E5%B0%8F%20simulation.ipynb"
    btn_label: "View Project"
    btn_class: "btn--primary"
intro2: 
  - excerpt: "# Machine Learning Playground"
feature_row2:
  - image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "R Pubs"
    excerpt: "My machine learning playground using machine learning libraries and experimenting using R"
    url: "http://www.rpubs.com/jasonchanhku"
    btn_label: "View Project"
    btn_class: "btn--primary"  
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "IPython Notebooks"
    excerpt: "Applying machine learning using Python libraries and presenting them in Jupyter Notebooks"
    url: "https://github.com/jasonchanhku/jupyternotebooks"
    btn_label: "View Project"
    btn_class: "btn--primary"
intro3: 
  - excerpt: "# Tableau Visualizations"
feature_row3:
  - image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "UFC Bantamweights"
    excerpt: "Webscraped data and images from UFC and visualized stats of UFC top Bantamweights"
    url: "https://public.tableau.com/profile/jason.chan.jin.an#!/vizhome/UFCTop5Bantamweights/UFCTop5Bantamweights"
    btn_label: "View Project"
    btn_class: "btn--primary"  
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Interactive Metrics"
    excerpt: "Demonstrated my parameter control and LOD skills by creating advanced analytics"
    url: "https://public.tableau.com/profile/jason.chan.jin.an#!/vizhome/InteractiveKeyMetricsDashboard/Dashboard1"
    btn_label: "View Project"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="intro2" type="center" %}

{% include feature_row id="feature_row2" %}

{% include feature_row id="intro3" type="center" %}

{% include feature_row id="feature_row3" %}

