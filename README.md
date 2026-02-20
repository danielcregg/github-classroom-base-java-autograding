# GitHub Classroom Base Java Autograding

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/danielcregg/github-classroom-base-java-autograding?style=flat-square)

A base template repository for GitHub Classroom assignments in Java. This project provides a ready-to-use Gradle project structure with JUnit 5 autograding support, making it easy for instructors to create Java programming assignments that are automatically tested when students push their code.

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

1. **Use this template** to create a new GitHub Classroom assignment, or clone it directly:
   ```bash
   git clone https://github.com/danielcregg/github-classroom-base-java-autograding.git
   cd github-classroom-base-java-autograding
   ```

2. **Open in a Dev Container** (optional): If you are using VS Code, open the project in a Dev Container for a fully configured Java 17 + Gradle environment.

## Usage

**Run the application:**
```bash
./gradlew run
```

**Run the tests locally:**
```bash
./gradlew test
```

**Submit your work (for students):**
```bash
git add .
git commit -m "Description of changes"
git push origin main
```

Pushing to `main` triggers GitHub Actions autograding, which runs the JUnit test suite and reports results back to GitHub Classroom.

## Project Structure

```
.
├── app/
│   ├── build.gradle                        # Application build config (JUnit 5, Guava)
│   └── src/
│       ├── main/java/miPaquete/App.java    # Main application class
│       └── test/java/miPaquete/AppTest.java # JUnit 5 test class
├── .devcontainer/                          # VS Code Dev Container configuration
│   ├── devcontainer.json
│   └── Dockerfile
├── gradle/wrapper/                         # Gradle Wrapper files
├── settings.gradle                         # Gradle settings
├── gradlew                                 # Gradle Wrapper (Linux/macOS)
└── gradlew.bat                             # Gradle Wrapper (Windows)
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
