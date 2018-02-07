<div align="left">
        <img width="25%" src="deeplearninginside2.png" alt="About screen" title="About screen"</img>
</div>

## DeepLearningMaster Repository

This repository contains notebooks used in DEEP LEARNING COURSE of the [MASTER ON FOUNDATIONS OF DATA SCIENCE](http://www.ub.edu/datascience/master/) of the Universitat de Barcelona.

## Course Description

Deep learning is one of the fastest growing areas of machine learning and a hot topic in both academia and industry. This course will cover the basics of deep learning by using a hands-on approach.

## Course Instructor

[Jordi Vitrià](http://www.ub.edu/cvub/jordivitria/)

## Class Time and Location

+ 2ond Semester (February - May, 2018)
+ Lecture: Tuesday 15:00h-17:00h
+ Location: Aula B1, Facultat de Matemàtiques i Informàtica, Universitat de Barcelona. [Map](https://www.google.es/maps/place/Gran+Via+de+les+Corts+Catalanes,+585,+08007+Barcelona/@41.3865736,2.1619408,17z/data=!3m1!4b1!4m5!3m4!1s0x12a4a28cbeee3689:0x4b4a8ba716765923!8m2!3d41.3865736!4d2.1641295?hl=ca).

## Prerequisites

+ Proficiency in Python: All class assignments will be in Python (using tensorflow). 
+ Calculus, Linear Algebra, Optimization: You should be comfortable taking derivatives and understanding matrix vector operations and notation.
+ Basic Probability and Statistics.
+ Machine Learning.

## Grading

+ Assignment #1: 30%. Submission deadline (UB Campus Virtual):   
+ Assignment #2: 30%. Submission deadline (UB Campus Virtual): 
+ Assignment #3: 40%. Submission deadline (UB Campus Virtual): 

Study groups are allowed but we expect students to understand and complete their own assignments and to hand in one assignment per student.

## Course Agenda
<ol type="1">
<li>  Introduction to Deep Learning and its applications. Using the Jupyter notebook & Docker. Software stack. 
<li>  Basic concepts: learning from data.
<li>  Automated differentiation & Backpropagation, Training a Neural Network from Scratch.                     
<li>  Tensorflow programming model. Dense Neural Networks.                                                     
<li>  Tensorflow ecosystem: Keras, tf-contribution.                                                            
<li>  Recurrent Neural Netwoks I.                                                                              
<li>  Recurrent Neural Netwoks II.                                                                             
<li>  Embeddings.                                                                                              
<li>  Convolutional Neural Networks I.                                                                         
<li>  Convolutional Neural Networks for Large Scale Learning.                                                  
<li>  Unsupervised Learning I.                                                                                 
<li>  No class.                                                                                
<li>  Unsupervised Learning II.                                                                                  
<li>  Deep Learning & Recommenders.                                                                                     
</ol>



## Course Software Installation

The best way to run the course software is to use a **Docker container**. 

> A gentle introduction to docker: [How Docker Can Help You Become A More Effective Data Scientist](https://towardsdatascience.com/how-docker-can-help-you-become-a-more-effective-data-scientist-7fc048ef91d5)

There’s full documentation on installing Docker at ``docker.com``, but in a few words, the steps are:

+ Go to ``docs.docker.com`` in your browser.
+ Step one of the instructions sends you to download Docker.
+ Run that downloaded file to install Docker.
+ At the end of the install process a whale in the top status bar indicates that Docker is running, and accessible from a terminal.
+ Click the whale to get ``Preferences``, and other options.
+ Open a command-line terminal, and run some Docker commands to verify that Docker is working as expected.
Some good commands to try are ``docker version`` to check that you have the latest release installed, and ``docker ps`` and ``docker run hello-world`` to verify that Docker is running. 
+ By default, Docker is set to use 2 processors. You can increase processing power for the app by setting this to a higher number in ``Preferences``, or lower it to have Docker for Mac use fewer computing resources.
+ Memory - By default, Docker is set to use 2 GB runtime memory, allocated from the total available memory on your computer. You can increase the RAM on the app to get faster performance by setting this number higher (for example to 3) or lower (to 1) if you want Docker to use less memory.

Once Docker is installed, you can dowload the image of this course and dowload the git repository:

+ In a terminal, go to your course folder and run (This operation requires a good internet connection; it will take some minutes):  ``docker pull datascienceub/deepub``    
+ MacOS & Linux: Run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks datascienceub/deepub``
+ Windows: Run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v C:/your/course/folder:/notebooks datascienceub/deepub``
+ Once these steps have been done, you can check the installation by starting your web browser and introducing this  URL: ``http://localhost:8888``.
+ Open a new Jupyter notebook and execute this instruction in a code cell: ``!git clone https://github.com/DeepLearningUB/DeepLearningMaster``.

Next times, you can bring your local copy of the repository up to date:

+ Windows: In a terminal, go to your course folder and run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v C:/your/course/folder:/notebooks datascienceub/deepub``.
+ MacOS & Linux: In a terminal, go to your course folder and run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks datascienceub/deepub``
+ Start your web browser and introduce this  URL: ``http://localhost:8888``.
+ Open a new Jupyter notebook and execute this instruction in a code cell: ``!git pull https://github.com/DeepLearningUB/DeepLearningMaster``.


