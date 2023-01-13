

# 1 - User viewing page( /Users)

## 1.1 - Introduction
This document outlines the user interface specifications for the user management screen of the system. The user management screen allows system administrators to manage and maintain user accounts within the system. This document will be used by software developers to guide the development of the user interface.

## 1.2 - User Interface Elements

- User Table: The main section of the screen will display a table of all registered users, including their username, email address, and status (active or inactive).
- Add User Button: Admins can add new users on new user page by clicking the "Add User" button.
- Add Dropdown for Status: The User Management Screen should have a drop-down filter to filter the list of users by their status(active, inactive).


## 1.3 - UI Behavior
- When the user management screen is first loaded, it should display a table of all registered users, sorted alphabetically by username.
- When the "Add User" button is clicked, a modal window should appear where the admin can enter the new user's information, including username, email address, and password. The modal should have validation on the fields, so that the user could not submit if any of the fields is empty.

## 1.4 - Error Handling
- If a user is searched for but not found, the table should display a message indicating that no matching users were found.
- If the admin attempts to add a new user with an email address or username that already exists in the system, an error message should appear and the form should be cleared.
- If the admin attempts to delete a user who is currently assigned to a role or group, the system should display an error message and prevent the deletion.

## 1.5 - Additional Considerations
-    The User Page should be responsive and accessible on all devices.
- Delete User Button: Admins can delete an existing user by clicking the "Delete" button next to the corresponding user in the table. (_it was not in illustration but I think that can be usefull_)
- - When the "Delete" button is clicked for a specific user, a prompt should appear to confirm the action before the user is permanently removed from the system.
- Search Bar: Users can search for specific users by entering a username or email address into the search bar. (_it was not in illustration but I think that can be usefull_)
- - When a user is searched for, the table should automatically filter to display only the matching user(s).
- Navigation Bar: The navigation bar at the top of the screen will provide access to the various sections of the system, including the user management screen. (_it was not in illustration but I think that can be usefull_)

# 2 - New user page( /New-User)

## 2.1 - Introduction
This document outlines the user interface specifications for the adding new user screen of the system. The user management screen allows system administrators to manage and maintain user accounts within the system. This document will be used by software developers to guide the development of the user interface.

## 2.2 - User Interface Elements
- Form: The main section of the screen will include a form to enter the new user's information, including username, email address, password, role, status (active or inactive)
- - "Username" Input Area 
- - "Display Name" Input Area
- - "Phone" Input Area 
- - "Email" Input Area 
- - "User Roles" Select List 
- - "Status" Dropdown 
- Submit button: Admins can submit the form to create the new user by clicking the "Submit" button.

## 2.3 - UI Behavior
-    When the new user page is first loaded, the form should be empty, ready to be filled out.
-    When the form is submitted, the system should validate the form fields, the form should not be submitted if any of the fields is empty.

## 2.4 - Error Handling
-    If the admin attempts to add a new user with an email address or username that already exists in the system, an error message should appear and the form should not be submitted.
-    If the admin attempts to submit the form without filling out all the required fields, an error message should appear next to each empty field.
-    If the username, email, phone fields are unique, it should give a warning when trying to register a user with the same informations.

## 2.5 - Additional Considerations
-    The New User Page should be accessible only by authorized users with admin roles.
-    The New User Page should be responsive and accessible on all devices.
-    The New User page should include a password strength indicator to help the admin to set a strong password.

