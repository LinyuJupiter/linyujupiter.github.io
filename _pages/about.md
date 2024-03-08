---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Liu Fangxin, a native of Heyuan, Guangdong, was admitted to the School of Intelligent Engineering at Sun Yat-sen University (Shenzhen Campus) in 2021 through the college entrance examination. I am currently a junior majoring in Intelligent Science and Technology.

I enjoy programming and have developed two software applications based on Python (privacy restrictions prevent their display). These applications have hundreds of users, and I have handled all the frontend, backend, and operations work on my own. [Here](http://linyujupiter.icu) is my self-built website homepage, and [here](http://linyujupiter.icu:3003) is my blog website, welcome to visit.

Currently, I am assisting with some scientific research tasks under the guidance of Professor [Gao Chenqiang](https://gaocq.github.io/index.html)'s research group. My main focus is on computer vision, primarily participating in intelligent behavior detection tasks in classroom settings.


# 🔥 News
- *2024.02*: &nbsp;🎉🎉 Participated in the International Collegiate Mathematics Modeling Competition (MCM/ICM) with two classmates from the same major, serving as the paper writer, and completed and submitted the paper on time.

- *2024.01*: &nbsp;🎉🎉 During the winter internship at Fenghua High-Tech, an intelligent document assistant application and an intelligent material robot application built with another colleague received high praise from the leadership. The project has been reported to the parent company for project demonstration.

- *2023.08*: &nbsp;🎉🎉 During the summer internship, independently designed and developed the software “Xiaobai Self-Installation (Yichun Edition)” which was launched successfully. The client was satisfied and settled the contract fees.

- *2023.05*: &nbsp;🎉🎉 The software “Sanqi Automatic Recognition (Online Edition)” was launched, attracting a large number of user resources. The software has been combined with the local edition and continuously updated and maintained.

- *2023.03*: &nbsp;🎉🎉 The self-developed software “Sanqi Automatic Recognition (Local Edition)” was launched, and user experience feedback was positive.

- *2022.07*: &nbsp;🎉🎉 Ranked in the top third of the computer science category (Shenzhen) among a total of 900 students, and entered the School of Intelligent Engineering to continue undergraduate studies in Intelligent Science and Technology as the first choice.

- *2021.07*: &nbsp;🎉🎉 Ranked 44th in the science department of Heyuan Middle School in the college entrance examination, and was admitted to Sun Yat-sen University for computer science (Shenzhen) with a provincial ranking of around 4900.

- *2018.08*: &nbsp;🎉🎉 Entered Heyuan Middle School for high school with the top score in the school (top 20 in the city) in the middle school entrance examination.

# 💬 Projects

## Key Special Project: Classroom Behavior Dataset Construction
*2023.10 - Present* - Core Team Member
- Constructing a high-quality large-scale dataset to explore behavior recognition in densely populated classroom settings;
- Using Python to crawl a large number of classroom scene videos from platforms such as YouTube and Youku, and using FFmpeg to clip videos into multiple 2-second segments;
- Utilizing the Baize BasicFinder system to verify and annotate the dataset, participating in video behavior timing localization, and extracting key time points of behavior duration;
- The research is currently at the stage of demonstrating the rationality of single video clipping, and the next stage will test the effects on SOTA models and compare them with other traditional datasets.

## Interactive Behavior Recognition in Classroom Settings
*2023.09 - Present* - Core Team Member
- Developed a technical plan based on the YoLov5 object detection module and the slowfast-based behavior classification module;
- Built and debugged project code on a Linux system, fixed vulnerabilities, and continuously optimized, configuring the server environment;
- Preprocessed the large-scale AVA dataset, used OpenCV to batch extract and classify video frames, organized valid labels, and converted label formats using Python;
- Trained the pretrained model provided by slowfast, trained different model structures with multiple configuration changes, and established a project demo to showcase the results;
- Preprocessed the large-scale Kinetics-400 dataset, used FFmpeg to batch clip and scale videos, extracted valid video labels, completed the dataset format configuration required for the slowfast network, and distributed the training of slowfast on multiple GPUs using the processed dataset to obtain pretrained models;
- Currently in the stage of adjusting network hyperparameters to improve accuracy, with the next step being to train new pretrained models on the new dataset.

## Fault-Tolerant Distributed Key-Value Storage System Based on Raft
*2023.11 - 2024.01* - Personal Project
- Implemented a fault-tolerant distributed key-value (KV) storage system using Go language, based on the project framework from MIT's 6.824 Distributed Systems course;
- Referenced the Raft-Extended paper to complete functionalities such as Raft Leader election and heartbeat, log replication and consistency, snapshot mechanism, and log compaction;
- Designed both the client and server sides, perfected functions like CRUD (Create, Read, Update, Delete), and integrated the database with the Raft algorithm;
- Developed a fault tolerance scheme and completed failure tests for scenarios such as node disconnection, RPC packet loss, and network partitioning;
- Conducted high-concurrency testing, and the system is capable of processing a large number of concurrent requests within the specified time.

## Apple Tree Leaf Disease Detection Based on Convolutional Neural Networks
*2023.10 - 2023.11* - Personal Project
- Performed one-hot encoding on the dataset labels, transforming the multi-classification task into a multi-label classification task;
- Designed and trained neural network models using both the LeNet and VIT architectural frameworks, compared the performance of CrossEntropyLoss versus ArcFaceLoss in addressing fine-grained classification issues, and the final trained LeNet model achieved an accuracy rate of 89.5% on the test set.

## Vehicle Traffic Analysis System Based on YoLov8 and Tesseract-OCR
*2023.06 - 2023.07* - Personal Project
- Trained a YoLo neural network model for vehicle type recognition and tested it on multiple road surveillance videos;
- Trained a Tesseract-OCR model for handwritten text recognition and applied it to license plate text recognition;
- Designed a vehicle traffic counting algorithm using Python, implemented object tracking with the BoT-SORT algorithm, and determined traffic flow through regional judgments;
- Developed the project UI using the tkinter library, added simple interactive controls and information display widgets, facilitating the expansion and application of the project.

## Automatic Pathfinding and Control Simulation for a Car Based on Simulink
*2023.06 - 2023.07* - Personal Project
- Implemented path planning from start to finish using the A* algorithm on randomly generated 2D maps by the system;
- Designed scaling and interpolation strategies to optimize the generated feasible paths with Bezier curve interpolation and the De Casteljau algorithm, and smoothed the paths in segments to handle collision issues;
- Used MATLAB programming to solve for LQR parameters, calculated the ABQR matrices corresponding to the car's parameters, and established a k-value table for the LQR controller;
- Designed a PID controller for lateral control of the car and an LQR controller that integrates the car's lateral speed and path curvature for longitudinal control;
- Conducted path tracking simulations for the car using Simulink, established a controller simulation model, and successfully guided the car to the finish line in one attempt without collisions;
- Secured a top 3 finish in the MATLAB group (out of 35 participants) in a racing competition.

## C++ Implementation of a Two-Player Chinese Chess Game
*2022.11 - 2023.01* - Personal Project
- Designed the program's underlying architecture, including base classes for chess pieces and the chessboard, a vector for piece states, and derived classes for 14 types of chess pieces. Stored piece viability using a vector-like class, and employed a move prediction and post-move validation strategy to ensure piece movement logic adhered to the rules;
- Utilized IO streams and a custom file format to save and load game progress, and added a detection mechanism to prevent unreasonable endgame situations;
- Designed the UI interface using QT Designer, added custom controls, and created an installer package with Visual Studio. The project achieved first place in the class (out of 47 students).


# 🎖 Honors and Awards
- *2024.02* Mathematical Contest in Modeling(MCM/ICM). 
- *2023.03* Third Prize in the First "Intelligent Data Cup" Data Analysis Competition of the School of Intelligent Engineering in 2023. 

# 📖 Educations
- *2021.09 - 2025.06 (now)*, Sun Yat sen University Shenzhen Campus, School of Intelligent Engineering, majoring in Intelligent Science and Technology, Shenzhen. 
- *2018.09 - 2021.06*, Heyuan Middle School (High School), Heyuan. 

# 📝 Publications 
- None

# 💻 Internships
## *2024.01 - 2024.02*, [Guang Dong Fenghua Advanced Technology (Holding) Co.,Ltd.](https://www.china-fenghua.com/), Artificial Intelligence Engineer, Zhaoqing.
- Developed an intelligent order report management program to batch process company order warehousing efficiently.
- Based on open-source large models such as chatGLM-6b and qwen-7b, used company documents to develop, train, and deploy the Fenghua Artificial Intelligence document large model.
- Organized the company's material database, used embedding models and reranker models to establish a material knowledge base, and developed an intelligent material information customer service application in conjunction with the large model.
- Developed the backend interfaces for the company's procurement material platform and completed the database integration work.

## *2023.07 - 2023.08*, Guangdong Wanshida Intelligent Technology Co., Ltd, Software Development Intern, Heyuan.
- Delved into the smart platform project for the decoration industry, independently developing a one-stop platform software for the client company based on Python and MySQL.
- Matched technical solutions to customer needs, set up an anaconda virtual environment, and designed the software's underlying architecture to enable features such as chat and shopping modules.
- Built a MySQL database to facilitate frontend-backend interaction, designed a graphical interface for the frontend, and completed the design and writing of interfaces by encapsulating SQL statements in the backend.
- Utilized the tkinter library to design the software's UI interface and interaction logic according to requirements, used the ttkbootstrap library to beautify the interface and make it adaptable to multi-resolution windows.
- Created an installation package with Inno Setup and wrote project documentation and usage instructions.
