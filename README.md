# Logo Project 

---

**Project Summary**

This project demonstrates how to build, test, and deploy a basic React.js application using GitLab CI/CD, Docker, and Terraform.

**Application**

The application is a simple "Hello, World!" app showcasing fundamental concepts of React.

**Dockerfile**

The Dockerfile is used to build the Docker image of the application. It performs the following steps:

- Creates a base image using node:18.
- Installs the application's dependencies.
- Copies the application's code.
- Compiles or runs the application code.

**GitLab CI/CD**

GitLab CI/CD provides an automation system for building, testing, and deploying the application. It executes the following stages:

- **Build:** Creates the Docker image of the application.
- **Test:** Runs the application's tests.
- **Publish:** Uploads the Docker image of the application to GitLab.

**Terraform**

Terraform is used to automate the creation of AWS infrastructure, including:

- **VPC:** Virtual Private Cloud where the application operates.
- **Security Groups:** Controls access to the application.
- **ECS Fargate:** Runs the application as a Fargate instance.
- **Load balancer:** Distributes traffic to the application.

**Technologies Used**

- React.js
- Docker
- GitLab CI/CD
- Terraform

**Pipeline Details**

The pipeline includes the following stages:

- **Build:**
    - Executes the Dockerfile for the application.
    - Creates the Docker image of the application.
- **Test:**
    - Runs tests for the application.
- **Publish:**
    - Uploads the Docker image of the application to GitLab.

**Comments in Dockerfile**

Comments in the Dockerfile explain why specific commands are used. For instance, the following comment clarifies why the node:18 image is used:

`# Create a base image from node:18
FROM node:18`

**Comments in GitLab YAML**

Comments in GitLab YAML explain the reasons for executing stages. For example:

`# Create the Docker image of the application
stage: build`

**Optional Components**

The project may optionally include:

- **Automatic scaling in Fargate instances**
- **Performance monitoring**
- **AWS architecture diagram**
- **Custom runner**

**Conclusion**

This project demonstrates how to build, test, and deploy a basic React.js application using GitLab CI/CD, Docker, and Terraform.
