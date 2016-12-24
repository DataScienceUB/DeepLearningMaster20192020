---
output: jupyter_notebooks
---

## DeepLearningMaster Repository

This repository contains notebooks used in DEEP LEARNING COURSE of the MASTER OF FUNDATIONS IN DATA SCIENCE of the Universitat de Barcelona.


## Course Agenda

<li> Introduction to Deep Learning and its applications. Using the Jupyter notebook & Docker.
<li> Basic Concepts: Score & Loss functions, Optimization (SGD), Linear Regression.
<li> Automated differentiation, Backpropagation, Training a Neural Netwotk from Scratch.
<li> Tensorflow programming model. Keras & TFLearn. 
<li> Convolutions & CNN models.
<li> Recurrent Neural Netwoks.
<li> Unsupervised Learning.
<li> Advanced Applications: Time Series, Recommenders, Natural Language.

## Course Software Installation

The best way to run the course software is to use a Docker container. There’s full documentation on installing Docker at ``docker.com``, but in a few words, the steps are:

+ Go to ``docs.docker.com`` in your browser.
+ Step one of the instructions sends you to download Docker.
+ Run that downloaded file to install Docker.
+ At the end of the install process a whale in the top status bar indicates that Docker is running, and accessible from a terminal.
+ Click the whale to get ``Preferences``, and other options.
+ Open a command-line terminal, and run some Docker commands to verify that Docker is working as expected.
Some good commands to try are ``docker version`` to check that you have the latest release installed, and ``docker ps`` and ``docker run hello-world`` to verify that Docker is running. 
+ By default, Docker is set to use 2 processors. You can increase processing power for the app by setting this to a higher number in ``Preferences``, or lower it to have Docker for Mac use fewer computing resources.
+ Memory - By default, Docker is set to use 2 GB runtime memory, allocated from the total available memory on your computer. You can increase the RAM on the app to get faster performance by setting this number higher (for example to 3) or lower (to 1) if you want Docker to use less memory.

Once Docker is installed, you can dowload the image of this course:

+ In a terminal, go to your course folder and run (This operation requires a good internet connection; it will take some minutes):  ``docker pull datascienceub/deepub``    
+ Run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks datascienceub/deepub``
+ Once these steps have been done, you can check the installation by starting your web browser and introducing this  URL: ``http://localhost:8888``.
+ Open a new Jupyter notebook and execute this instruction in a code cell: ``!git clone https://github.com/jvitria/DeepLearningMaster``
