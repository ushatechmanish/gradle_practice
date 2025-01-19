# Gradle Build Tool Overview

Gradle is a powerful build automation tool that simplifies tasks like compiling, testing, publishing, managing dependencies, and handling transitive dependencies with their versions.

---

## Key Concepts in Gradle

### Build Scripts vs. Build Configuration
- **Earlier**: Build scripts were used.
- **Now**: Build configuration is employed for better clarity and efficiency.

### Configuration Files
1. **`build.gradle`**
    - Core file for project configuration.
    - Used to define dependencies, plugins, and tasks.
    - In multi-module projects, the root `build.gradle` often contains shared dependencies and configurations.

2. **`settings.gradle`**
    - Primarily for managing **multi-module projects**.
    - Specifies project structure and module inclusion.

---

## Gradle Philosophy: Convention Over Configuration
- Gradle assumes a **default project structure** for Java source files, resources, tests, etc.
- You can override this structure explicitly in the build configuration.

---

## Modern Practices in Gradle
1. **Kotlin vs. Groovy**
    - Kotlin provides better **IDE support** compared to Groovy for build configurations.

2. **Version Management**
    - Use `libs.versions.toml` to manage dependency versions, ensuring cleaner and more maintainable configurations.

3. **Gradle Wrapper**
    - Ensures **consistent and reproducible builds** across environments.
    - Highly recommended for all Gradle projects.

---

## Creating a New Gradle Project
Run the following commands to initialize a new project:
```bash
mkdir <project-folder> ; cd <project-folder> ; gradle init

```
This will give various options. Choose as per your requirement 

## Notes
he `build.gradle` in root project is normally used for having shared dependencies and configuration .

There are other modern ways so you may not find the build.gradle in the root project 