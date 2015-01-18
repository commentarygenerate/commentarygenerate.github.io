---
layout: post-no-feature
title: "Introduction to HOG3d features"
description: "Desciption and usage of HOG3d Features "
comments: true
category: articles
---


###CMU Winter School Program-December 2014 NITK Surathkal
This Blog is a basic introduction to we did for the Winter School program and our successes and failures.

Our Idea was to create an AI System that can generate Automatic commentary for Tennis matches.

We broke down the problem to few blocks so that we can divide the work amongst ourselves and work on the same.

They were  as follows-

*Player Detection

*Action Recognition

*Commentary generation

First we had to decide what features to use for detecting the action.This is a serious problem in Computer Vision.We went through few research papers and found that Calculation of local Spatio-Temporal Interest Points would be going forward in some direction.The Research paper is found here- http://www.irisa.fr/vista/Papers/2009_bmvc_wang.pdf

Basically,it uses a combination of HOG3D(Histogram Of Gradients) and HOF(Histogram of Optical Flow) to detect some interest point which might be an indicator of the action performed by a person.

The Code for calculating the STIP detector and descriptor can be found in the following website-

http://www.di.ens.fr/~laptev/download.html

Although I managed to view a demo version of the code and see what it does(with the help of http://web.michaelchughes.com/how-to/install-stip-software-with-opencv-v2),we were unable to make changes to it since it was dependent on a much older version of OpenCV which was 2.3.The binaries are already compiled and they require the OpenCV libraries of that version.

The Latest version is 3.0.0 and i was using the 2.4.9 version.So after installing required version as well,we were unable to make any sort of changes to it as it was leading to a build error when we used Cmake.

Hence we dropped the idea of using STIP and tried using HOF Features and the details of which can be view in the blog post written by my friend.

The Action Recognition requires calculation of large amounts of data and it seemed tedious and inefficient to track unnecessary movements such as player walking,ball-boys running etc.

So,to increase the efficiency of the Action Recognition algorithm,I started working on the Audio Analysis of the input Video.The basic understanding is that actions such as serve and hit are performed only when the ball hits the racquet and this is accompanied by the 'plopp!' sound(Honestly i tried searching for the right word to describe the sound but i found this!Others may describe it as Pock!/Plock! whatever.Well you know what i am talking about anyways :D )

If we can detect the time interval at which we know that sound is detected,then we can use that to increase the probability of our Action Recognition Algorithm's results at that instant accordingly.
~                               
