<div align="left">
        <img width="25%" src="images/deeplearninginside2.png" alt="About screen" title="About screen"</img>
</div>

## DeepLearningMaster Repository

This repository contains notebooks used in 2019/2020 DEEP LEARNING COURSE of the [MASTER IN FUNDAMENTAL PRINCIPLES OF DATA SCIENCE](http://www.ub.edu/datascience/master/) of the Universitat de Barcelona.

## Course Description

Deep learning is one of the fastest growing areas of machine learning and a hot topic in both academia and industry. This course will cover the basics of deep learning by using a hands-on approach.

## Course Instructor

[Jordi Vitrià](http://www.ub.edu/cvub/jordivitria/)

## Class Time and Location
+ First Semester (September, 2019 - January, 2020)
+ Lectures: Wednesday 17:00h-19:00h
+ Location: Aula B1, Facultat de Matemàtiques i Informàtica, Universitat de Barcelona.  [Map](https://www.google.es/maps/place/Gran+Via+de+les+Corts+Catalanes,+585,+08007+Barcelona/@41.3865736,2.1619408,17z/data=!3m1!4b1!4m5!3m4!1s0x12a4a28cbeee3689:0x4b4a8ba716765923!8m2!3d41.3865736!4d2.1641295?hl=ca).

## Prerequisites

+ Proficiency in Python (3.7): All class assignments will be in Python (using ``tensorflow`` and ``keras``). 
+ Calculus, Linear Algebra: You should be comfortable taking derivatives and understanding matrix vector operations and notation.
+ Basic Probability and Statistics.

If you are not used to Git, you can complete this free online git [course](https://try.github.io/levels/1/challenges/1)

## Grading

+ Assignment #1: 30%. Submission deadline (UB Campus Virtual): **TBD**
+ Assignment #2: 30%. Submission deadline (UB Campus Virtual): **TBD**
+ Assignment #3: 40%. Submission deadline (UB Campus Virtual): **TBD**

Study groups are allowed but we expect students to understand and complete their own assignments and to hand in one assignment per student.

## Course Agenda
<ol type="1">
<li>  Introduction to Deep Learning and its applications. Using the Jupyter notebook & Docker. Software stack. 
<li>  Basic concepts: learning from data.
<li>  Automated differentiation & Backpropagation, Training a Neural Network from Scratch.                     
<li>  Tensorflow programming model. Dense Neural Networks.                                                     
<li>  Keras.                                                           
<li>  Recurrent Neural Netwoks I.                                                                              
<li>  Recurrent Neural Netwoks II.                                                                             
<li>  Embeddings.                                                                                              
<li>  Convolutional Neural Networks I.                                                                         
<li>  Convolutional Neural Networks for Large Scale Learning.                                                  
<li>  Unsupervised Learning I.                                                                                 
<li>  Unsupervised Learning II.                                                                                  
<li>  Deep Reinforcement Learning.                                                                                     
</ol>

## Course Software Installation: Working in Colab

You can develop deep learning applications with Google Colaboratory (Colab) -on the free Tesla K80 GPU- using Keras and Tensorflow. Colab is a Google internal research tool for data science. They have released the tool sometime earlier to the general public with a goal of dissemination of machine learning education and research. This is a free service that may not always be available, and requires extra steps to ensure your work is saved. Be sure to read the docs on the Colab web site to ensure you understand the limitations of the system.

For accessing Colab, first of all you should sign in to you Google account if you are not signed in by default. You must do this step before opening Colab, otherwise the notebooks will not work. 

Next, head on to the Colab Welcome Page (https://colab.research.google.com) and click on ‘Github’. In the ‘Enter a GitHub URL or search by organization or user’ line enter ‘https://github.com/DataScienceUB/DeepLearningMaster2019’. You will see all the courses notebooks listed there. Click on the one you are interested in using.

You should see your notebook displayed now. Before running anything, you need to tell Colab that you are interested in using a GPU. You can do this by clicking on the ‘Runtime’ tab and selecting ‘Change runtime type’. A pop-up window will open up with a drop-down menu. Select ‘GPU’ from the menu and click ‘Save’.

When you run the first cell, you will face a pop-up saying ‘Warning: This notebook was not authored by Google’; you should leave the default tick in the ‘Reset all runtimes before running’ check box and click on ‘Run Anyway’.

If you opened a notebook from Github, you will need to save your work to Google Drive. You can do this by clicking on ‘File’ and then ‘Save’. 

Click on ‘SAVE A COPY IN DRIVE’. This will open up a new tab with the same file, only this time located in your Drive. If you want to continue working after saving, use the file in the new tab. Your notebook will be saved in a folder called Colab Notebooks in your Google Drive by default.

If you run a script which creates/ downloads files, the files will NOT persist after the allocated instance is shutdown. To save files, you need to permit your Colaboratory instance to read and write files to your Google Drive. Add the following code snippet at the beginning of every notebook.

```python
from google.colab import drive
drive.mount('/content/gdrive', force_remount=True)
root_dir = "/content/gdrive/My Drive/"
base_dir = root_dir + 'masterUB/'
```

Now, you may access your Google Drive as a file sytem using standard python commands to both read and write files. 

You can find more information in these blogs: 
+ https://medium.com/deep-learning-turkey/google-colab-free-gpu-tutorial-e113627b9f5d
+ https://medium.com/tensorflow/colab-an-easy-way-to-learn-and-use-tensorflow-d74d1686e309

## Course Software Installation: Working with Docker

You can run the course software using a **Docker container**. 

> A gentle introduction to docker: [How Docker Can Help You Become A More Effective Data Scientist](https://towardsdatascience.com/how-docker-can-help-you-become-a-more-effective-data-scientist-7fc048ef91d5)

There’s full documentation on installing Docker at ``docker.com``, but in a few words, the steps are:

+ Go to ``docs.docker.com`` in your browser.
+ Step one of the instructions sends you to download Docker.
+ Run that downloaded file to install Docker.
+ At the end of the install process a whale in the top status bar indicates that Docker is running, and accessible from a terminal.
+ Click the whale to get ``Preferences``, and other options.
+ Open a command-line terminal, and run some Docker commands to verify that Docker is working as expected.
Some good commands to try are ``docker version`` to check that you have the latest release installed, and ``docker ps`` and ``docker run hello-world`` to verify that Docker is running. 
+ By default, Docker is set to use 2 processors. You can increase processing power for the app by setting this to a higher number in ``Preferences``, or lower it to use fewer computing resources.
+ Memory - By default, Docker is set to use 2 GB runtime memory, allocated from the total available memory on your computer. You can increase the RAM on the app to get faster performance by setting this number higher (for example to 3) or lower (to 1) if you want Docker to use less memory.

Once Docker is installed, you can download the **image of this course** and download this git repository:

+ In a terminal, go to your course folder and run (This operation requires a good internet connection; it will take some minutes):  ``docker pull datascienceub/deepub``    
+ MacOS & Linux: Run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks datascienceub/deepub``
+ Windows: Run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v C:/your_course_folder_path:/notebooks datascienceub/deepub``
+ Once these steps have been done, you can check the installation by starting your web browser and introducing the referred URL.
+ Finally, to have the contents of this repository in your computer, open terminal from your browser and execute this instruction: ``git clone https://github.com/DataScienceUB/DeepLearningMaster2019``.

To run this image:

+ Windows: In a terminal, go to your course folder and run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v C:/your_course_folder_path:/notebooks datascienceub/deepub``.
+ MacOS & Linux: In a terminal, go to your course folder and run the ``deepub`` image on your system: ``docker run -it -p 8888:8888 -p 6006:6006 -v /$(pwd):/notebooks datascienceub/deepub``
+ Start your web browser and introduce the corresponding URL.

Next times, if there are new contents in the repository, you can bring your local copy of the repository up to date:

+ Open a new Jupyter notebook and execute this instruction in a code cell: 
``!git pull https://github.com/DataScienceUB/DeepLearningMaster2019``

