---
tags:
    - Set Up
    - VScode
    - IDE
    - Tools
---

# VSCode - IDE for Developers
 
<!-- ![ollama](https://ollama.com/public/ollama.png) -->

## Description
VSCode (Visual Studio Code) is an open-source code editor made by Microsoft that supports programming in multiple languages, including JavaScript, Python, C++, Java, and many others. It offers a lightweight yet powerful toolset, allowing developers to quickly build, debug, and test applications with the help of extensions, which add functionality to the core editor.

It is a powerful and flexible tool that offers both beginner-friendly features and advanced capabilities for professional developers, making it an excellent choice for a wide range of programming tasks.

#### Key Features:

- Lightweight & Fast: VSCode is designed for efficiency, requiring minimal system resources.
- Rich Extensions: A vast ecosystem of extensions that can enhance its functionality based on developer needs.
- IntelliSense: Provides intelligent code completion and suggestions, improving productivity.
- Debugger Support: Supports debugging for various languages directly from the editor.
- Git Integration: Built-in support for Git version control.
- Terminal & SSH: Integrated terminal and SSH capabilities make it easy to work with remote servers.

#### Pro Features:

- Multi-language Support: Excellent support for multiple programming languages.
- Extensibility: Highly extensible through a rich plugin ecosystem.
- User-Friendly Interface: Intuitive UI and customizable settings.
- Cross-Platform: Available on Windows, macOS, and Linux.

## Installation Methods

#### 1. Windows Installation:

- Download the installer from the [VSCode website](https://code.visualstudio.com).
- Run the downloaded ```.exe``` file and follow the installation wizard to complete the setup.

##### 2. macOS Installation:

- Download the ```.zip``` archive from the [VSCode website](https://code.visualstudio.com).
- Unzip the contents and move the Visual Studio Code.app to your Applications folder.

##### 3. Linux Installation:

- For Debian-based systems (like Ubuntu), open a terminal and run:
  ```bash
    sudo apt update
    sudo apt install software-properties-common apt-transport-https wget
    wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
    sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
    sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/trusted.gpg.d/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'
    rm -f packages.microsoft.gpg
    sudo apt update
    sudo apt install code
  ```
  - For Red Hat-based systems (like Fedora), open a terminal and run:
    ```bash
        sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
        sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
        sudo dnf check-update
        sudo dnf install code
    ```