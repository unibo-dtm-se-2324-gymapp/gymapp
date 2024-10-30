---
title: Concept
has_children: false
nav_order: 2
---

<h1>Six-pack Application Overview</h1>
<p>Six-pack is a web-based application designed to help users manage their personal fitness and routines efficiently. The goal of the app is to help people organize their training sessions by allowing them to select exercises and personalize their workout details (e.g., reps, series, duration) with added visuals (images/videos) to ensure proper form. It offers features like account creation, training tracking, and week-based planning to support users’ fitness journeys.</p>

<h3>Key Characteristics of the Product</h3>
<ul>
    <li><strong>Application:</strong> Web-based, accessible on all modern browsers with a dedicated URL; a desktop version is planned for future development.</li>
    <li><strong>User Interface:</strong> Simple, clean, and user-friendly GUI to facilitate efficient access to training and profile management features.</li>
    <li><strong>Functionality:</strong> Core features include user registration, login, training session management (from Monday to Sunday), profile updates, and access to historical records.</li>
</ul>

<h3>Features and Use Case Collection</h3>

<h4>Use Case 1: Account Registration</h4>
<ul>
    <li><b>Actor:</b> Non-registered user</li>
    <li><b>Goal:</b> First-time users register for access to platform features</li>
    <li><b>Flow of Procedures:</b>
        <ol>
            <li>User clicks on the "Register" button.</li>
            <li>User inputs email and password.</li>
            <li>System registers the account, allowing the user to start personalizing training sessions.</li>
        </ol>
    </li>
</ul>

<h4>Use Case 2: Profile Information Update</h4>
<ul>
    <li><b>Actor:</b> Logged-in user</li>
    <li><b>Goal:</b> View or edit profile details (e.g., username, email, age, gender)</li>
    <li><b>Basic Flow:</b>
        <ol>
            <li>User navigates to the profile page by selecting the "Profile" button on the home page.</li>
            <li>Profile page displays user's personal details (e.g., username, email).</li>
            <li>User edits their information (e.g., updates email, age, gender, job title, etc.).</li>
            <li>System updates the profile data in the database.</li>
        </ol>
    </li>
</ul>

<h4>Use Case 3: Exercise Modification</h4>
<ul>
    <li><b>Actor:</b> Logged-in user</li>
    <li><b>Goal:</b> Modify exercise details to align with personal fitness objectives</li>
    <li><b>Basic Flow:</b>
        <ol>
            <li>User accesses their training session by selecting a day from the weekly planner.</li>
            <li>User selects an exercise to modify.</li>
            <li>User edits the exercise:
                <ul>
                    <li>Change exercise name</li>
                    <li>Adjust repetitions and duration</li>
                    <li>Select target body part, prompting the system to suggest suitable exercises</li>
                </ul>
            </li>
            <li>User saves changes; the system updates the data in the database.</li>
        </ol>
    </li>
</ul>

<h4>Use Case 4: Linking Images and Videos</h4>
<ul>
    <li><b>Actor:</b> Logged-in user</li>
    <li><b>Goal:</b> Attach tutorial images or videos to an exercise to ensure proper technique</li>
    <li><b>Basic Flow:</b>
        <ol>
            <li>User accesses a training session and selects an exercise.</li>
            <li>User links an image or video tutorial.</li>
            <li>User previews and confirms the media attachment.</li>
            <li>System displays the linked tutorial for reference during workouts.</li>
        </ol>
    </li>
</ul>
<h4>User stories</h4>
<p>
    <ul>
        <li>As a potential fitness enthusiast, I want create my account and subscribe to the app; so that I can start to plan my training session and personalize the exercises, so that i can have a routine that suits my fitness goals. </li>
        <li>As a fitness beginner, I want to view video or image demonstrations for each exercise as instructions, so that I can perform them safely and effectively.</li>
        <li>As a busy worker, I want to save and load my workout sessions quickly, so that I can fit my training into my daily working schedule.</li>
        <li>As an experienced athlete, I want to customize the sets, reps, and rest times, so that my workouts are aligned with my training level.</li>
        <li>As a user, I want to log in and save my training data, so that I can access my workouts across multiple devices.
</li>
        <li>As a user, i want to save as many training sessions as possible, decide the number of series of the same exercises, how many reps so that i can get fit in a proper way.  </li></ul>
</p>

