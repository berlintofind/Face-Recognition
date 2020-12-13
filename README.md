# Face-Recognition
Face Recognition application with FaceNet

By Tianyang Zhao

## Table of Contents
1. Introduction
2. Models
3. Results
4. Reference

## Introduction
This repository contains the Face Recognition model. The goal of the model is to recognize if the person is identified in the database by comparing the 128-dimensional encodings.

#### Packages Version
1. Python 3.6.9 
2. tensorflow-gpu 1.13.1
3. numpy 1.19.1
4. CUDA Version 10.1
5. scipy 1.2.1
6. keras-gpu 2.3.1


## Models
The model is built based on FaceNet. The concept comes from Google InceptionNet. The weights of pre-trained model can be loaded by the function load_weights_from_FaceNet.
The triplet loss is an effective loss function for training a neural network to learn an encoding of a face image.The same encoding can be used for verification and recognition. Measuring distances between two images' encodings allows you to determine whether they are pictures of the same person.

The user can test with his own image by changing the name of image in line 190.

**Keep safe and see you soon!**


## Reference
1. [Florian Schroff, Dmitry Kalenichenko, James Philbin (2015). FaceNet: A Unified Embedding for Face Recognition and Clustering](https://arxiv.org/pdf/1503.03832.pdf)
2. [Yaniv Taigman, Ming Yang, Marc'Aurelio Ranzato, Lior Wolf (2014). DeepFace: Closing the gap to human-level performance in face verification](https://research.fb.com/wp-content/uploads/2016/11/deepface-closing-the-gap-to-human-level-performance-in-face-verification.pdf)
3. [The pretrained model used is inspired by Victor Sy Wang's implementation and was loaded using his code:]( https://github.com/iwantooxxoox/Keras-OpenFace)
4. [The implementation also took a lot of inspiration from the official FaceNet github repository](https://github.com/davidsandberg/facenet)
