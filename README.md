# Ansible Role: user_management

# Disclaimer

I couldn't be responsible with any production issues if you use this role without any prior tests.  
This role is designed for my proper environment and possibly not correspond to your.

The master branch is development branch. Use only release/* branches for production.

# Introduction

This role is designed to perform user management (creation/update/deletion) on GNU/Linux servers and to performs systems updates.  
It's structured and do tasks according to my own requirements and production needs.  
Feel free to fork and update this according to your requirements.

# Supported OS

**Debian** :
- buster (10)
- bullseye (11)

**Ubuntu** :
- Bionic Beaver (18.04) - ESS : 04/2023 / EOL : 04/2028
- Focal Fossa (20.04) - ESS : 04/2025 / EOL : 04/2030
- Hirsute Hippo (21.04) - ESS : 01/2022 / EOL : 01/2022

**Rocky** :
- 8

**RHEL** :
- 8

# Variables

Read content of [defaults variables](./defaults/main.yml) to get configurables variables

# Requirements

## On target OS

You need to have python3 package installed on remote OS to use this role.

# Actions

- Full create user
- Deploy SSH authorized keys
- Update password
- Remove user and home directory

# Changelog

To clearest and updated changelog, I encourage you to see pull requests with flags "feature".

# Roadmap

You could refer to milestones to full current roadmap.

### v1.0.0

- Hability to manage users on following OS :
  - Debian 10
  - Debian 11
  - RHEL 8
  - Rocky 8
  - Ubuntu 18.04
  - Ubuntu 20.04
  - Ubuntu 21.04

# Tests

Initials tests was done through molecule.  
Role fully tested on virtual machines vanilla installed.
