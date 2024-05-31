# Package Management System - Draft

## :newspaper: About the project

The Package Management System is a command line tool designed to manage packages stored as zip archives. It provides functionalities to install, uninstall, and reset packages, ensuring smooth package management operations.

### How it works

1. Run the script `main.cpp` with appropriate commands to perform package management tasks. For example, `packages-manager.exe install package_id` installs a package (zip archive), `packages-manager.exe uninstall package_id` uninstalls a package, and `packages-manager.exe reset` resets the package storage.

2. The system manages package information stored in the `pkgs.json` file, which includes package IDs, URLs, and installation directories.

### Content overview

    .
    ├── packages_manager - package manager project
    ├── pkgs_installed/ - folder to store installed packages
    ├── storage/ - folder to store package archives    
    ├── vcpkg/ - contains vcpkg package manager
    ├── tests/ - folder to store the installed packages
    ├── .gitignore - ignore files, folders, etc. for version control
    ├── CMakeLists.txt - configurations for cmake buildsystem
    ├── CMakePresets.json - settings for cmake buildsystem
    ├── COPYRIGHT - project copyright
    └── README.md - relevant information about the project

## :notebook: Features

* Install packages from storage
* Uninstall installed packages
* Reset package storage
* Logging available

## :runner: Getting started

### Prerequisites

0. Clone the project:

```sh
git clone https://github.com/CH6832/packages-manager.git
```

1. Navigate into root folder:

```sh
cd packages-manager
```

### Usage

1. Run the script `main.cpp` with appropriate commands:

```sh
python main.py [install/uninstall/reset] [package_id]
```

2. Example usage:

```sh
python main.py install test1-1.2.0
```

## :books: Resources used to create this project

* CPlusPlus
  * [C++ Programming Language](https://devdocs.io/cpp/)
  * [Standard C++ Library reference](https://cplusplus.com/reference/)
  * [C++ reference](https://en.cppreference.com/w/)
  * [CMake Documentation and Community](https://cmake.org/documentation/)
* Editor
  * [Visual Studio Community Edition](https://code.visualstudio.com/)

## :bookmark: License

This project is licensed under the terms of the [MIT License](LICENSE).

## :copyright: Copyright

See the [LICENSE](LICENSE) file for copyright and licensing details.
