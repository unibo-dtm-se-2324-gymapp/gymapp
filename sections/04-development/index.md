---
title: Development
has_children: false
nav_order: 5
---

# Development

### Use of DVCS

The code was developed using a Distributed Version Control System (DVCS) that is Git. This allowed to track changes in the in the repository in a collaborative and granular way by following some fundamental conventions:

- *Branching Conventions:*  
  The project followed a branch-based workflow inspired by Git Flow. A main branch (main) is used for stable, production-ready code and repository, instead new development and features are implemented using secondary branches ( like "Domenico Branch" ), which once completed, are merged into the main branch, after a code review.

- *Conventions for commits:*  
  Commits were made following a clear and descriptive convention for commit messages, crucial for maintaining a clean history of changes. Each commit includes a simple and easy to understand message explaining the change made, for example: "user guide updated".

- *Any other relevant aspect:*  
The use of git, together with the conventions already provided, allowed us to work separately, basing on the skills of each person, avoiding conflicts between the different phases of the project. 
Once we reached the final phase of the project, we reviewed the individual parts together, trying to evaluate the work done by each member of the team.

### Implementation Details

- *New and relevant learnings:*  
  During the development of this code, we adopted  Flask with CORS, that is a security mechanism that allows resources (such as APIs) to be requested from a domain different from the one where the server responded, making it more versatile and ready for distributed web application. In particular we used allow to link back end and front that were developed separately.
  Additionally, working with the Flask-CORS extension helped solidify the understanding of securing APIs in a cross-domain environment, preparing the project for a broader deployment context.


- *A class of which you are particularly proud:*  
  
The User class is the one that we want to highlight, even though its current implementation is quite simple. This class represents a good starting point for new features implementation within the application. At the moment, the User class includes fundamental attributes like user_id, name, and password, which are essential for identifying and authenticating a user within the system.

 The object-oriented design in Python allows for easy expansion of the class with new attributes and methods that could handle more advanced aspects of user management. For instance, it could be enriched with features for session management, such as tracking the last login and supporting two-factor authentication. 

It is an example of how thoughtful and forward-looking design can facilitate the growth and evolution of a software project.

### Development Description

The code is a simple Flask API that allows saving and loading user session data in memory. It is structured to be extensible and easy to maintain. It relies on in-memory data management for demonstration purposes but can easily be adapted to use a persistent database in a production context. 

### Architecture Overview

The architecture of the code was designed with modularity, allowing new features to be added easily without compromising the existing structure.
 The frontend is developed using HTML, CSS, and JavaScript, which interact with the backend through well-defined API endpoints. The backend is built with Flask, providing endpoints for user management and session handling. The in-memory data handling approach demonstrates the core logic, while the backend is flexible enough to support integration with a database system like MySQL or MongoDB in the future.

By separating concerns between the frontend and backend and employing Flask’s modular structure, the project remains scalable and easy to extend, accommodating new features or changes with minimal disruption to the existing codebase.
