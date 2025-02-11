---
title: Validation
has_children: false
nav_order: 6
---

# Validation

## Testing


### Test Overview

This section details the testing approach for the Sixpack application, focusing on essential features like user registration, login persistence, data management, and interface usability. These acceptance tests are theoretical but structured to validate key functions according to the acceptance criteria.

### Test development process

The acceptance tests are based on Test-Driven Development (TDD) principles, simulating real-world scenarios to verify that each feature meets specific acceptance criteria.

    - Success Rate: Each test is designed to achieve a 100% success rate.
    - Coverage: These tests cover user registration, login, workout session management, and responsiveness.
    - Acceptance Criteria Validation: Each test is mapped to acceptance criteria, ensuring requirements are met.

### Acceptance test Cases and criteria

#### 1. User registration

- *Acceptance Criteria:*
    The user should only be able to register if they provide a unique email, a valid username, and a password meeting minimum security requirements.
    An error message should display if any required input is invalid.
    A confirmation message should be shown upon successful registration.

- *Acceptance Test:*
    Test with valid inputs to verify successful registration and confirmation message.
    Attempt to register with an existing email to check that an error message appears.
    Test input with weak passwords and invalid emails to confirm appropriate validation.

#### 2. User login persistence

- *Acceptance Criteria:*
    Once logged in, the user should stay authenticated across sessions (even after refreshing the page).
    Users should be redirected to the login page if not authenticated.

- *Acceptance Test:*
    Log in and refresh the page to verify that the session persists.
    Log out and attempt to access a protected page to confirm redirection to the login page.


#### 3. Workout session duplication and storage

- *Acceptance Criteria:*
    Users can add multiple workout sessions, with each session saved and retrievable.
    Each new session must duplicate correctly without affecting existing data.

- *Acceptance Test:*
    Duplicate an existing workout session and verify that both instances are saved and retrievable.
    Modify one session and check that changes do not affect the duplicated session.

#### 4. Workout data reset functionality
- *Acceptance Criteria:*
    Users can clear all workout session data using a reset function.
    Confirmation of data clearance should be displayed.

- *Acceptance Test:*
    Populate workout sessions, use the reset button, and confirm data is cleared.
    Check for confirmation message and verify the session data is empty.

#### 5. Profile information retrieval
- *Acceptance Criteria:*
    Profile data, including username and email, must display accurately upon login.

- *Acceptance Test:*
    Log in and access the profile page to verify that user information is correctly retrieved and displayed.

#### 6. User interface responsiveness
- *Acceptance Criteria:*
    The interface must adapt to various screen sizes (e.g., mobile, tablet, desktop).
    Text, buttons, and layout should be accessible and readable across devices.

- *Acceptance Test:*
    Test on multiple devices and resolutions to confirm UI adaptability.
    Verify that all buttons and text are accessible and readable on different screens.

#### 7. Error handling in workout data storage
- *Acceptance Criteria:*
    Users should be notified if data saving fails due to issues like network errors.
    A retry option should be available without losing previously entered data.

- *Acceptance Test:*
    Simulate a network failure during a data save and check for an error message.
    Ensure the retry function works, allowing data to be saved once the network is restored.