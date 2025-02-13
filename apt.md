# APT (Advanced Package Tool)

A comprehensive guide to using APT (Advanced Package Tool) for package management on Debian-based systems. This repository serves as a quick reference for common and advanced APT commands.

## Table of Contents
1. [Basic Package Management](#basic-package-management)
2. [Package Search and Information](#package-search-and-information)
3. [Package Upgrades](#package-upgrades)
4. [Package Removal](#package-removal)
5. [Source and Dependency Management](#source-and-dependency-management)
6. [Advanced APT Operations](#advanced-apt-operations)
7. [Legacy Commands](#old-apt-commands)

---

## Basic Package Management

Update Package Lists.
```bash
sudo apt update
```

Update all installed packages.
```bash
apt update
```

Install a package.
```bash
apt install ssh
```

Install multiple packages.
```bash
apt install vim nmap openssh
```

Install package with wildcard.
```bash
apt install zsh*
```

Reinstall a package.
```bash
apt reinstall
```

---

## Package Search and Information

Search for a package.
```bash
apt search nmap
```

Show package details.
```bash
apt show nmap
```

List all available packages.
```bash
apt list
```

Show all upgradable packages.
```bash
apt list --upgradable
```

Upgrade all installed packages.
```bash
apt list upgrade
```

---

## Package Upgrades 

Upgrade all installed packages.
```bash
apt upgrade
```

Perform a Full Upgrade (Including Dependencies).
```bash
apt full-upgrade
```

Upgrade to latest distribution.
```bash
apt dist-upgrade
```

Upgrade specific package.
```bash
apt install --only-upgrade vim
```

---

## Package Removal

Remove a package.
```bash
apt remove zsh
```

Remove package with wildcard.
```bash
apt remove zsh*
```

Completely Remove a Package (Including Configuration Files)
```bash
apt purge zsh
```

Remove unused packages.
```bash
apt autoremove
```

Remove unused packages in cache.
```bash
apt autoclean
```

Remove & purge a package.
```bash
apt remove --purge zsh
```

Clean package cache.
```bash
apt clean
```

---

## Source and Dependency Management

Download a package.
```bash
apt download nmap
```

Show package dependencies.
```bash
apt depends nmap
```

SHow Reverse dependencies of the package.
```bash
apt rdepends nmap
```

Source packet info of the package.
```bash
apt showsrc nmap
```

Download source of the package.
```bash
apt source nmap
```

Show changelog of the package.
```bash
apt changelog nmap
```

Fix broken packages.
```bash
apt --fix-broken install
```

---

## Advanced APT Operations

Search for files in packages.
```bash
sudo apt install apt-file
apt-file update
apt-file search <file_name>
```

Example: Search for `/usr/bin/zip`
```
apt-file search /usr/bin/zip
```

---

## Old APT Commands

Querying package information from the APT cache.
```bash
apt-cache
```

Query APT configuration.
```bash
apt-config
```

Search for files in packages.
```bash
apt-file
```

Used for package management.
```bash
apt-get
```

Show changelogs for upgrades.
```bash
apt-listchanges
```

Sort package lists.
```bash
apt-sortpkgs
```

Manage CD-ROM sources.
```bash
apt-cdrom
```

Extract configuration templates.
```bash
apt-extracttemplates
```

Create package archives.
```bash
apt-ftparchive
```

Manage APT keys.
```bash
apt-key
```

Mark packages as automatically/manually installed.
```bash
apt-mark
```

### apt-cache Conmmands

Search for a package.
```bash
apt-cache search nmap
```

Show package details.
```bash
apt-cache show nmap
```

Show package dependencies.
```bash
apt-cache depends nmap
```

Show reverse dependencies.
```bash
apt-cache rdepends nmap
```

Show source package details.
```bash
apt-cache showsrc nmap
```

Show package installation status.
```bash
apt-cache policy nmap
```

### apt-get Commands

Update package lists.
```bash
apt-get update
```

Upgrade installed packages.
```bash
apt-get upgrade
```

Install a package.
```bash
apt-get install nmap
```

Reinstall a package.
```bash
apt-get reinstall nmap
```

Remove a package.
```bash
apt-get remove nmap
```

Completely remove a package.
```bash
apt-get purge nmap
```

Remove unused packages.
```bash
apt-get autoremove
```

Clean package cache.
```bash
apt-get clean
```

Perform a distribution upgrade.
```bash
apt-get dist-upgrade
```

Perform a full upgrade.
```bash
apt-get full-upgrade
```

Download package source.
```bash
apt-get source nmap
```

Download a package.
```bash
apt-get download nmap
```

Show package changelog.
```bash
apt-get changelog nmap
```

---
