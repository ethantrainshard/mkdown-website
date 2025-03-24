---
tags:
    - set up
    - docker
    - container
---

# Docker - Containerization for Developers
 
<!-- ![ollama](https://ollama.com/public/ollama.png) -->

## Description
Docker is a platform designed to simplify application deployment, scaling, and management across different environments. It enables developers to package applications into lightweight, portable containers that can run consistently on any system or cloud.

It is a versatile platform that simplifies the process of building, deploying, and managing applications across different environments. Its key features make it an essential tool for developers and DevOps professionals looking to streamline their workflows.

## Key Features

1. Portability: Containers are self-contained and consistent, allowing them to run in any environment.
2. Efficiency: Shares the operating system kernel, reducing resource usage and startup time.
3. Isolation: Ensures applications run in isolated environments, preventing conflicts between dependencies.
4. Scalability: Easily scales applications up or down as needed using container orchestration tools.
5. Security: Provides strong isolation and security features to protect against vulnerabilities.

## Uses

- Development & Testing: Consistent development environments across different teams and machines.
- Deployment: Simplifies deployment to various cloud platforms and on-premises environments.
- CI/CD: Facilitates continuous integration and delivery pipelines.
- Microservices: Enables the creation of loosely coupled services.

## Installation Methods

#### 1. Windows Installation

- Download Docker Desktop from the [Docker website](https://www.docker.com/products/docker-desktop).
- Run the installer and follow the setup wizard to install Docker on Windows.

#### 2. macOS Installation

- Download Docker Desktop from the [Docker website](https://www.docker.com/products/docker-desktop).
- Run the downloaded .dmg file and drag Docker to your Applications folder.

#### 3. Linux Installation (Ubuntu)

- Open a terminal and run:
    ```bash
        sudo apt-get update
        sudo apt-get install docker-ce docker-ce-cli containerd.io
    ```
- Verify installation by running ```sudo docker --version```.

#### 4. Linux Installation (CentOS)

- Open a terminal and run:
    ```bash
        sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
        sudo yum install docker-ce docker-ce-cli containerd.io
    ```
- Verify installation by running ```sudo docker --version```.

#### 5. Linux Installation (Fedora)

- Open a terminal and run:
    ```bash
        sudo dnf config-manager --add-repo https://download.docker.com/linux/fedora/docker-ce.repo
        sudo dnf install docker-ce docker-ce-cli containerd.io
    ```
- Verify installation by running ```sudo docker --version```.