---
tags:
    - set up
    - poetry
    - python
    - dependency management
---

# Poetry - Packaging and Dependency Management

## Description
**Poetry** is a packaging and dependency management tool for Python. It simplifies the process of managing dependencies and packaging your Python projects, ensuring they are easily shareable and deployable.

It is an excellent tool for Python developers, simplifying the process of managing dependencies and packaging projects. Its key features make it a valuable addition to any development workflow.

## Key Features:

1. Dependency Management: Manages project dependencies in an isolated environment.
Version Constraints: Specifies version constraints for packages to ensure compatibility.
2. Virtual Environment Management: Automatically manages virtual environments for each project.
3. Packaging & Distribution: Simplifies the packaging and distribution of Python projects.
4. Consistent Project Structure: Ensures consistent structure across different projects.

## Installation Methods:

#### 1. Using pip (Python's Package Installer):

- Open a terminal and run:
    ```bash
        pip install poetry
    ```

#### 2. Installing from Source:

- Clone the Poetry repository to your local machine:
    ```bash
        git clone https://github.com/python-poetry/poetry.git ~/.poetry
    ```
- Add the following lines to your shell configuration file (```.bashrc```, ```.zshrc```, etc.):
    ```bash
        export PATH="$HOME/.poetry/bin:$PATH"
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
        brew install poetry
    ```

#### 4. Using Scoop (Windows):

- Install Scoop if you haven't already by following the instructions on Scoop's website.
- Open PowerShell as Administrator and run:
    ```powershell
        scoop bucket add extras
        scoop install poetry
    ```

## Example Usage:

- Initialize a new Poetry project:
    ```bash
        poetry new my-project
    ```
- Install dependencies from ```pyproject.toml```:
    ```bash
        poetry install
    ```
- Add a dependency to your project:
    ```bash
        poetry add requests
    ```
- Build your project package:
    ```bash
       poetry build
    ```
- Publish your package to PyPI:
    ```bash
       poetry publish
    ```
