---
layout: post
title: Open CV
project-id: openCV
description: Using OpenCV to stitch 2 images together
skills: 
- Python
- OpenCV

main-image: /images/openCV_combined.png
---

Autonomous warehouse robots require accurate environmental awareness to navigate safely. Traditional solutions such as LiDAR-based SLAM can be expensive, while line-following systems lack flexibility. This project explored a low-cost vision-based approach using overhead fisheye cameras to monitor multiple robots and obstacles within a simulated warehouse environment.

{% include image-gallery.html images="images/openCV_setup.png" height="500" %} <br> 

Using normal camera lenses, it produces the following two images. <br>
{% include image-gallery.html images="images/openCV_normalLens.png" height="300" %} <br>

Now, using fisheye camera lenses and then undistorting the perspective, we obtain the following image. <br>
{% include image-gallery.html images="images/openCV_distorted_fisheye.png" height="300" %} <br>
{% include image-gallery.html images="images/openCV_sift.png" height="300" %} 

Sift is used to automatically match points together. <br><br>

Below is the resulting merged images.
{% include image-gallery.html images="images/openCV_combined.png" height="300" %} <br>
