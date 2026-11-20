# Experiment-3.2 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-3.2
# Experiment-3.2

## Analysis of Speech Processing Workflows and Vision AI Architectures Using Microsoft Foundry.

## CO5

##

## Aim

To study the basic concepts of Computer Vision in Artificial Intelligence and understand how AI systems process, analyze, classify, detect, segment, interpret, and generate images.

## Objectives

The objectives of this experiment are:

- To understand the meaning and importance of computer vision.

- To study how images are represented using pixels and RGB channels.

- To understand filters, kernels, and convolution in image processing.

- To explain image classification, object detection, semantic segmentation, and contextual image analysis.

- To understand the basic workings of Convolutional Neural Networks.

- To study Vision Transformers and multimodal AI models.

- To understand image generation using diffusion models.

- To identify real-life applications of computer vision.

## Introduction

Computer vision is an important branch of Artificial Intelligence that enables computers to process and understand visual information from images, videos, and live camera feeds. It helps machines identify objects, detect locations, understand scenes, and generate descriptions from visual data.

Computer vision is used in many real-life applications such as autonomous vehicles, smart checkout systems, doorbell cameras, medical imaging, security systems, agriculture, robotics, and image generation tools.

A computer does not see an image like a human. It reads an image as numerical data made up of pixels. By analyzing these pixel values, AI models can understand objects, colors, shapes, textures, and patterns.

## Theory

## Computer Vision

Computer vision is the field of AI that allows machines to interpret and understand visual information. Its main purpose is to extract meaningful information from images or videos, as shown in Figure 1.

For example, a self-driving car uses computer vision to detect traffic lights, pedestrians, vehicles, and road signs. A smart checkout system uses computer vision to identify products automatically. A doorbell camera uses it to detect people at the door.

Computer vision combines image processing, machine learning, deep learning, pattern recognition, and neural networks.

## Figure 1: Comparison between human vision and computer vision systems.

## Image Representation

An image is made up of tiny units called pixels. A pixel is the smallest part of a digital image. Each pixel stores numerical information about brightness or color.

In a grayscale image, each pixel has a value from 0 to 255.

0 represents black.

255 represents white.

Values between 0 and 255 represent different shades of gray.

A color image usually has three channels: Red, Green, and Blue. This is called the RGB model.

Different combinations of red, green, and blue values create different colors. For example, red and green together can form yellow, while all three channels at maximum value form white.

## Image Processing

Image processing means applying operations on an image to improve it or extract useful information. It is used before applying AI models so that images become clearer and easier to analyze.

Common image processing tasks include:

Image enhancement

Noise removal

Edge detection

Blurring

Sharpening

Color correction

Conversion from color to grayscale

Image processing is important because raw images may contain noise, poor lighting, blur, or unwanted background information.

## Filters, Kernels, and Convolution

A filter is used to modify an image or extract features from it. A filter is represented by a small matrix called a kernel.

A kernel moves across the image and performs mathematical calculations on pixel values. This process is called convolution.

Different kernels create different effects. For example:

A blur kernel smooths the image.

A sharpening kernel makes details clearer.

An edge detection kernel highlights boundaries.

A Laplace filter detects sharp changes in pixel intensity.

Convolution is important because it helps identify visual features such as edges, lines, corners, shapes, and textures as shown in Figure 2.

Figure 2: Image filtering operation showing blurring and pixel shifting using convolution kernels.

## Image Classification

Image classification is a computer vision task in which an AI model predicts the label of an image.

For example, if an image contains an apple, the model may classify it as “apple.” If it contains a banana, the model may classify it as “banana.”

Image classification gives one main label for the entire image. It is used in fruit recognition, medical diagnosis, animal classification, face recognition, and document classification, as shown in Figure 3.

## Figure 3: Image classification process showing how a computer interprets image pixels and predicts object categories.

## Object Detection

Object detection is used to identify multiple objects in an image and show their locations. It gives both the name of the object and its position.

Object detection uses bounding boxes. A bounding box is a rectangular box drawn around an object.

For example, in an image containing an apple, banana, and orange, object detection can identify all three objects and draw separate boxes around them.

Object detection is used in self-driving cars, CCTV cameras, smart checkout systems, face detection, and traffic monitoring as shown in Figure 4.

## Figure 4: Object detection in a street scene using computer vision.

## Semantic Segmentation

Semantic segmentation is a more detailed computer vision task. In this technique, every pixel in an image is classified into a category.

Unlike object detection, which uses boxes, semantic segmentation marks the exact area of an object.

For example, in a road image, segmentation can mark road pixels, vehicle pixels, pedestrian pixels, and sky pixels separately.

Semantic segmentation is useful in medical imaging, autonomous vehicles, satellite image analysis, agriculture, and robotics, as shown in Figure 5.

## Figure 5: Image segmentation showing object-wise labeling of cat, cow, sky, trees, and grass.

## Contextual Image Analysis

Contextual image analysis means understanding not only objects in an image but also the relationship between them.

For example, if an image shows a person eating an apple, the system can understand the activity and generate the description:

“A person eating an apple.”

This technique is used in image captioning, visual question answering, AI assistants, content tagging, and accessibility tools.

## Convolutional Neural Network

A Convolutional Neural Network, or CNN, is a deep learning model widely used in computer vision. CNNs are designed to automatically learn important features from images.

A CNN usually contains:

Input layer

Convolutional layer

Activation function

Pooling layer

Flattening layer

Fully connected layer

Output layer

The convolutional layer applies filters to extract features. The pooling layer reduces the size of feature maps. The flattening layer converts feature maps into a one-dimensional array. The fully connected layer makes the final prediction.

CNNs are used for image classification, object recognition, face recognition, handwritten digit recognition, medical image analysis, and defect detection, as shown in Figure 6.

## Figure 6: Convolutional Neural Network architecture for image classification.

## Feature Maps and Training of CNN

When a filter is applied to an image, it creates a feature map. A feature map shows where important features such as edges, lines, or shapes are present.

During training, a CNN is given many labeled images. The model first makes predictions and compares them with the correct labels. If the prediction is wrong, it calculates the loss and adjusts its weights.

This process is repeated for many epochs. After training, the CNN learns useful patterns and can classify new images.

## Vision Transformers

Vision Transformers, also called ViTs, are modern computer vision models based on transformer architecture.

In Vision Transformers, an image is divided into small patches. Each patch is converted into a numerical vector. The model then uses attention to understand the relationship between different patches.

CNNs focus mainly on local features using filters, while Vision Transformers can understand global relationships in the image.

Vision Transformers are used in image classification, object recognition, medical image analysis, and multimodal AI systems as shown in Figure 7.

## Figure 7: Patch embedding and self-attention mechanism in Vision Transformer.

## Multimodal Models

Multimodal models are AI models that can process more than one type of data, such as text and images.

A vision model understands image features, while a language model understands words and sentences. When both are combined, the model can understand the relationship between images and text.

For example, if an image shows a person in a park with a hat and a backpack, a multimodal model can generate a description like:

“A person in a park with a hat and a backpack.”

Multimodal models are used in image captioning, visual question answering, AI assistants, image search, and text-to-image generation.

## Image Captioning and Visual Question Answering

Image captioning is the process of generating a text description for an image.

For example, an image of a dog running in a garden may be described as:

“A dog is running in a garden.”

Visual Question Answering, or VQA, allows a model to answer questions about an image.

For example, if an image shows a red car and the question is “What color is the car?”, the model may answer “red.”

Both tasks use computer vision and natural language processing together, as shown in Figure 8.

##

## Figure 8: Image captioning and visual question answering using a language model.

## Image Generation

Image generation is a modern AI technique in which models create new images from text prompts.

For example, if the prompt is:

“A dog carrying a stick in its mouth”

The AI model can generate an image matching the description.

Image generation models learn the relationship between words and visual features. They are used in design, education, advertising, entertainment, storytelling, and research visualization.

## Diffusion Models

Most modern image generation models use diffusion. A diffusion model starts with random noise and gradually removes the noise to create a meaningful image.

The process begins with random pixels. Then the model slowly forms shapes, colors, objects, and backgrounds according to the text prompt.

Diffusion models are powerful because they can generate realistic and creative images from natural language descriptions.

## Video Generation

Video generation is similar to image generation, but it creates a sequence of frames. These frames must follow a logical order to show motion.

Video generation is more complex because the model must understand movement, time, object behavior, and scene consistency.

It is used in animation, simulation, education, advertising, and entertainment.

## Difference Between CNN and Vision Transformer

CNN and Vision Transformer are both used in computer vision, but they work differently.

A CNN uses filters and convolution to extract features from images. It is effective for detecting edges, shapes, textures, and object parts.

A Vision Transformer divides an image into patches and uses attention to understand relationships between patches. It is useful for understanding the global context of an image.

In simple words:

CNN learns images using filters.

Vision Transformer learns images using patches and attention.

## Applications

Computer vision is used in many fields:

- Autonomous vehicles for detecting roads, traffic lights, vehicles, and pedestrians.

- Healthcare for analyzing X-rays, MRI scans, CT scans, and medical images.

- Smart checkout systems for recognizing products automatically.

- Security and surveillance for face detection and activity monitoring.

- Agriculture for crop monitoring and disease detection.

- Manufacturing for defect detection and quality inspection.

- Robotics for object recognition and navigation.

- Education for smart learning and image-based teaching.

- Accessibility tools for describing images to visually impaired users.

- Media and entertainment for image editing, AR, VR, and image generation.

## Code

# Import DeepFace for facial analysis

!pip install deepface  &> /dev/null

from deepface import DeepFace

# Import OpenCV for image handling

import cv2

# Import Matplotlib for image visualization

import matplotlib.pyplot as plt

# Load the input image using OpenCV

img1 = cv2.imread("/content/rachit.jpg")  # Reads the image file and stores it as an array

# Display the loaded image using Matplotlib

plt.imshow(img1)  # Converts the array back to an image format for visualization

plt.show()        # Displays the image on the screen

# Analyze the image using DeepFace for specific attributes

obj = DeepFace.analyze(img1, actions=['age', 'gender', 'race', 'emotion'])

# DeepFace analyzes the image to determine age, gender, race, and emotion

# 'actions' parameter specifies which attributes to analyze

# Print the entire analysis result as a dictionary

print(obj)  # Displays the results including all detected attributes

obj_first = obj[0]  # Get the first element if it's a list

print("Your age is", obj_first["age"],

"and you are", obj_first["dominant_race"],

"and current emotion is", obj_first["dominant_emotion"],

"and your gender capture is", obj_first["gender"])

## Practice Task Questions

- Write a short note on computer vision and explain any three real-life applications of it.

- Explain how an image is represented in a computer using pixels and numerical values.

- Differentiate between grayscale images and RGB color images with suitable examples.

- Explain the role of filters, kernels, and convolution in image processing.

- Describe image classification with an example of a fruit recognition system.

- Explain object detection and the use of bounding boxes in identifying objects.

- Differentiate between object detection and semantic segmentation.

- Draw and explain the basic architecture of a Convolutional Neural Network.

- Explain the difference between CNN and Vision Transformer in simple words.

- Write a short note on multimodal models and image generation using diffusion models.

## Video Links

Image classification vs Object detection vs Image segmentation

Introduction to Mask R-CNN for Image Segmentation

Vision Transformers Explained | The ViT Paper

Diffusion Models for AI Image Generation

Introduction to Image Generation

## Additional Resources

- Microsoft Learn: Introduction to Computer Vision Concepts

https://learn.microsoft.com/en-us/training/modules/introduction-computer-vision/

This resource covers computer vision tasks, filters, CNNs, Vision Transformers, and image generation.

- Azure AI Vision Documentation

https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/

Useful for understanding cloud-based computer vision services for image analysis and visual AI applications.

- Microsoft Azure: What is Computer Vision?

https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-computer-vision

This explains computer vision in simple terms and describes how computers process and understand images/videos.

- TensorFlow Tutorial: Convolutional Neural Network

https://www.tensorflow.org/tutorials/images/cnn

Useful for learning how CNNs classify images using TensorFlow and Keras.

- TensorFlow Tutorial: Image Classification

https://www.tensorflow.org/tutorials/images/classification

This explains a basic image classification workflow, including dataset preparation, model building, training, and evaluation.

- PyTorch: Transfer Learning for Computer Vision Tutorial

https://docs.pytorch.org/tutorials/beginner/transfer_learning_tutorial.html

Useful for learning how pretrained CNN models can be used for image classification tasks.

- PyTorch: TorchVision Object Detection Finetuning Tutorial

https://docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html

Useful for object detection and segmentation using a pretrained Mask R-CNN model.

- Google Machine Learning Crash Course

https://developers.google.com/machine-learning/crash-course

Helpful for understanding machine learning basics before studying CNNs and computer vision models.

- Keras Example: Image Classification from Scratch

https://keras.io/examples/vision/image_classification_from_scratch/

Useful for learning how to create an image classification model from image files.

- Learn PyTorch: Computer Vision

https://www.learnpytorch.io/03_pytorch_computer_vision/

This resource explains computer vision problems such as binary classification, multiclass classification, object detection, and segmentation.

## Textbooks

- Computer Vision: Algorithms and Applications — Richard Szeliski

PDF / Online Link: https://szeliski.org/Book/download.php

- Deep Learning — Ian Goodfellow, Yoshua Bengio, Aaron Courville

Online Link: https://www.deeplearningbook.org/

- Dive into Deep Learning — Aston Zhang, Zachary C. Lipton, Mu Li, Alexander J. Smola

PDF / Online Link: https://d2l.ai/

- Learning OpenCV — Gary Bradski and Adrian Kaehler

PDF Link: https://www.eecs.yorku.ca/course_archive/2010-11/W/4421/doc/LearningOpenCV_1_2.pdf

- First Principles of Computer Vision — Shree K. Nayar, Columbia University

PDF / Online Link: https://fpcv.cs.columbia.edu/Monographs

## Reference Books / Reference Resources

-  Deep Learning for Computer Vision—Stanford University

Online Notes Link: https://cs231n.github.io/

- Introduction to Computer Vision — Shree K. Nayar, Columbia University

PDF Link: https://cave.cs.columbia.edu/Statics/monographs/Introduction%20FPCV-0-1.pdf

- OpenCV-Python Tutorial — TutorialsPoint

PDF Link: https://www.tutorialspoint.com/opencv_python/opencv_python_tutorial.pdf

- TensorFlow Tutorial: Convolutional Neural Network

Online Link: https://www.tensorflow.org/tutorials/images/cnn

- PyTorch Tutorial: TorchVision Object Detection Finetuning

Online Link: https://docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html

---


## 🖥️ PRESENTATION SLIDES


# Experiment-3.2 - All Lecture Slides Text


## Exp 3.2
### Slide 1
- UNIVERSITY INSTITUTE OF
- ENGINEERING
- DEPARTMENT OF ENGINEERING FOUNDATION-2
- PROGRAM
- NAME
- :
- Bachelor
- of Engineering
- SPECIALIZATION
- :
- COMPUTER SCIENCE & ENGINEERING
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 3                   Experiment No.3.2
- Topic
- : Analysis of Speech Processing Workflows and Vision AI Architectures Using Microsoft Foundry
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- After
- completing this experiment, students will be able
- to:
- Understand
- computer vision concepts
- .
- Study
- image representation using pixels and RGB channels
- .
- Understand
- image classification, object detection and segmentation
- .
- Explain
- CNNs, Vision Transformers and multimodal models
- .
- Understand
- image generation using diffusion models.

### Slide 3
- Recap
- of Previous Experiment
- Speech-enabled AI applications allow users to interact with machines using voice.
- Speech recognition converts spoken language into written text.
- Speech synthesis converts written text into spoken audio.
- Together, speech recognition, NLP, and speech synthesis create conversational AI systems.
- These systems are widely used in voice assistants, customer support, healthcare, education, accessibility tools, navigation, and smart homes.

### Slide 4
- Figure-1 :
- Applications of
- Computer
- Vision in AI
- Source:
- https
- ://www.upgrad.com/blog/what-are-the-applications-of-computer-vision-in-ai/
- Topic(s
- )
- Topic 1: Computer Vision
- Topic 2: Image Classification
- Topic 3: Object Detection
- Topic 4: Optical Character Recognition
- Computer Vision
- and
- AI-Based Image Intelligence

### Slide 5
- Figure-2:
- Computer Vision in AI
- Source:
- https
- ://www.almabetter.com/bytes/tutorials/artificial-intelligence/computer-vision-in-ai
- Computer Vision in AI
- Computer vision is a branch of AI that helps machines understand visual information
- .
- It
- processes images, videos and live camera feeds
- .
- It
- is used in autonomous vehicles, smart checkout systems, medical imaging, doorbell cameras and surveillance systems.

### Slide 6
- A digital image is made up of pixels.
- Each pixel stores numerical
- information.
- Gray scale
- images use values from 0 to
- 255.
- Color
- images use RGB channels: Red, Green and
- Blue.
- Different
- RGB values
- create different
- colors.
- Figure-3
- :A rasterized form of the letter 'a' magnified 16 times using pixel doubling
- Source:
- https
- ://pippin.gimp.org/image-processing/chap_dir.html
- Image Representation

### Slide 7
- Image processing improves or extracts information from
- images.
- Filters
- are used for blurring, sharpening and edge
- detection.
- A
- kernel is a small matrix used to process pixel
- values.
- Convolution
- means moving the kernel over the image to extract features.
- Figure-4
- :Convolution Kernel
- Example
- Source:
- https
- ://muneebsa.medium.com/deep-learning-101-lesson-20-convolution-kernels-40641dda695d
- Image Processing, Filters and Kernels

### Slide 8
- Image classification predicts the main label of an image
- .
- Example
- : apple, banana, orange, dog or car.
- The
- model is trained using labeled images
- .
- It
- is used in fruit recognition, medical diagnosis, face recognition and document classification.
- Figure-5
- :Image Classification
- Source:
- https
- ://www.superannotate.com/blog/image-classification-basics
- Image Classification

### Slide 9
- Object detection identifies multiple objects and shows their locations using bounding boxes
- .
- Semantic
- segmentation classifies every pixel of an image
- .
- Object
- detection gives rectangular boxes.
- Semantic segmentation gives exact object regions
- .
- Both
- are useful in self-driving cars, healthcare and robotics.
- Figure-6
- :Object Detection
- and Semantic
- Segmentation
- Source:
- https
- ://manipulation.csail.mit.edu/segmentation.html
- Object Detection
- and
- Semantic Segmentation

### Slide 10
- CNNs are deep learning models used for image-related tasks
- .
- They
- automatically learn features from images
- .
- Main
- layers include input layer, convolutional layer, pooling layer, flattening layer, fully connected layer and output layer
- .
- CNNs
- are used in image classification, object recognition and medical image analysis.
- Figure-7 :
- Convolutional Neural Networks
- Source:
- https
- ://www.dragon1.com/terms/convolutional-neural-networks-definition
- Convolutional Neural Networks

### Slide 11
- Vision Transformers divide images into small patches
- .
- They
- use attention to understand relationships between image parts
- .
- Multimodal
- models combine image and text understanding
- .
- They
- are used in image captioning, visual question answering and AI assistants.
- Figure-8 :
- Vision Transformers and
- Multimodal Models
- Source:
- https
- ://www.linkedin.com/pulse/vision-transformers-vit-rise-multi-modal-deep-dr-satupati-jamalaiah-rvdqc/
- Vision Transformers and
- Multimodal
- Models

### Slide 12
- Image generation creates images from text prompts
- .
- Example
- : “A dog carrying a stick in its mouth
- .”
- Diffusion
- models start with random noise and gradually create a meaningful image
- .
- They
- are used in design, education, advertising, entertainment and research visualization.
- Figure-9
- :
- Image Generation and Diffusion Models
- Source:
- https
- ://www.geeksforgeeks.org/artificial-intelligence/diffusion-models-in-machine-learning/
- Image Generation and Diffusion Models

### Slide 13
- Summary of the
- Experiment
- Computer vision is a branch of Artificial Intelligence that helps machines understand images, videos, and camera inputs
- .
- Images
- are represented using pixels,
- gray scale
- values, and RGB color channels
- .
- Image
- processing uses filters, kernels, and convolution to improve images and extract important features
- .
- Major
- computer vision tasks include image classification, object detection, semantic segmentation, and contextual image analysis
- .
- CNNs
- and Vision Transformers are used to learn visual features and recognize patterns in images
- .

### Slide 14
- Next
- Experiment
- T
- opic(s)
- Introduction to Information
- Extraction
- Optical
- Character
- Recognition
- OCR Pipeline
- Field
- Extraction and Field Mapping

### Slide 15
- Quiz/ FAQ’s
- What is computer vision
- ?
- What
- is a pixel in a digital image
- ?
- What
- is the full form of RGB
- ?
- What
- is the difference between
- gray scale
- and RGB images
- ?
- What
- is the role of filters in image processing
- ?
- What
- is convolution in computer vision
- ?
- What
- is image
- classification? What
- is object detection
- ?
- What
- is the use of a bounding box
- ?
- What
- is the difference between CNN and Vision Transformer?

### Slide 16
- R
- eferences/ Articles/ Videos
- References / Articles
- Microsoft
- Learn — Introduction to Computer Vision Concepts
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/introduction-computer-vision
- /
- Microsoft
- Learn — What is Image Analysis?
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://
- learn.microsoft.com/en-us/azure/ai-services/computer-vision/overview-image-analysis
- Microsoft
- Learn — Get Started with Computer Vision in Azure
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/get-started-vision-azure
- /
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Videos
- Computer Vision Explained | What is Computer Vision?
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://www.youtube.com/watch?v=OcycT1Jwsns
- Image Classification
- vs
- Object Detection
- vs
- Image Segmentation
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId7"/></a:rPr><a:t>https://www.youtube.com/watch?v=taC5pMCm70U
- Convolutional Neural Networks Explained
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=YRhxdVk_sIs

### Slide 17
- Additional
- learning
- R
- esources
- TensorFlow
- — Computer Vision Tutorials
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://
- www.tensorflow.org/tutorials/images
- PyTorch
- —
- TorchVision
- Object Detection
- Fine tuning
- Tutorial
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://
- docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html
- Hugging
- Face — Diffusion Models Course
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://
- huggingface.co/learn/diffusion-course/en/unit0/1
- Microsoft
- Learn — Introduction to Computer Vision Concepts
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/introduction-computer-vision/

### Slide 18
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 19
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---
