<h1> Six-pack</h1>
Sixpack is a web application built with Flask that allows users to register, login, create personalized training sessions with exercises that can be tailored to the user needs.

<h3>Features</h3>
<h5>User Authentication</h5>
User registration and login system
<h5>Training sessions</h5>
Browse available gym classes with descriptions and slots
<h5>Personalized Training Sessions</h5>
Create custom training sessions
Add exercises to sessions, specifying sets and reps

<h3>Requirements</h3>
Before running the application, make sure you have the following installed:

Python 3.7+
Pip (Python package manager)
<h3>Installation</h3>

<h5>Clone the Repository</h5>
git clone + link of the repository on github

<h5>Create a Virtual Environment</h5>

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
<h5>Install Dependencies</h5>

pip install -r requirements.txt
<h5>Run the Application</h5>

python Sixpack.py
<h5>Access the Application</h5>

Open your browser and navigate to:
In the terminal, there must be a link like the one below, click on it and the website should appear.
http://127.0.0.1:5000


<h3>Usage</h3>
<h5>Register an Account</h5>
We put some basic security measures like the compulsory presence of the @ in the mail but further improvements could be made on the password
<h5>Log In</h5>

Log in to your account to access features.
<h5>View Training sessions</h5>
If it is your first time on Sixpack, you will see just empty tables to be filled with exercise
<h5>Create exercises</h5>
Add exercises to your session by specifying exercise names, sets, and reps.

<h3>Technologies Used</h3>
Backend: Python
Frontend: HTML, CSS and JS
Database: In-memory Python structures (extendable to SQL with Flask-SQLAlchemy)
<h3>Future Enhancements</h3>
Add a database (e.g., SQLite, PostgreSQL) for persistent data storage.
Implement advanced user authentication (e.g., password hashing with Flask-Bcrypt).
Add a user dashboard to track progress over time.
Integrate class booking with calendars.
Enhance styling with Bootstrap or TailwindCSS.
<h3>Contributing</h3>
Contributions are welcome! If you find bugs or have suggestions, please open an issue or submit a pull request.

<h3>License</h3>
This project is licensed by using the Standard Semantic versioning.

<h3>Contact</h3>
For questions or feedback, feel free to reach out:

Name: Alessandro Astolfi, Marta Betti,Domenico Bonifazio, Klaudia Daci e Leilei Zhang
Email: alessandro.astolfi@studio.unibo.it,marta.betti5@studio.unibo.it,domenico.bonifazio@studio.unibo.it,klaudia.daci@studio.unibo.it,leilei.zhang@studio.unibo.it
