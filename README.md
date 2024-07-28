# node-todo-cicd

![diagram-export-28-07-2024-15_05_45](https://github.com/user-attachments/assets/2dcdb868-c8c3-4eb6-bccf-b9fe16378aec)


This diagram illustrates a real-world implementation of a CI/CD pipeline designed to streamline the deployment of Node.js applications on Amazon Elastic Container Service (ECS). By automating the build, test, and deployment processes, this pipeline significantly enhances development efficiency and reduces time-to-market.

## CI/CD Pipeline Overview
### Code Repository:
Code is stored and managed in GitHub.
### Build and Test:
Jenkins, running on an EC2 instance, automatically builds the Node.js application.
Unit and integration tests are executed.
### Docker Image Creation:
A Docker image is created containing the application and its dependencies.
### Image Storage:
The Docker image is pushed to Amazon ECR for secure storage and distribution.
### Deployment:
The updated image is deployed to an ECS cluster.
### Load Balancing:
An Application Load Balancer distributes traffic to the ECS cluster for high availability.
## Key Components

**GitHub**: Version control system for code management.

**Jenkins**: CI/CD automation server.

**Docker**: Containerization platform for building and packaging the application.

**Amazon ECR**: Container image registry for storing Docker images

**AWS ECS**: Container orchestration service for deploying and managing containers.

**Application Load Balancer**: Load balancer for distributing traffic across ECS instances.
