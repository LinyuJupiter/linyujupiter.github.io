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

Liu Fangxin, a native of Heyuan, Guangdong, graduated from the School of Intelligent Engineering at Sun Yat-sen University in 2025 with a major in Intelligent Science and Technology. Currently pursuing a master's degree in Information Engineering at The Chinese University of Hong Kong.

I enjoy programming and have developed two software applications based on Python (privacy restrictions prevent their display). These applications have hundreds of users, and I have handled all the frontend, backend, and operations work on my own. [Here](http://134.175.123.166) is my self-built website homepage, and [here](http://134.175.123.166:3003) is my blog website, welcome to visit.

I previously worked with Professor [Gao Chenqiang](https://gaocq.github.io/index.html)'s research group on computer vision tasks, primarily focusing on behavior detection in classroom settings. I have published one SCI paper in the fourth quartile.

Later, I worked with Associate Professor [Shen Ying](https://sysu-hcp.net/faculty/442.html) in the field of large language models, completing my undergraduate thesis on "Research on Acceleration Algorithms and Accuracy Improvement Methods for Large Model RAG."

Currently working at Tencent Financial Technology as a Test Development Engineer, focusing on improving development efficiency using artificial intelligence technologies such as large language models.

# 🔥 News
- *2025.04*: &nbsp;🎉🎉 Paper "Dual-branch vision transformer for low-resolution action recognition" accepted by SCI journal "Multimedia Tools and Applications".

- *2024.07*: &nbsp;🎉🎉 Joined Tencent Financial Technology as a Test Development Engineer, working on improving development efficiency using AI technologies.

- *2024.06*: &nbsp;🎉🎉 Won the Hebei Province Second Prize in the "Challenge Cup" China College Student Entrepreneurship Competition.

- *2024.02*: &nbsp;🎉🎉 Participated in the International Collegiate Mathematics Modeling Competition (MCM/ICM) with two classmates from the same major, serving as the paper writer, and completed and submitted the paper on time.

- *2024.01*: &nbsp;🎉🎉 During the winter internship at Fenghua High-Tech, an intelligent document assistant application and an intelligent material robot application built with another colleague received high praise from the leadership. The project has been reported to the parent company for project demonstration.

- *2023.08*: &nbsp;🎉🎉 During the summer internship, independently designed and developed the software "Xiaobai Self-Installation (Yichun Edition)" which was launched successfully. The client was satisfied and settled the contract fees.

- *2023.05*: &nbsp;🎉🎉 The software "Sanqi Automatic Recognition (Online Edition)" was launched, attracting a large number of user resources. The software has been combined with the local edition and continuously updated and maintained.

- *2023.03*: &nbsp;🎉🎉 The self-developed software "Sanqi Automatic Recognition (Local Edition)" was launched, and user experience feedback was positive.

- *2022.07*: &nbsp;🎉🎉 Ranked in the top third of the computer science category (Shenzhen) among a total of 900 students, and entered the School of Intelligent Engineering to continue undergraduate studies in Intelligent Science and Technology as the first choice.

- *2021.07*: &nbsp;🎉🎉 Ranked 44th in the science department of Heyuan Middle School in the college entrance examination, and was admitted to Sun Yat-sen University for computer science (Shenzhen) with a provincial ranking of around 4900.

# 💬 Projects

## screenshot2code - A Tool for Converting Web Screenshots to HTML Code Based on GLM-4
*2023.12 - 2024.01* - Personal Project [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="20"/>](https://github.com/LinyuJupiter/screenshot2code)
- Developed a tool that uses domestic large language models to recognize web page styles from screenshots and generate page code
- Explored the capabilities of domestic large models in visual recognition and code generation, selecting GLM-4 as the technical solution
- Built backend interfaces using FastAPI, designed prompts for visual large models to recognize screenshots, and used text large models to generate HTML+tailwind code
- Designed frontend interface using PyQT, implemented real-time display of generation results through websocket communication
- Created installation package using Inno Setup, wrote detailed project documentation and usage instructions

## Key Special Project: Classroom Behavior Dataset Construction
*2023.10 - 2024.06* - Core Team Member
- Constructing a high-quality large-scale dataset to explore behavior recognition in densely populated classroom settings;
- Finding data sources, developing annotation plans, organizing project teams, and forming project schedules
- Downloading classroom scene videos in bulk from the internet; manually screening videos with appropriate perspectives and segmenting video clips
- Organizing the annotation team and quality control team to check completed data labels

## Low-Resolution Scene Behavior Recognition
*2023.09 - 2024.06* - Core Team Member
- Developed a technical plan based on the YoLov5 object detection module and the slowfast-based behavior classification module;
- Preprocessed the large-scale AVA dataset, used OpenCV to batch extract and classify video frames, organized valid labels, and converted label formats using Python;
- Preprocessed the large-scale Kinetics-400 dataset, used FFmpeg to batch clip and scale videos, extracted valid video labels, completed the dataset format configuration required for the slowfast network, and distributed the training of slowfast on multiple GPUs using the processed dataset to obtain pretrained models;
- Proposed a dual-branch network based on the slowfast network to separate spatiotemporal features. The main branch uses lower frame rates to extract spatial information, while the auxiliary branch uses higher frame rates to extract temporal information. The information from both branches is fused bidirectionally through cross-attention;
- The proposed new network structure achieved 75.2% F1 score on public datasets and 83.41% accuracy on the newly proposed classroom behavior recognition dataset, surpassing the baseline model with only a 13.41% increase in inference cost.

## Fault-Tolerant Distributed Key-Value Storage System Based on Raft
*2023.11 - 2024.01* - Personal Project [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="20"/>](https://github.com/LinyuJupiter/Distributed-Raft)
- Implemented a fault-tolerant distributed key-value (KV) storage system using Go language, based on the project framework from MIT's 6.824 Distributed Systems course;
- Referenced the Raft-Extended paper to complete functionalities such as Raft Leader election and heartbeat, log replication and consistency, snapshot mechanism, and log compaction;
- Designed both the client and server sides, perfected functions like CRUD (Create, Read, Update, Delete), and integrated the database with the Raft algorithm;
- Developed a fault tolerance scheme and completed failure tests for scenarios such as node disconnection, RPC packet loss, and network partitioning;
- Conducted high-concurrency testing, and the system is capable of processing a large number of concurrent requests within the specified time.

## Apple Tree Leaf Disease Detection Based on Convolutional Neural Networks
*2023.10 - 2023.11* - Personal Project [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="20"/>](https://github.com/LinyuJupiter/Identify-the-category-of-foliar-diseases-in-apple-trees)
- Performed one-hot encoding on the dataset labels, transforming the multi-classification task into a multi-label classification task;
- Designed and trained neural network models using both the LeNet and VIT architectural frameworks, compared the performance of CrossEntropyLoss versus ArcFaceLoss in addressing fine-grained classification issues, and the final trained LeNet model achieved an accuracy rate of 89.5% on the test set.

## Vehicle Traffic Analysis System Based on YoLov8 and Tesseract-OCR
*2023.06 - 2023.07* - Personal Project [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="20"/>](https://github.com/LinyuJupiter/Traffic-Flow-Analysis-System)
- Trained a YoLo neural network model for vehicle type recognition and tested it on multiple road surveillance videos;
- Trained a Tesseract-OCR model for handwritten text recognition and applied it to license plate text recognition;
- Designed a vehicle traffic counting algorithm using Python, implemented object tracking with the BoT-SORT algorithm, and determined traffic flow through regional judgments;
- Developed the project UI using the tkinter library, added simple interactive controls and information display widgets, facilitating the expansion and application of the project.

## Automatic Pathfinding and Control Simulation for a Car Based on Simulink
*2023.06 - 2023.07* - Personal Project [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="20"/>](https://github.com/LinyuJupiter/Fundamentals-of-autopilot-project)
- Implemented path planning from start to finish using the A* algorithm on randomly generated 2D maps by the system;
- Designed scaling and interpolation strategies to optimize the generated feasible paths with Bezier curve interpolation and the De Casteljau algorithm, and smoothed the paths in segments to handle collision issues;
- Used MATLAB programming to solve for LQR parameters, calculated the ABQR matrices corresponding to the car's parameters, and established a k-value table for the LQR controller;
- Designed a PID controller for lateral control of the car and an LQR controller that integrates the car's lateral speed and path curvature for longitudinal control;
- Conducted path tracking simulations for the car using Simulink, established a controller simulation model, and successfully guided the car to the finish line in one attempt without collisions;
- Secured a top 3 finish in the MATLAB group (out of 35 participants) in a racing competition.

## C++ Implementation of a Two-Player Chinese Chess Game
*2022.11 - 2023.01* - Personal Project [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="20"/>](https://github.com/LinyuJupiter/Two-Player-Chinese-Chess-Game)
- Designed the program's underlying architecture, including base classes for chess pieces and the chessboard, a vector for piece states, and derived classes for 14 types of chess pieces. Stored piece viability using a vector-like class, and employed a move prediction and post-move validation strategy to ensure piece movement logic adhered to the rules;
- Utilized IO streams and a custom file format to save and load game progress, and added a detection mechanism to prevent unreasonable endgame situations;
- Designed the UI interface using QT Designer, added custom controls, and created an installer package with Visual Studio. The project achieved first place in the class (out of 47 students).

# 🎖 Honors and Awards
- *2024.07* Second Prize in Hebei Province for the "Challenge Cup" China College Student Entrepreneurship Competition
- *2024.02* Mathematical Contest in Modeling(MCM/ICM)
- *2023.03* Third Prize in the First "Intelligent Data Cup" Data Analysis Competition of the School of Intelligent Engineering in 2023

# 📖 Educations
- *2025.09 - Present*, Master's Degree: The Chinese University of Hong Kong, Faculty of Engineering, Department of Information Engineering, Hong Kong
- *2021.09 - 2025.06*, Bachelor's Degree: Sun Yat-sen University, School of Intelligent Engineering, Intelligent Science and Technology, Shenzhen
- *2018.09 - 2021.06*, High School: Heyuan Middle School, Heyuan

# 📝 Publications 
- *2025.04* [Chen, R., Gao, C., Tan, Z., Liu, F., Yu, J., & Li, X. (2025). Dual-branch vision transformer for low-resolution action recognition. Multimedia Tools and Applications, 1-20.](https://link.springer.com/article/10.1007/s11042-025-20827-w)
- *2024.06* Computer Software Copyright - CellMaster Teaching System

# 💻 Internships
## *2024.07 - Present*, [Tencent Technology (Shenzhen) Co., Ltd.](https://www.tencent.com/zh-cn/index.html), Test Development Engineer, Shenzhen
- Responsible for developing automated test case generation tools that use large model-based Agent workflows to generate corresponding test scenario code based on call logs and other information
- Designed log parsing solutions and wrote algorithms to extract valid interface information from complex interface call logs
- Used a multi-path matching solution combining matching algorithms and the Hunyuan large model to trace the source of various interface request body parameters
- Designed prompts using Few-shot-Cot method based on the Hunyuan large model and vector indexing service, providing interface information and a small amount of code templates to enable the large model to output test case code
- Parsed database table records, used multi-path matching solutions to trace the source of database fields, thereby implementing result checking for test processes
- Completed the overall system design, split tasks and built decoupled modules, connected the entire process and finally implemented a complete system

## *2024.01 - 2024.02*, [Guang Dong Fenghua Advanced Technology (Holding) Co.,Ltd.](https://www.china-fenghua.com/), Artificial Intelligence Engineer, Zhaoqing
- Developed an intelligent order report management program to batch process company order warehousing efficiently
- Based on open-source large models such as chatGLM-6b and qwen-7b, used company documents to develop, train, and deploy the Fenghua Artificial Intelligence document large model
- Organized the company's material database, used embedding models and reranker models to establish a material knowledge base, and developed an intelligent material information customer service application in conjunction with the large model
- Developed the backend interfaces for the company's procurement material platform and completed the database integration work

## *2023.07 - 2023.08*, Guangdong Wanshida Intelligent Technology Co., Ltd, Software Development Intern, Heyuan
- Delved into the smart platform project for the decoration industry, independently developing a one-stop platform software for the client company based on Python and MySQL
- Matched technical solutions to customer needs, set up an anaconda virtual environment, and designed the software's underlying architecture to enable features such as chat and shopping modules
- Built a MySQL database to facilitate frontend-backend interaction, designed a graphical interface for the frontend, and completed the design and writing of interfaces by encapsulating SQL statements in the backend
- Utilized the tkinter library to design the software's UI interface and interaction logic according to requirements, used the ttkbootstrap library to beautify the interface and make it adaptable to multi-resolution windows
- Created an installation package with Inno Setup and wrote project documentation and usage instructions
