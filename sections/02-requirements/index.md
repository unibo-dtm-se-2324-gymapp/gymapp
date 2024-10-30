---
title: Requirements
has_children: false
nav_order: 3
---

# Requirements

<h3>Goals</h3>
The goal of Six-pack is to provide an easy-to-use app where users can manage autonomously their training routine by deciding which exercises to do according to their needs.

<h3>Functional Requirements</h3>
<h4>1.User Authentication</h4>
<p>Requirement: Users must be able to create a profile and log in to the application.</p>
<h7>Acceptance Criteria:</h7>
<ul>
    <li>Users can create an account using an email and password.</li>
    <li>After creating an account, users can use their email and password to log in and access to our app functionalities.</li>
    <li>On successful login, users are directed to the home page where they can start creating their training plans.</li>
</ul>

<h4>2.Creation of a training session and customization </h4>
<p>Requirement: Users must be able to create a personalized training session and insert as many exercises as they want by simply pushing a few buttons.</p>
<h7>Acceptance Criteria:</h7>
<ul>
    <li>Users can start a new session by clicking on “New Training Session.”</li>
    <li>A page shows up, allowing users to add exercises, select the number of reps, sets, and rest intervals.</li>
    <li>Once saved, the session appears on the user’s main dashboard.</li>
</ul>

<h4>3.Multimedia Integration</h4>
<p>Requirement:Users must be able to add image or video links to exercises for instructional purposes.</p>

<h7>Acceptance Criteria:</h7>

<ul>
    <li>Users can insert a link to a video or image as part of each exercise.</li>
    <li>The app displays these visuals next to the exercise in the training session view.</li>
    <li>When clicked, the media opens in an external player or browser. Internet connection is needed</li>
</ul>

<h4>4.Session Management</h4>
<p>Requirement: Users can save, edit, or delete their training sessions.</p>

<h7>Acceptance Criteria:</h7>

<ul>
    <li>Users can view saved sessions on their dashboard.</li>
    <li>Each session can be edited by selecting an “Edit” option, allowing modifications to exercises, reps, sets, and rest periods.</li>
    <li>Users can delete a session by selecting “Delete,” and a confirmation message appears.</li>
</ul>

<h3>Non-functional requirements</h3>

<h4>1.Usability</h4>
<p>Requirement: The application must be easy to navigate, allowing users to complete tasks with minimal clicks. Users can complete common tasks in a short time span.</p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>Any function (adding exercises, editing, deleting) must be accessible within 3 clicks.</li>
    <li>All buttons and icons are clearly labeled with intuitive visuals.</li>
</ul>

<h4>2.Performance</h4>
<p>Requirement: The app should load each screen and execute actions (saving, editing, deleting sessions) with minimal delay.</p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>Each page or action must load and execute within 2 seconds on standard network conditions.</li>
    <li>Video and image previews load without delays (within 1 second).</li>
</ul>
<h4>3.Security</h4>
<p>Requirement: User data must be securely stored and protected, with data transfers encrypted.</p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>User passwords and sensitive data are encrypted before storage.</li>
    <li>The app uses HTTPS for all data transmission to secure user interactions.</li>
    <li>Access to the app requires login after inactivity or logout, protecting user information.</li>

</ul>
<h4>4.Device Compatibility</h4>
<p>Requirement: The application should be able to run on recent IOS and Android devices. </p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>The app works well perfectly on devices running iOS 13.0+ and Android 9.0+.</li>
    <li>Screens are responsive and adapt to different sizes of devices.
</li>

</ul>

<h5>5.Data synchronization</h5>
<p>Requirement: Data should sync perfectly across devices for users logged into the same account.</p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>When a user makes changes, updates to the training plan on the device, the data syncs to other devices within a few seconds of the change. </li>
    <li>The syn occurs in the background without effecting the overal performance of the application. </li>
</ul>

<h3>Implementation requirements</h3>
<h4>1.Programming Language & Frameworks</h4>
<p>REQUIREMENTS: The application should be developed using a modern framework compatible with mobile and desktop environments.</p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>Frontend is implemented using HTML, CSS, and JavaScript for flexibility and responsiveness. </li>
    <li>Backend services are developed using Python with the Flask framework. </li>
</ul>

<h4>2.Database Management</h4>
<p>REQUIREMENTS: User and training session data must be stored in our own database system so we can have an easier data management. </p>
<h7>Acceptance Criteria:</h7>

<ul>
    <li>The database must be SQL-based  </li>
    <li>The data model should include user accounts, training sessions, exercises, and multimedia links. </li>
</ul>
