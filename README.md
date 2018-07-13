# The Tiger Guide
Code, git and publishing guidelines

## Table of contents
* [Code Guidelines](#code-guidelines)
    * [Code Style](#code-style)
* [Github Guidelines](#Github-Guidelines)
    * [Repository and File Naming](#repository-and-file-naming)
    * [License](#license)
    * [Readme style](#readme-style)
* [Build System Guildelines](#build-system-guidelines)
    * [gradle](#gradle)


# Code Guidelines
### Code Style
Every language used should be using the proper code style guidelines:
Java - [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)
Kotlin - [Kotlin's Coding Conventions](https://kotlinlang.org/docs/reference/coding-conventions.html)
Python - [PEP 8](https://www.python.org/dev/peps/pep-0008/?)
HTML/CSS - [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)
C++ - [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
JavaScript - [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)

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
