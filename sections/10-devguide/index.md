<h1>Development guide</h1>

This section explains how to use the software (from a developer perspective)
For example, how to use the software API to build more software
Here is a detailed description of the APIs and routes defined in the this code. Each endpoint, its purpose, the HTTP methods supported, and how to interact with them are described in the following text.

Home Page (/) Route: / Methods: GET Description: It redirects to the login page (/loginpage), if a user is not logged in. Otherwise, it redirects it to the home page (/homepage) on logging into the account. Behavior: The program examines for the cookie (user_id). If one is present and fits into the user_data, a user is directed to the homepage. Otherwise, to the login page.

Login Page (/loginpage) Route: /loginpage Methods: GET, POST Description: Operates with the login form (GET request) and accuracy of the supplied login information (POST request). When user views a form (POST request), the system evaluates the credentials in the database. If found correct, then user is cookie noted as online as “user_id” and directed to their homepage. If the user is not yet a member of the system or provided the wrong access passwords for the system, and error will emerge. Form Parameters (POST): email: please put the retrieved email into this our form for the user. password: The retrieved password will go into the password field of the user form.

Register Page (/register) Route: /register Methods: GET, POST Description: Shows the registration form (GET request) and processes the registration operation taken by the user (As in the POST method). After that, the application checks if the passwords match and if the email is already in use when the form is posted. If all is well, the user_information table is updated with the new user and redirects user to the home page and also set a cookie for the user_id. Form Parameters (POST): username: please put the appropriate name in this perimeter of the user. email: please put the email address of the user in the email field. password: the password of the new user on this form should be entered here. confirm-password: an exact copy of the password to enable confirmation is entered here.

Home Page (Logged In) (/homepage) Route: /homepage Methods: GET Description: Shows that a user is logged in and displays the user's home page for this situation. Otherwise, to the login page.

Profile Page (/profile) Route: /profile Methods: GET Description: Shows the details of the user profile. If the user tried to access his/her profile but he/she was not logged-in, redirected to the login page.

Logout (/logout) Route: /logout Methods: GET Description: Logs the user out by removing the user_id cookie and redirects him to