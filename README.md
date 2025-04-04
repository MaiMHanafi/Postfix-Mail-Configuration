# Ansible Playbook - SMTP Server Installation

## Overview
This repository provides an Ansible playbook to install and configure an SMTP server for use in automated deployment environments. It is designed to be easily integrated into CI/CD pipelines such as Jenkins for sending email notifications.

Repository: [Pre-requisites-SMT-Configuration](https://github.com/MaiMHanafi/Pre-requisites-SMT-Configuration.git)

## Features
- Installs Postfix, a popular and reliable SMTP server.
- Automatically configures mail relay settings.
- Ensures idempotent setup using Ansible.

## Project Structure
```
Pre-requisites-SMT-Configuration/
│-- smtp-playbook.yml
│-- inventory
│-- README.md
```

## Prerequisites
- Ansible installed on the control node
- SSH access to the target machine(s)

## Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/MaiMHanafi/Pre-requisites-SMT-Configuration.git
   cd Pre-requisites-SMT-Configuration
   ```

2. Update the `inventory` file with your target host IP or hostname.

3. Run the playbook:
   ```sh
   ansible-playbook -i inventory smtp-playbook.yml
   ```

## Customization
You can modify the `smtp-playbook.yml` file to set specific domain names, relay servers, or authentication methods depending on your environment requirements.

## License
This project is licensed under the MIT License.

---
Developed by [Mai Hanafi](https://github.com/MaiMHanafi) 💡

