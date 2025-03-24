---
tags:
    - set up
    - poetry
    - dependency management
    - version management
---

# UV - Alternative to Poetry

I have been using UV for a while and it has been working well for me. It is a great alternative to Poetry if you are looking for something that is more lightweight and easier to use. 

 UV is an extremely fast Python package installer and resolver, written in Rust, and a single tool to replace pip, pip-tools, pipx, poetry, pyenv, twine, virtualenv, and more. It is designed to be fast and efficient, making it ideal for projects with many dependencies. UV is created by the company Astral, who is also the creators of ruff, a linter for Python. Check them out at [https://astral.dev/uv](https://astral.dev/uv).

Here are some of the key features of UV:

- **Lightweight**: UV is a lightweight tool that does not require any dependencies other than Python.
- **Easy to Use**: UV is easy to use and has a simple command-line interface.
- **Dependency Management**: UV can manage dependencies for your project, including installing and updating packages.
- **Version Management**: UV can manage the version of Python that you are using for your project.

#### Installation

- On macOS and Linux

```bash
    # On macOS and Linux.
    curl -LsSf https://astral.sh/uv/install.sh | sh
```

- On Windows

```bash
    # On Windows.
    powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

#### My Workflow using UV

1. Install the version of Python that I want to use for my project.
    
    ```bash
        # This is for multiple Python version, you can just indicate the version you want to install
        uv python install 3.10 3.11 3.12
        Searching for Python versions matching: Python 3.10
        Searching for Python versions matching: Python 3.11
        Searching for Python versions matching: Python 3.12
        Installed 3 versions in 3.42s
        + cpython-3.10.14-macos-aarch64-none
        + cpython-3.11.9-macos-aarch64-none
        + cpython-3.12.4-macos-aarch64-none
    ```

2. Ensure that the python version that you wanted is installed

    ```bash
        uv python list
    ```
3. Create the project folder using uv. It will create a folder with all the necessary files and virtual environment for your project.

    ```bash
        uv init <project name>
    ```

    ```
        .
        ├── .venv
        │   ├── bin
        │   ├── lib
        │   └── pyvenv.cfg
        ├── .python-version
        ├── README.md
        ├── hello.py
        ├── pyproject.toml
        └── uv.lock
    ```

4. Install dependencies using ``` uv add```. You can also remove the dependencies using ```uv remove```

    ```bash
        # Add a package to your project's virtual environment
        uv add <package name>
        
        # Install a specific version of a package
        uv add <package name>==<version number>
        
        # Remove a package from your project's virtual environment
        uv remove <package name>
    ```

5. To run the project using the virtual environment created, you can use ```uv run```.
    
    ```bash
        # Run a Python script in your project's virtual environment
        uv run <Python file>

        # Run a Flask application using uv (for example)
        uv run flask app.py --host 0.0.0.0 --port 5000
    ```

Once you have the hang of uv, it will be easy to manage your project's virtual environment and dependencies.