---
title: Home
layout: home
has_children: false
nav_order: 1
---

# Project title

### Authors
- [Domenico Bonifazio]
(mailto: domenico.bonifazio@studio.unibo.it)
- [Alessandro Astolfi]
(mailto: alessandro.astolfi@studio.unibo.it)
- [Marta Betti]
(mailto: marta.betti5@studio.unibo.it)
- [Leilei Zhang]
(mailto: leilei.zhang@studio.unibo.it)
- [Klaudia Daci]
(mailto: klaudia.daci@studio.unibo.it)

## Introduction
This group is composed by all students with a background in business and management, 
So this was the fist time that we approached the developement of a software. 
The main idea was to create a tool that supports athletes and fitness enthusiasts, including those involved in bodybuilding and similar disciplines, in tracking, managing, and customizing their workouts independently. 
Furthermore, the tool allows users to design personalized training programs without being constrained by pre-selected exercise databases or the need to subscribe to premium versions. 

## Abstract

This project was conceived with the goal of developing a web application fully adaptable to all devices, making it responsive. 
In the future, the aim is to create a mobile application to ensure even easier and more immediate access. 
Our software’s primary objective is to enable users to independently manage their workouts by creating personalized weekly schedules. 
The application has been designed to provide simple and intuitive navigation, making it user-friendly, and offering users, after registration, the perfect tool for managing their training routines.

From the **client side**, users can perform diffent tasks:
- **Registration** The first step is the creation of a new user profile.
- **Home page access** After the access, the user will be redirected to the home page.
- **Training sessions access** Through the hompage the user can access to the training section that is weekly slint into days.
- **Workout planning** The user can access to each day of the week, and create, manage and save workouts. 
- **Add exercises** The user can add and remove exercises for each workout plan, naming the exercise, setting the number of sets, the number of repetitions and rest time.

In the **server side**, we decided to use the **Flask** to manage the communication between the backend and frontend. The Flask APIs allow saving and loading user session data in memory.
**Flask_cors** is used as security mechanism that allows resources (such as APIs) to be requested from a domain different from the one where the server responded, making it more versatile and ready for distributed web application.
Thanks to flask library, we were able to link the beckend and the frontend, that were developed separately.

The application is designed to rely on in-memory data management for demonstration purposes but can easily be adapted to use a persistent database in a production context.
In fact we tried to develop the applicatio with a modular approach, allowing new features to be added easily without compromising the existing structure.
Thanks to this the backend is flexible enough to support integration with a database system like MySQL or MongoDB in the future.

Finally, we can consider our software a goood start point to develop a more complex tool to manage workout sessions. Thanks to some future improvements, like a digital timer, multimedia integration or 
the integration with IoT devices (smartwatch and smartring), we belive this software can be a functional tool for every athlete and fitness enthusiast.
















