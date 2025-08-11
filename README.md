# AAI-511_Final_Project
Final Project for USD AAI511 - Music Genre and Composer Classification Using Deep Learning

This project is a part of the AAI-511 course in the Applied Artificial Intelligence Program at the University of San Diego (USD).
-- Project Status: [Completed]

Installation

Using a browser, navigate to https://colab.research.google.com/. From there, upload the ipynb files to run our training jupyter notebooks.

In the AAI511ML_Final_Project_Composer_Model.ipynb file, change the paths for the drive directories to your drive path. This way you will be able to save the models to your drive directory for later evaluation in the code. After changing all the drive paths, your code should be able to run from start to finish without issues.
  
Project Intro/Objective
The main purpose of this project is to be able to identify composers by their music. By doing so, we will be able to build various tools around the prediction process. This can be useful for education, data collection of unknown musical compositions, and more.


Partner(s)/Contributor(s)  
⦁	D. Keith Holder, Victor Hsu
⦁	dholder@sandiego.edu, vhsu@sandiego.edu

Methods Used
⦁	Deep Learning


Technologies
⦁	Python
⦁	Tensorflow
⦁	MatPlot (graphing libraries)
⦁	sk-learn libraries (evaluation of model)
⦁	Keras (high lvl API used with tensorflow)

Project Description

Data source: https://www.kaggle.com/datasets/blanderbuss/midi-classic-music - A dataset with a large number of music files by various composers
Vocabulary Size (unique notes/chords): 55053
(After splitting the data)
Training samples: 642152
Validation samples: 160539

We had to do significant tuning to get the model to reach the classification numbers that we found. We added a CNN block to find local musical patterns, added dropout, a custom learning rate, early stopping, and more various techniques we learned throughout the course. We tried different models (bidirectional) and used keras tuner to find optimal hyperparameters.

To perform evaluation, we utilized the sklearn library.

We encountered some roadblocks in the pre-processing step where it was taking a very long time to preprocess the data into musical notes/chords. After multithreading the process it went much more smoothly. Even then, highly recommend the paid version of colab to run this code at a fair speed. Colab was an important tool in terms of resources for training which helped to speed along training/evaluation.

License

CC0: Public Domain
https://creativecommons.org/publicdomain/zero/1.0/

Acknowledgments
Thanks to the professor for teaching us, and to the team who worked hard on this project.
