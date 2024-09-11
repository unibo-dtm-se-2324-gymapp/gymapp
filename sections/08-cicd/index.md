---
title: CI/CD
has_children: false
nav_order: 9
---

# CI/CD

- This section provides a conceptual description of the CI/CD workflow
    - What is how automated?
    - Why?
- Relevant details of GitHub Actions exploitation / implementation


The application Six-Pack backend is based on FastAPI, and the frontend uses Vue.js. The CI/CD process must reflect this.
Tailor the testing and deployment processes to align with the project's specific requirements, while maintaining automated testing, building, and deploying.

# CI/CD Strategy for "Six Pack" Application

CI/CD Overview:

The CI/CD pipeline automates testing, building, and deployment processes to ensure that the "Six Pack" frontend and backend are always in a deployable state. Automated checks prevent issues and ensure smooth updates.

Setting Up CI/CD with GitHub Actions
CI/CD Pipeline Configuration

Workflow Definition:
The pipeline uses GitHub Actions and is defined in the .github/workflows directory of both the frontend and backend repositories. The backend is built with FastAPI, and the frontend uses Vue.js.

Workflow Triggers:

The CI/CD workflow is triggered by events like pushes to the main branch and pull requests targeting the main branch.

Job Structure for Backend (FastAPI)
...

Python Environment: Sets up Python (compatible with FastAPI).
Dependencies: Poetry manages dependencies.
Testing: Runs backend tests using pytest.
...

Build and Deploy: The FastAPI backend is built, deployed to TestPyPI, and a GitHub release is created.

Job Structure for Frontend (Vue.js)
...

Node.js Environment: Set up for Vue.js.
Dependencies: Uses npm for package management.
Testing: Runs frontend tests.
Build: Builds the Vue.js frontend application.
...

This updated CI/CD pipeline is customized for the "Six Pack" application, ensuring that both the FastAPI backend and Vue.js frontend are tested, built, and deployed seamlessly.
