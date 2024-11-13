---
title: CI/CD
has_children: false
nav_order: 9
---

---

# CI/CD

- This section provides a conceptual description of the CI/CD workflow
    - What is how automated?
    - Why?
- Relevant details of GitHub Actions exploitation / implementation


The application Six-Pack backend is based on FastAPI, and the frontend uses Vue.js. The CI/CD process must reflect this.
Tailor the testing and deployment processes to align with the project's specific requirements, while maintaining automated testing, building, and deploying.

---

# CI/CD Strategy for "Six Pack" Application

The CI/CD (Continuous Integration / Continuous Deployment) process is an essential practice in modern software development, enabling the automation of testing, building, and deploying applications. 
For the Six Pack application, which consists of a FastAPI backend and a Vue.js frontend, the CI/CD pipeline ensures that the codebase is always in a deployable state. Through automated processes, we can continuously integrate code changes and deploy them efficiently, preventing potential errors and enabling faster releases: the CI/CD strategy for the Six Pack application, outlining how both the backend and frontend are integrated, built, tested, and deployed.

# Why implement CI/CD?

The adoption of a CI/CD pipeline for the Six Pack project offers several key advantages:

- Shorter Development Cycles: Automating key processes such as testing and deployment accelerates development, allowing features to be released quicker.
- Increased Efficiency: By eliminating manual intervention in the build and deployment processes, development time is optimized.
- Reliability: With every code change automatically tested, the risk of introducing errors is minimized, ensuring higher quality in production.
- Faster Time-to-Market: Automation reduces the delay between code submission and production deployment, which accelerates feature delivery to users.

This results in both reduced development costs and enhanced developer satisfaction as more time can be spent on feature development rather than routine tasks.

# Backend procedure (FastAPI)
How we managed to structure our job for Backend (FastAPI) and the steps are the following:
1. Python Environment: Sets up Python (compatible with FastAPI)
2. Dependencies: Poetry manages dependencies
3. Testing: Runs backend tests using pytest.
Let's now talk about Build and Deploy procedure. The FastAPI backend is built, deployed to TestPyPI, and a GitHub release is created.

# Job Structure for Frontend (Vue.js)

1. Node.js Environment: Set up for Vue.js.
2. Dependencies: Uses npm for package management.
3. Testing: Runs frontend tests.
4. Build: Builds the Vue.js frontend application.

We created a file which is a GitHub Actions workflow configuration written in YAML, designed for automated deployment of an application. Let us break it down of its purpose and key steps:

# Main Purpose:

The main purpose is to automatically build and deploy the application whenever a new commit is pushed to the main branch of the repository. The deployment process involves:

1. Checking out the code
2. Installing dependencies
3. Building the application.
4. Deploying the built app to GitHub Pages
   Key Steps:
5. Trigger (on: push):
   The workflow is triggered on a push to the main branch.This means that whenever someone pushes new changes to the main branch, the workflow will start running
6. Job (jobs: build):
   The job is named “Build” and runs on the latest version of Ubuntu (ubuntu-latest)
   Steps:
   Checkout the repository (uses: actions/checkout@v3): This pulls the repository’s code into the runner.Set up Node.js (uses: actions/setup-node@v2): It sets up Node.js version 16. The token (GH_TOKEN) is included to allow access to private packages if necessary.

- Install dependencies (run: yarn): Installs all necessary dependencies using Yarn.
- Build the app (run: yarn build): Executes the build command, usually compiling code or bundling assets.
- Deploy to GitHub Pages (uses: JamesIves/github-pages-deploy-action@v4.2.5):
- The deployment action uploads the built application to the GitHub Pages branch (branch: github-pages).
- The folder out contains the output files (HTML, CSS, JS, etc.) that will be deployed to GitHub Pages.
  Why we should imply ci/cd?
The benefits of ci/cd:

- Shorter cycle time
- Happier employees
- Gets to market faster: codes run in the pipeline and now in production is just making the money


This updated CI/CD pipeline is customized for the "Six Pack" application, ensuring that both the FastAPI backend and Vue.js frontend are tested, built, and deployed seamlessly.
This updated CI/CD pipeline is tailored specifically for the "Six Pack" application, which helps users organize their workout sessions by specifying daily exercises, the number of series, and reps. The pipeline ensures that both the FastAPI backend and the Vue.js frontend are consistently tested, built, and deployed seamlessly.

For "Six Pack," the backend will handle user registration, session management, and exercise tracking. The frontend provides an intuitive interface where users can add and modify sessions and exercises, aligned with their fitness goals. The integration of a timer and the potential use of Tkinter for images/videos makes the application interactive and engaging.

This CI/CD approach guarantees reliable deployments and smooth updates, ensuring that the features supporting user interaction—like adding/modifying workouts—are always functional.
