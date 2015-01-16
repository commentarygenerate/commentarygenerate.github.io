---
layout: post_without_image
permalink: /methodology/index.html
title: Methodology
description: Approach
tags: [methodology, commentary,generator]
<!-- image:
  feature: soft-trees.jpg -->
---


Owing to the complexity of the problem statement, we aim at a simpler problem statement. Since the action, the objects and the sound captures the essence of the entire tennis match video, we inspect each of the problem statement seperately and try to make inferences out of it. Once efficient results can be obtained for the individual parts, we can combine them to render an efficient end to end system.

<img src="/images/simple.png" alt="Reduced Problem Statement" style="width:60%">

<h4 style="text-align:center"><b>Appraoch</b></h4>
<!-- ![Reduced Problem Statement]({{ site.url }}/images/simple.png )

![Reduced Problem Statement]({{ site.url }}/images/pr_2.png )
 -->

<img src="/images/pr_2.png" alt="Reduced Problem Statement" style="width:60%;">

<h4 style="text-align:center"><b>Reduced Problem Statement</b></h4>


### Work Flow

We consider a modular approach to the problem and the solution has the following major components:

- Tennis Court Detection (Applied Homographic and Hough Transforms)
- Object Detection (Applied Regions with Convoluted Neural Networks (RCNN))
- Action Recognition (Applied SVM (classifier) to extracted HOF features)
- Ball Tracking (Optical Flow)
- Sound Analysis (Naive Bayes Classifier on sound features)

<img src="/images/flow.png" alt="Reduced Problem Statement" style="width:100%">

<h4 style="text-align:center"><b>Work Flow</b></h4>

<!-- ### Features
* flexible, uses max-width for responsive goodness
* responsive drop down menu
* retina images using @2x
* post loop in the footer showing 3 latest post
* custom portfolio page for case studies

### Acknowledgements
I utilized my own HTML templates, but had no prior knowledge of liquid nor the required Jekyll system file format. I took [Michael Rose](http://twitter.com/mmistakes)'s theme [Minimal Mistakes](http://mmistakes.github.io/minimal-mistakes/). Having a prebuilt archive and the YAML front-matter already set up was a great help. 

 The lovely font shown here is Calendas. For full splendor on your blog, I suggest you [head over and buy that](http://calendasplus.com/). The full family is 3 weights and costs $3. Many thanks to Daniel Bruce for the wonderful Entypo icons. Those can be picked up at [entypo.com](http://entypo.com), but are included with the source files. It's also <b>retina ready</b> via retina.js. Check out how that works over at [retinajs.com](http://retinajs.com).

### The Name
Balzac was a famous writer, known for his beautiful prose. I read some Balzac in school, but mostly feel comfort in the name of my favorite coffee shop in Stratford, Ontario. 
 -->
