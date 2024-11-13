---
title: Deployment
has_children: false
nav_order: 8
---

# Deployment
- This section explains what operations are needed to make the software work on the users' machine(s)

The deployment of the Six-pack application requires some foundamental steps and the configuration of some elements, before users can use it.
We used:
-Backend: Flask (Python)
-Frontend: HTML, JS, CSS
-Database: 
-Server: Python

System requirements for the application:
-Python 3.8 or later
-Git
-Visualstudiocode
-Flask
-Flask cors

Prerequisites:
Before getting started, make sure you have the following tools installed:
-Python 3.x: This application requires Python 3.x. You can download the latest version of Python from the official Python website.
-pip: Python should come with pip, the package manager. If it’s not already installed you should install it by following the instructions you find in https://pip.pypa.io/en/stable/installation/



1-step
The first step is to clone the repository settled in github with the command 'git clone https://github.com/unibo-dtm-se-2324-gymapp/gymapp.git' and then access it.

2-step
Create a virtual environment, by following these instructions:(optional but recommended):
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

3-step
You need to install Flask and Flask Cors if are not present in your device. You can do it by installing the file Requirements.txt that is in the application's folder.

-Running the application:
To start the gymapp application run the command "python Sixpack.py"

At this point the application will be running in debug mode and will be accessible via your browser at http://127.0.0.1:5000/.

-Troubleshooting:
Error: ModuleNotFoundError: If you encounter an error indicating that a module is not found, make sure you have correctly run the command pip install -r requirements.txt.
Port 5000 already in use: If port 5000 is already in use, you can run the application on a different port by modifying the last line of the app.py file: app.run(debug=True, port=5001)



