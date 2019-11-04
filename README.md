# Image Classification with Watson Visual Recognition and Watson Studio  

## Table of Contents

* [Overview](#overview)
* [Lab 0 Setup (Pre-Requisite)](#lab-0-setup-pre-requisite)
* [Lab 1 Using Pre Trained and Custom Classifiers with Watson Visual Recognition](#lab-1-using-pre-trained-and-custom-classifiers-with-watson-visual-recognition)
* [Lab 2 Object Detection with Power AI](#lab-3-object-detection-with-power-ai)
* [Lab 3 Visual Recognition and Object Detection using a Pre Trained MAX Model](#lab-3-visual-recognition-and-object-detection-using-a-pre-trained-max-model)
* [Lab 4 Developing a Custom Visual Recognition Classifier with Watson Studio](#lab-4-developing-a-custom-visual-recognition-classifier-with-watson-studio)
* [Conclusion](#conclusion)
* [Reference](#references) 


## Overview
The explosive growth of cameras, image sensors, and computer vision as a discipline of Artificial Intelligence (AI) has garnered strong interest from researchers, businesses, and the general public. One of the main area’scomputer vision employs amachine learning technique known as deep learning to conduct analysis on vast sources of visual content. Such types of analysis include image classification, object detection, and object tracking. Image classification refers to a process to classify an image according to a model and match it to a set of classes or categories [1]. Object detection is similar to image classification, which is a process to classify, locate and count multiple objects in an image and their respective locations within the image [2]. Object tracking involves using object detection in each frame of a video to track the desired object through a series of image frames or video [3].There are a number of use cases for computer vision including face recognition for application or device security, automatically counting and classifying items on a production line, and monitoring and responding to traffic conditions on busy road sections. 

In the world of computer vision, data and model are the two keys. Data in this context refers to visual content, including image and video, while a data set refers to a collection of those items. A model is a set ofalgorithms tuned to produce some desired output based on some input. The common analysis procedure includes the following steps: Prepare representative data for model training; create a model based on deep learning; train and validate the model with some data sets as input; and finally deploy the model. 

[IBM Watson Studio](https://www.ibm.com/watson) is IBM’s suite of enterprise-ready AI services, applications and tooling. As a service on IBM Cloud, IBM Watson Visual Recognition uses deep learning algorithms to analyze images for scenes, faces, and objects. This service provides built-in models and can also be used to create and train custom models for specific needs. Watson Studio provides a collaborative platform on top of IBM Cloud's cloud computing capabilities to use existing models or train and deploy new models with minimal coding. Watson Studio has the added capability of setting up custom environments and Notebooks,llowing quick, cloud-enabled development machines that can scale as your projects scale. 

[IBM PowerAI Vision](https://www.ibm.com/ca-en/marketplace/ibm-powerai-vision) is a Graphics Processing Unit (GPU) accelerated visual recognition solution running on IBM Power Systems. PowerAI Vision [4] puts data science in the hands of subject matter experts. This tool simplifies building machine learning models with IBM Power Systems. As a result, users can build models and deploy them to the web without coding. The models can be accessed through an Application Program Interface (API). On the other hand, users can call the API from their own applications with a few lines of code.IBM provides developers free, open source, state-of-the-art assets for deep learning through the [Model Asset Exchange (MAX)](https://developer.ibm.com/exchanges/models/)on IBM Developer.In the repository developers can find both assets for training deep learning models and pre-trained models to use in their projects. 

The first half of this workshop will focus on exploring the Watson Visual Recognition and Watson Studio service in IBM Cloud. We will begin by building and deploying a model on Watson Visual Recognition. We will focus on the key benefits of the service, including the ability of anyone with minimal coding experience to be able to train and deploy a computer vision model to the cloud. We will then demonstrate how easy it can be to integrate the model in any web-enabled application through a demo web application. 

Next we will demonstrate detecting and labeling objects within an image using [PowerAI Vision object detection](https://github.com/IBM/powerai-vision-object-detection), based on customized training. Instead of writing code to train, deploy, and test the new model, we will only need to upload the images, and label the objects in the provided application. Once the model is deployed, we will use the PowerAI Vision user interface (UI) to test it. We will also use our application as a Representational State Transfer (REST) client to locate and count objects in an image using the provided REST API endpoint. In our application, we will upload an image, label the objects in the image, call the REST API for object detection, and finally display the returned result. 

Next we will introduce you to the Model Asset Exchange which is a free open source repository of deployable and trainable deep learning models for visual recognition, speech and natural language processing. You will navigate through the user interface to find and learn how to use a deployable object detection model through different methods such as the provided Swagger docs, deploy and invoke the model from a container running on IBM Cloud and use it in a Node-Red flow.

The second half of the workshop is a deep dive into building a custom visual recognition model using Watson Studio, Jupyter Notebooks and Keras and Tensor flow. You will start the lab with an introduction to Watson studio, followed by setting  up  a  [Jupyter  notebook](https://jupyter.org/), and then go over some prepared code snippets to train and analyze a model fully on the cloud. We will then demonstrate how we can export the model and use it in our applications. 


## Labs
## Lab 0 Setup (Pre-Requisite)
In [this lab](./Lab-0/README.md) you will:

* Setup and IBM Cloud Account
* Provision instances of the Watson Visual Recognition, Watson Studio and Cloud Object Storage services
* Get familiar with the IBM Cloud web dashboard and service dashboards
* Understand how visual recognition works with a demo applicaion

## Lab 1 Using Pre Trained and Custom Classifiers with Watson Visual Recognition 
In [this lab](./Lab-1/README.md) you will:
* Learn how to use Watson Visual Recognition to classify an image using the pre trained classifiers. 
* Use Watson Visual Recognition to build a custom classifier. 
* Learn how to use/test the classifier and APIs by calling the APIs from the command line using cURL
* Learn how to use/test the classifier using a Python code snippet from a Watson Studio Jupyter Notebook

## Lab 2 Object detection with Power AI
In [this lab](./Lab-2/README.md) you will 
* Learn about Power AI
* Watch a demo of how to use the intuitive user interface in Power AI to build custom models to classify images and detect objects in images and video.
* Test and evaluate your visual recognition models.

## Lab 3 Visual Recognition and Object Detection using a Pre Trained MAX Model
In [this lab](./Lab-3/README.md) you will:
* Learn how to use a deployable or trainable visual recognition deep learning model available in the Model Asset Exchaing to classify images and detect objects in an Image. 

## Lab 4 Developing a Custom Visual Recognition Classifier with Watson Studio
In [this lab](./Lab-4/README.md) you will:
* Learn how to use Watson Studio to build a custom visual recognition model.

## Conclustion
In summary, we will introduce some visual recognition services provided by IBM in this workshop. We will explore built-in image classification models available in Watson Visual Recognition and then develop a custom image classification model using Watson Visual Recognition and Watson Studio. Then we discuss the features of PowerAI Vision and demonstrate object detection using PowerAI Vision. We then introduce the Model Asset Exchange and give you a tour of it by showing you how deployable and custom deep learning models like the Object Detector model can easily be deployed and consumed in your application. Finally, we get into a deep dive hands-on workshop of building a custom image classification model using a Jupyter notebook running in Watson Studio and using Keras and Tensor.
 
## References
[1] FNMSurname(2018). Article Title. Journal Title, 10(3), 1–10.  
[2] F.N.MSurname, Article  Title, https://www.acm.org/publications/proceedings-template.  
[3] F.N.MSurnameand F.N.MSurname,2018Article Title, The title of book two(2nd. ed.).Publisher Name, City, State, Country.  
[4] IanEditor(Ed.). 2018. The title of book two(2nd. ed.).University of XXXPress, City, Chapter 100. DOI:http://dx.doi.org/10.1000/0-000-00000-0.  
[5] Watson Studio https://www.ibm.com/cloud/watson-studio/details  
[6] PowerAI Vision https://www.ibm.com/ca-en/marketplace/ibm-powerai-vision  
[7] Model Asset Exchange https://developer.ibm.com/exchanges/models/  
[8] Object Detector MAX Model https://github.com/IBM/powerai-vision-object-detection  
[9] Deep learning and AI on IBM Power Systems https://developer.ibm.com/linuxonpower/deep-learning-powerai/  
[10]Getting started with Watson Visual Recognition https://developer.ibm.com/technologies/vision/series/learning-path-watson-visual-recognition  
[11] Getting Started with PowerAI Vision https://developer.ibm.com/technologies/vision/series/learning-path-powerai-vision  





