# DevOps Internship Task 1: CI/CD Pipeline for a Node.js App

## Overview 🚀

This project demonstrates a complete CI/CD (Continuous Integration/Continuous Deployment) pipeline using GitHub Actions. The goal is to automate the process of building a Docker image for a simple Node.js web application and pushing it to DockerHub.

The automation is triggered every time new code is pushed to the `main` branch of this repository.

## Technologies Used 🛠️

* **Application**: Node.js, Express.js
* **Containerization**: Docker
* **CI/CD**: GitHub Actions
* **Image Registry**: DockerHub

## CI/CD Workflow ⚙️

The automation pipeline is defined in the `.github/workflows/main.yml` file and consists of the following steps:

1.  **Trigger**: The workflow starts automatically on a `push` to the `main` branch.
2.  **Checkout**: The runner checks out the latest version of the repository's code.
3.  **Login to DockerHub**: It securely logs into DockerHub using credentials stored as GitHub secrets.
4.  **Build and Push**: It builds the Docker image from the `Dockerfile` and pushes the final image to my DockerHub repository.
