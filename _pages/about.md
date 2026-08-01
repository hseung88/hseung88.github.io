---
layout: about
title: About
permalink: /
subtitle: >
  Postdoctoral Research Associate · University of Wisconsin–Madison

profile:
  align: right
  image: profile_old.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Morgridge Hall 4516</p>
    <p>1207 University Avenue</p>
    <p>Madison, WI 53706</p>
    <p><a href="mailto:hseung2@wisc.edu">hseung2 [at] wisc [dot] edu</a></p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit:  # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: false # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 0 # leave blank to include all the blog posts
---

<div class="about-text" lang="en" markdown="1">

I am a postdoctoral researcher in the Department of Statistics at the University of Wisconsin--Madison, where I work with 
Professor <a href="https://sites.google.com/view/katzfuss/home?authuser=0">
Matthias Katzfuss</a>. 
I received my Ph.D. in Statistics from the University of Georgia, 
advised by Professor <a href="https://ppmlguy.github.io/">Jaewoo Lee</a> 
and Professor <a href="https://yuan-ke.github.io/">Yuan Ke</a>.

My research is driven by a fundamental scalability challenge in modern machine learning.
Gradients and curvature often contain the local information needed to make 
learning more statistically and computationally efficient, but exploiting this 
information directly can be prohibitively expensive in high-dimensional settings. 
I develop methods that retain the useful structure in such information while 
reducing the memory, computation, and approximation costs that usually limit its use.

This principle connects my work on Gaussian processes, 
Bayesian optimization, and deep learning optimization. 
In Gaussian processes, I develop methods that use gradient observations for scalable prediction 
and data-efficient decision making without forming prohibitively 
large gradient covariance systems. In deep learning optimization, I develop 
curvature-aware methods for pretraining and fine-tuning that capture useful second-order 
structure under the memory and compute constraints of large-scale neural networks.

My current research directions include:

- scalable Gaussian processes with gradient observations
- Bayesian optimization and sample-efficient decision making
- memory-efficient fine-tuning of large language models
- curvature-aware optimization for deep neural networks

</div>
