# The Tiger Guide
Code, git and publishing guidelines

## Table of contents
* [Code Guidelines](#code-guidelines)
    * [Code Style](#code-style)
    * [The Module System](#the-module-system)
        * [Modules explained](#modules-explained)
        * [Developing a module](#developing-a-module)
        * [Using a module](#Using-a-modules)
* [Github Guidelines](#Github-Guidelines)
    * [Repository and File Naming](#repository-and-file-naming)
    * [License](#license)
    * [Readme style](#readme-style)
* [Build System Guildelines](#build-system-guidelines)
    * [gradle](#gradle)


# Code Guidelines
### Code Style
Every language used should be using the proper code style guidelines:
* Java - [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
* Kotlin - [Kotlin's Coding Conventions](https://kotlinlang.org/docs/reference/coding-conventions.html)
* Python - [PEP 8](https://www.python.org/dev/peps/pep-0008/?)
* HTML/CSS - [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
* C++ - [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* JavaScript - [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)

### The Module System
#### Modules Explained
When we are programming a robot, things can get messy very fast, especially when are creating a very big project, It's harder to debug and maintain, Thus the module system was created. By creating libraries with different tasks, we can divide the project into modules with different tasks. Then when we want to use our module we can compile them using [Gradle](#Gradle). 

#### Developing a module
each module has it's own repository, in order to make the module more maintainable. When we make a change and want to update the module, we will release a new version of the code to Github using [Github Releases](https://blog.github.com/2013-07-02-release-your-software/). 

#### Using a modules
In order to import and use our module, we will use [Jitpack](https://jitpack.io/). Using Jitpack we are able to fetch Github releases using maven and use them as dependencies in our [Gradle](#Gradle) project. Check the [Jitpack site](https://jitpack.io/) for more information.

#### Modules List
* [Framework](https://github.com/Tiger-team-2679/FRC-Framework) - A module created for managing the robot's system and functionality.
* [Logger](https://github.com/Tiger-team-2679/FRC-Logger) - A module created for logging robot and other modules' information.
* [Web Dashboard](https://github.com/Tiger-team-2679/FRC-Web-Dashboard) - A custom dashboard created to enable custom data transference.
* [Motion](https://github.com/Tiger-team-2679/FRC-Motion) - A module containing the autonomous algorithms, like PID and 

# Github Guidelines
### Repository and File Naming 
Repository names should use higher-case with hyphens in place of spaces between words.
Programming language source files should use the style dictated by the style guide for that language.

### License 
Every project should contain a license in a file called LICENSE containing the project's license (dah...).
The license of the repository must be declared as well in the project's Readme file, attached with a link to the LICENSE file.

### Readme Style
Every repository should contain a Readme file. Readme files should always contain a title declared with # as the repositories' name, with spaces instead of hyphens. also, every Readme should contain a table of contents, with linking to every part of the Readme.

# Build System Guidelines
Every project, if necessary, should contain a proper Gradle configuration for building and testing.
### Gradle
If you don't know what Gradle is, go read about it right [here](https://docs.gradle.org/current/userguide/userguide.html).
The Gradle project must contain the files necessary for building the program and must use the Gradle wrapper.
