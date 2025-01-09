---
tags:
    - set up
    - pyenv
    - python
    - version management
---

# Pyenv - Python Version Management
 
<!-- ![ollama](https://ollama.com/public/ollama.png) -->

## Description
**Pyenv** is a command-line utility that allows you to manage multiple Python versions on your system. It simplifies the process of installing, switching between, and managing different versions of Python without affecting the global Python environment. 

It is a powerful tool that helps developers manage multiple Python versions efficiently and easily, making it an essential part of the development workflow.

## Key Features:

- Multiple Python Versions: Pyenv enables you to have multiple Python versions installed simultaneously.
- Version Management: Easily switch between different Python versions as needed for various projects.
- Shell Integration: Provides shell functions that simplify working with different Python versions.
- Compatibility: Works on Unix-like operating systems, including macOS and Linux.

## Pros:

- Isolation: Each Python version can be configured independently, avoiding conflicts between project requirements.
- Simplicity: Easy to install and use, reducing the complexity of managing multiple Python environments.
- Flexibility: Supports both global and local Python versions for different projects.
- Automation: Automates the process of switching between Python versions, saving time.

## Installation Methods:

#### 1. Using pyenv-installer (Recommended):

- Open a terminal and run:
    ```bash
        curl https://pyenv.run | bash
    ```
    or
    ```bash
        wget https://pyenv.run | bash
    ```
- Follow the installation instructions displayed in the terminal.

#### 2. Manual Installation:

- Clone the pyenv repository to your home directory:
    ```bash
        git clone https://github.com/pyenv/pyenv.git ~/.pyenv
    ```
- Add the following lines to your shell configuration file (```.bashrc```, ```.zshrc```, etc.):
    ```bash
        export PYENV_ROOT="$HOME/.pyenv"
        export PATH="$PYENV_ROOT/bin:$PATH"
        if command -v pyenv 1>/dev/null 2>&1; then
            eval "$(pyenv init --path)"
            eval "$(pyenv virtualenv-init -)"
        fi
    ```
- Apply the changes by sourcing your shell configuration file:
    ```bash
        source ~/.bashrc
    ```
    or
    ```bash
        source ~/.zshrc
    ```

#### 3. Using Homebrew (macOS):

- Open a terminal and run:
    ```bash
        brew update
        brew install pyenv
    ```
- Follow the installation instructions displayed in the terminal.

## Example Usage:

- Install a specific Python version:
    ```bash
        pyenv install 3.9.7
    ```
- Set a global Python version:
    ```bash
        pyenv global 3.9.7
    ```
- List all installed Python versions:
    ```bash
        pyenv versions
    ```
- Create a virtual environment for a project:
    ```bash 
        pyenv virtualenv 3.9.7 myproject-env
        pyenv activate myproject-env
    ```
