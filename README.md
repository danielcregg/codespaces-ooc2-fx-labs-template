# Codespaces OOC2 JavaFX Labs Template

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![JavaFX](https://img.shields.io/badge/JavaFX-007396?style=flat-square&logo=java&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/danielcregg/codespaces-ooc2-fx-labs-template?style=flat-square)

A **GitHub Codespaces** template for **Object-Oriented Computing 2 (OOC2)** JavaFX lab exercises at ATU (Atlantic Technological University). Students can launch a fully configured Java + JavaFX development environment in the browser with a built-in virtual desktop for GUI applications -- no local installation required.

## Features

- **Java 21 (Zulu FX)** with JavaFX bundled out of the box
- **Desktop-lite VNC** environment (noVNC) for rendering JavaFX GUI windows directly in the browser
- Pre-configured VS Code extensions: Java Language Support, Debugger, Project Manager, IntelliCode
- Starter code with a console `HelloWorld` and a JavaFX `HelloWorldFX` application
- Designed for use with **GitHub Classroom** assignments

## Prerequisites

- A [GitHub](https://github.com) account
- Access to [GitHub Codespaces](https://github.com/features/codespaces)

## Getting Started

1. **Fork** this repository (or use it as a GitHub Classroom template).
2. Click the green **Code** button and select **Open with Codespaces**.
3. Wait for the Dev Container to build. This installs Java 21 with JavaFX and the VNC desktop.
4. Once ready, a **Simple Browser** tab opens automatically showing the virtual desktop (port `6080`).
5. Run the JavaFX application from the terminal or VS Code to see the GUI on the virtual desktop.

## Usage

### Run the console application

```bash
cd /workspaces/codespaces-ooc2-fx-labs-template
javac -d bin src/ie/atu/intro/HelloWorld.java
java -cp bin ie.atu.intro.HelloWorld
```

### Run the JavaFX application

```bash
cd /workspaces/codespaces-ooc2-fx-labs-template
javac -d bin src/ie/atu/intro/HelloWorldFX.java
java -cp bin ie.atu.intro.HelloWorldFX
```

The JavaFX window will appear on the virtual desktop accessible via the **Ports** tab (port 6080).

## Project Structure

```
codespaces-ooc2-fx-labs-template/
├── .devcontainer/
│   └── devcontainer.json       # Codespaces config (Java 21 FX + VNC desktop)
├── .vscode/
│   └── settings.json           # VS Code editor and Java project settings
├── src/
│   └── ie/atu/intro/
│       ├── HelloWorld.java     # Console "Hello, World!" starter
│       └── HelloWorldFX.java   # JavaFX GUI "Hello World" starter
├── LICENSE
└── README.md
```

## License

This project is licensed under the [MIT License](LICENSE).
