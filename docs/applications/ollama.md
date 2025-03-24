---
tags:
    - Docker
    - Ollama
    - Local AI
    - Step-By-Step
---

# Ollama - Your Local LLM Server
 
<p align="center">
    <img src="https://ollama.com/public/ollama.png" alt="Ollama">
</p>

## Description
Ollama is an open source project that aims to provide a local language model server. It is designed to be easy to use and deploy, making it accessible for developers and researchers alike.
Ollama is versatile and can be used in various applications such as chatbots, virtual assistants, and more. The community working on Ollama provides support and resources to help users get started with Ollama, and also provides different models for users to use.

Ollama can be installed on different platforms such as Linux, MacOS, and Windows. The installation process is straightforward and can be completed in a few minutes. It also supports docker.

## Purpose of Having a Local LLM
Having a local LLM server allows organizations which have restrictions for using AI. It gives them the flexibility to use AI without worrying about compliance issues, as they can control their own infrastructure. It also allows organizations to have more control over their data and avoid privacy concerns associated with cloud-based solutions.


## Uses
- Chatbots
- Virtual Assistants
- Language Translation
- Text Summarization
- Sentiment Analysis
- Question Answering
- Code Completion / Refactoring / Debugging


## Installation

#### MacOS
You can use download from Ollama offical website or install via Homebrew.

#### Linux

Run the following command to install ollama:
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

#### Windows

You can use download from Ollama offical website or install via Chocolatey.

#### Docker

The official Ollama Docker image [ollama/ollama](https://hub.docker.com/r/ollama/ollama) is available on Docker Hub.

### Docker (With Restriction)

If you are unable to create a Docker container using the official Ollama Docker image, you can use the following Dockerfile to build your own. The [Dockerfile](https://github.com/ethantrainshard/ollama-server-docker) is hosted in my Github Repo.

