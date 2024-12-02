---
title: Requirements
has_children: false
nav_order: 3
---

# Requirements

# Requirements


## Goals

The goal of **Sixpack** is to provide an easy-to-use app where users can autonomously manage their training routines by selecting exercises tailored to their needs.


## Functional Requirements

### 1. User Authentication

**Requirement:** Users must be able to create a profile and log in to the application.

**Acceptance Criteria:**
- Users can create an account using an email and password.
- After creating an account, users can log in using their email and password to access the app's functionalities.
- On successful login, users are redirected to the home page where they can start creating their training plans.

### 2. Creation of a Training Session and Customization

**Requirement:** Users must be able to create personalized training sessions and add as many exercises as they want by interacting with a simple interface.

**Acceptance Criteria:**
- Users can start a new session by clicking on "New Training Session."
- A page appears, allowing users to add exercises, define the number of reps, sets, and rest intervals.
- Once saved, the session is displayed on the user’s main dashboard.

### 3. Multimedia Integration

**Requirement:** Users must be able to add image or video links to exercises for instructional purposes.

**Acceptance Criteria:**
- Users can insert a link to a video or image as part of each exercise.
- The app displays the visuals next to the exercise in the training session view.
- When clicked, the media opens in an external player or browser (an internet connection is required).

### 4. Session Management

**Requirement:** Users must be able to save, edit, or delete their training sessions.

**Acceptance Criteria:**
- Users can view saved sessions on their dashboard.
- Sessions can be edited by selecting "Edit," allowing changes to exercises, reps, sets, and rest periods.
- Users can delete a session by selecting "Delete," with a confirmation prompt displayed before deletion.


## Non-Functional Requirements

### 1. Usability

**Requirement:** The application must be easy to navigate, enabling users to complete tasks with minimal clicks and in a short time span.

**Acceptance Criteria:**
- Any function (adding, editing, deleting exercises) is accessible within three clicks.
- Buttons and icons are clearly labeled with intuitive visuals.

### 2. Performance

**Requirement:** The app should load each screen and execute actions (saving, editing, deleting sessions) with minimal delay.

**Acceptance Criteria:**
- Pages and actions load and execute within two seconds under standard network conditions.
- Video and image previews load within one second.

### 3. Security

**Requirement:** User data must be securely stored and protected, with all data transfers encrypted.

**Acceptance Criteria:**
- User passwords and sensitive data are encrypted before storage.
- The app uses HTTPS for secure data transmission.
- Access to the app requires login after inactivity or logout, protecting user information.

### 4. Device Compatibility

**Requirement:** The application should be compatible with modern iOS and Android devices.

**Acceptance Criteria:**
- The app works seamlessly on devices running iOS 13.0+ and Android 9.0+.
- Screens are responsive and adapt to different device sizes.

### 5. Data Synchronization

**Requirement:** Data should sync perfectly across devices for users logged into the same account.

**Acceptance Criteria:**
- Changes made to training plans are synced across devices within seconds.
- Synchronization occurs in the background without impacting the app's overall performance.


## Implementation Requirements

### 1. Programming Language & Frameworks

**Requirement:** The application should use modern frameworks compatible with both mobile and desktop environments.

**Acceptance Criteria:**
- The front-end is implemented using HTML, CSS, and JavaScript for flexibility and responsiveness.
- Backend services are developed using Python with the Flask framework.

### 2. Database Management

**Requirement:** User and training session data must be stored in a database system for effective management.

**Acceptance Criteria:**
- The database allows for seamless storage and retrieval of user data and training plans.
- Data structures are optimized for scalability and performance.
