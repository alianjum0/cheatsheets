#-#
#-# Package management
#-#

#-# Advanced Packaging Tool (apt)

Command                                    Description
-------                                    -----------
apt-get install <package-name>             Install specified package(s), along with any dependencies.
apt-get remove <package-name>              Removes specified package(s), but don't remove dependencies.
apt-get autoremove                         Remove 'orphaned' dependencies which are installed but are not used by any apps.
apt-get clean                              Remove downloaded package files (.deb) for software that is already installed.
apt-get purge [package-name]               Remove and clean a specific package. (also removes configuration files)
apt-get update                             Read /etc/apt/sources.list and update the system’s database of available packages.
apt-get upgrade                            Upgrade all packages if there are updates available.
apt-cache search <package-name>            Find out the name of a package that you know is in the system.
apt-cache show <package-name>              Show details about a package, including description, dependency info and version numbers.
apt-cache depends <package name(s)>        List the packages that the specified packages depends upon in a tree.
apt-cache rdepends <package name(s)>       Generate and output the list of packages that depend upon the specified package.
apt-cache pkgnames                         Generate a list of the currently installed packages on your system.

[reference](https://github.com/vrachieru/cheatsheet)
