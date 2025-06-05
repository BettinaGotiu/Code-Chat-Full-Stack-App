# Code Chat Full Stack App 

This project, **Code-Chat-2024**, is a cloud-native, production-ready full-stack chatbot application developed as part of the **Arnia x LigaAC Labs 2024** program. It was built under the guidance and mentorship of industry professionals and academic coordinators, offering valuable experience in collaborative software development and modern application architecture.

The app combines the power of contemporary web technologies with Large Language Model (LLM) integration and scalable AWS infrastructure to deliver intelligent, customizable chatbot interactions in a full-stack environment.

##  Purpose

- Deliver a scalable, full-stack chatbot with Retrieval-Augmented Generation (RAG) capabilities.
- Enable cloud-native deployment using AWS services.
- Provide consistent local development through DevContainers and Docker Compose.

---

##  Key Features

- Real-time AI-powered chat interface.
- LLM integration with LangChain and Amazon Bedrock.
- Modular monorepo structure for easy maintenance and extension.
- CI/CD-ready with full DevOps support and automated testing.
- Built with Next.js, Node.js, and DynamoDB, supporting full-stack scalability.

---

##  Architecture Overview

The project follows a monorepo pattern organized under `packages/`, with the major components:

- **Frontend:** `packages/client` – Built with Next.js and TypeScript.
- **API/Backend:** `packages/infra` – AWS Lambda (Node.js), API Gateway, and DynamoDB.
- **LLM Logic:** `packages/llm` – LangChain orchestration using Bedrock (Titan model).
- **Infrastructure:** `packages/infraorg` – Organization-level IaC using AWS CDK.

---

##  Technologies Used

| Layer            | Stack                                                                 |
|------------------|-----------------------------------------------------------------------|
| **Frontend**     | React, Next.js, TypeScript                                            |
| **Backend**      | Node.js, AWS Lambda, API Gateway, DynamoDB                           |
| **LLM**          | LangChain, Amazon Bedrock (Titan), vector search, embeddings         |
| **Infrastructure** | AWS CDK, S3, CloudFront, Route 53, Certificate Manager (ACM)        |
| **DevOps**       | Docker, Docker Compose, DevContainers, Yarn, Jest                    |
| **Other**        | Python (RAG utilities: `ragutil.py`, `requirements.txt`)             |

---

## Table of Contents

- [Code-Chat-2024](#code-chat-2024)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Requirements](#requirements)
  - [Installation](#installation)
    - [Postman](#postman)
  - [Running](#running)
    - [Web](#web)
      - [Shell](#shell)
      - [VSCode](#vscode)
    - [API](#api)
      - [Shell](#shell-1)
      - [VSCode](#vscode-1)

## Overview

ArniaxLigaAC Labs Fullstack Chatbot

Uses [`devcontainers`](https://code.visualstudio.com/docs/devcontainers/containers).

Advantages:

1. Consistent Environments: DevContainers ensure that every developer on a team is working with the same environment. This eliminates the "works on my machine" problem and makes onboarding new team members easier.
2. Isolation: DevContainers isolate your development environment from your local machine. This means you can work on multiple projects with different dependencies without conflicts.
3. Version Control: Since the configuration for a DevContainer is stored in a file, it can be version controlled. This means that changes to the development environment can be tracked and rolled back if necessary.
4. Integration with VS Code: DevContainers are deeply integrated with VS Code. This means you can use VS Code's features, like IntelliSense and debugging, inside the container.
5. Flexibility: DevContainers can be configured to use any Docker image. This means you can use any tools or languages that can be run in a Docker container, giving you a lot of flexibility in setting up your development environment.

## Requirements

- [Docker](https://docs.docker.com/engine/install/)
- [VSCode](https://code.visualstudio.com/download)
- VSCode Extension DevContainers (ms-vscode-remote.remote-containers)

  - Windows: Docker Desktop 2.0+ on Windows 10 Pro/Enterprise. Windows 10 Home (2004+) requires Docker Desktop 2.2+ and the WSL2 back-end. (Docker Toolbox is not supported.)
  - macOS: Docker Desktop 2.0+.
  - Linux: Docker CE/EE 18.06+ and Docker Compose 1.21+. (The Ubuntu snap package is not supported.)

## Installation

To install the necessary dependencies, run the following command:

```shell
yarn install
```

To enter DevContainer environment:

1. `(⌘/CTRL + SHIFT + P)`
2. `Dev Containers: Open Folder in Container`

### Postman

Postman collection has been attached to this repo [here](./docs/postman)

Import the collection and environment to facilitate development by calling API through an efficient and reproduceable flow.

## Running

### Web

To start the client application, run the following command:

#### Shell

```shell
yarn workspace @code-chat-2024/client dev
```

#### VSCode

1. `(⌘/CTRL + SHIFT + P)`
2. Task: Run Task
3. `Client Dev`

### API

To start the API application, run the following command:

#### Shell

```shell
yarn workspace @code-chat-2024/api dev
```

#### VSCode

1. `(⌘/CTRL + SHIFT + P)`
2. Task: Run Task
3. `API Dev`



1. Infrastructure as a Service IaaS
2. Platform as a Service PaaS
3. Software as a Service SaaS
