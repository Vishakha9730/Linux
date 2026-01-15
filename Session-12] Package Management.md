
# Package Management-
- Package Management is the method of installing and maintaining the package/software.
- Package management in Linux refers to the process of installing, updating, configuring, and removing software packages
- In Linux, software is available in the form of packages (packages are the collection of programs).
- And installing the packages means simply extracting the files from the archive and put it on the system.

# Repositories-
- Centralized location where software packages are stored and maintain that are made available for installation

# Dependencies-
- Some package requires shared library, or another package, called dependency.
- Dependency refers to a software component or library that another piece of software relies on in order to function correctly.

## Low-level Utilities-
- Low-level tool manages package files installation, update and uninstallation of package without their dependencies.
## High-level Utilities-
- high-level tool can install the package with their dependencies. 

| Linux Family | Low-level Tool | High-level Tool |
|--------------|----------------|-----------------|
| Red Hat      | rpm            | yum             |
| Debian       | dpkg           | apt-get         |

* Red Hat Based OS- Fedora, Linux, Amazon linux CentOS, Rhel, etc
* Debian Based OS- kali linux, Ubantu, etc
# rpm- 
- RPM packages are typically files with a .rpm extension.
- They are archives that contain the files to be installed, along with metadata such as package name, version, dependencies, and installation scripts.
#### rpm option package-name
- -i install package file
- -v verbose
- -h show hash bar
- -U Upgrade package
- -q query package
- -e erase package
# yum-
### To use YUM, you typically use commands like:
* Install a Package:
  - yum install package_name
* Update a Package:
  - yum update package_name
* Remove a Package:
  - yum remove package_name
* List Installed Packages:
  - yum list installed

# dnf - (Dandified Yum)
- DNF is a package manager used in RHEL, CentOS Stream, Rocky Linux, AlmaLinux, Fedora.
- It is the next-generation replacement of yum.

| Feature             | YUM                        | DNF           |
|---------------------|----------------------------|---------------|
| Full form           | Yellowdog Updater Modified | Dandified Yum |
| Speed               | Slower                     | Faster        |
| Dependency handling | Not very good              | Better        |
| Default OS          | RHEL 6 / 7                 | RHEL 8 / 9    |
| Memory usage        | High                       | Lower         |
| Python version      | Python 2                   | Python 3      |

