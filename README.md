# GitHub Classroom Base Java Autograding

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)

A base template repository for GitHub Classroom assignments in Java with Gradle and JUnit 5 autograding support.

## Overview

This project provides a ready-to-use Gradle project structure with JUnit 5 autograding support, designed for instructors using GitHub Classroom. When students push their code, GitHub Actions automatically runs the JUnit test suite and reports results back to GitHub Classroom. A VS Code Dev Container configuration is included for consistent development environments.

## Features

- **Gradle 7.5.1** build system with the Application plugin
- **JUnit 5** (Jupiter) test framework for autograding
- **Java 17** support via VS Code Dev Container
- **GitHub Classroom** compatible with automated test grading on push
- Pre-configured **Dev Container** for consistent development environments

## Prerequisites

- **Java 17** or higher
- **Gradle 7.5+** (or use the included Gradle Wrapper)
- **Git** for version control

## Getting Started

### Installation

1. Use this template to create a new GitHub Classroom assignment, or clone it directly:
   ```bash
   git clone https://github.com/danielcregg/github-classroom-base-java-autograding.git
   cd github-classroom-base-java-autograding
   ```

2. Open in a Dev Container (optional): If you are using VS Code, open the project in a Dev Container for a fully configured Java 17 + Gradle environment.

### Usage

Run the application:
```bash
./gradlew run
```

Run the tests locally:
```bash
./gradlew test
```

Submit your work (for students):
```bash
git add .
git commit -m "Description of changes"
git push origin main
```

Pushing to `main` triggers GitHub Actions autograding, which runs the JUnit test suite and reports results back to GitHub Classroom.

## Tech Stack

- **Java 17** - Programming language
- **Gradle 7.5.1** - Build automation tool
- **JUnit 5 (Jupiter)** - Testing framework for autograding
- **GitHub Actions** - CI/CD for automated test grading
- **VS Code Dev Containers** - Containerized development environment

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
