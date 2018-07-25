# The Tiger Guide
Code, git, and publishing guidelines

## Table of contents
* [Code Guidelines](#code-guidelines)
    * [Code Style](#code-style)
    * [The Module System](#the-module-system)
        * [Modules explained](#modules-explained)
        * [Developing a module](#developing-a-module)
        * [Using a module](#Using-a-module)
* [Github Guidelines](#Github-Guidelines)
    * [Repository and File Naming](#repository-and-file-naming)
    * [License](#license)
    * [Readme style](#readme-style)
* [Build System Guildelines](#build-system-guidelines)
    * [gradle](#gradle)
        * [Gradle wrapper](#Gradle-wrapper)
        * [Gradle plugins](#Gradle-plugins)


# Code Guidelines
### Code Style
Every language used should be using the proper code style guidelines:
|  Language  | Guide                           |
|------------|---------------------------------|
| Java       | [Google's Java Style Guide](https://google.github.io/styleguide/javaguide.html)       |
| Kotlin     | [Kotlin's Coding Conventions](https://kotlinlang.org/docs/reference/coding-conventions.html)     |
| Python     | [PEP 8](https://www.python.org/dev/peps/pep-0008/?)                           |
| HTML/CSS   | [Google's HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)   |
| C++        | [Google's C++ Style Guide](https://google.github.io/styleguide/cppguide.html)        |
| JavaScript | [Google's JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html) |
### The Module System
#### Modules Explained
When we program a robot, things can get messy pretty fast; especially when working a very big project. The larger a project's scope, the more difficult it becomes to debug and maintain. Thus, the modular system was created. By delegating each task to a different library, we can divide the project into modules in a clear, efficient way. Then, when we want to use our module, we can compile the corresponding libraries using [Gradle](#Gradle). 

#### Developing a module
Each module has it's own repository in order to decrease the difficulty of module maintenance. When we make a change and want to update the module, we will release a new version of the code to Github using [Github Releases](https://blog.github.com/2013-07-02-release-your-software/). 

#### Using a module
In order to import and use our module, we will use [Jitpack](https://jitpack.io/). Using Jitpack we are able to fetch Github releases using `maven` and use them as dependencies in our [Gradle](#Gradle) project. Check the [Jitpack site](https://jitpack.io/) for more information.

#### Modules List
|  Module       | Description                                                                        |
|---------------|------------------------------------------------------------------------------------|
| [Framework](https://github.com/Tiger-team-2679/FRC-Framework)     | A module created for managing the robot's system and functionality.                |
| [Logger](https://github.com/Tiger-team-2679/FRC-Logger)        | A module created for logging the robot's and other modules' information.           |
| [Web Dashboard](https://github.com/Tiger-team-2679/FRC-Web-Dashboard) | A custom dashboard created to facilitate custom data transference.                 |
| [Motion](https://github.com/Tiger-team-2679/FRC-Motion)        | A module containing the autonomous algorithms, like PID and Trajectory Generation. |

# GitHub Guidelines
### Repository and File Naming 
Repository names should use higher-case with hyphens in place of spaces between words (also known as Kebab-Case).
Programming language source files should use the style dictated by the style guide for that language.

### License 
Every project should contain a license in a file called LICENSE containing the project's license information.
The license of the repository must be declared in the project's Readme file as well, with a link to the LICENSE file.

### Readme Style
Every repository should contain a Readme file. Readme files should always contain a title (declared with #) as the repository's name, with spaces instead of hyphens. Also, every Readme should contain a table of contents linking to every part of the Readme file.

# Build System Guidelines
Every project, if necessary, should contain a proper Gradle configuration for building and testing.
## Gradle
If you don't know what Gradle is, go read about it right [here](https://docs.gradle.org/current/userguide/userguide.html).
The Gradle project must contain the files necessary for building the program and must use the Gradle wrapper.

### Gradle wrapper
Instead of downloading Gradle to the computer we are working on, we can use the Gradle wrapper. The Gradle wrapper is a version of Gradle that can be run only by using the Gradle jar and executables, That way we can use Gradle on any computer with Java installed.

### Gradle plugins
In order to expand the abilities of Gradle, we will use Gradle plugins. For example, in order to deploy and compile our robot code easily, we will use the [GradleRio](https://github.com/wpilibsuite/GradleRIO) plugin. 

