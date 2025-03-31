# Ansible Skeleton Template

This repository provides a clean and modular file structure template for building Ansible projects. Whether you’re just starting out with Ansible or looking to standardize your projects, this skeleton will help you get organized quickly.

---

## Table of Contents

- [Overview](#overview)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

The Ansible Skeleton Template is designed to serve as a starting point for Ansible automation projects. I prefer a modular layout that separates inventories, playbooks, and roles, ensuring a clean and scalable codebase.

---

## File Structure

Below is the typical directory structure provided by this template:

```
ansible-skeleton/ 
├── group_vars/ 
├── host_vars/ 
├── inventory/ 
├── playbooks/ 
├── roles/ 
│ ├── common/ 
│ │ ├── tasks/
│ │ │ └── main.yml
│ │ ├── handlers/
│ │ │ └── main.yml
│ │ ├── templates/
│ │ ├── files/
│ │ ├── vars/
│ │ │ └── main.yml
│ │ ├── defaults/
│ │ │ └── main.yml
│ │ ├── meta/ 
│ │ │ └── main.yml 
├── ansible.cfg 
└── README.md
```

- **inventories/**: Contains host inventory files for different environments (e.g., development, production).
- **playbooks/**: Stores your Ansible playbooks. The `site.yml` playbook is often used as the main entry point.
- **roles/**: Contains modular roles. A sample `common` role is provided, which can be extended or replicated for other functionalities.
- **ansible.cfg**: Custom Ansible configuration file to override default settings.

---

## Getting Started

### Prerequisites

- **Ansible:** Ensure Ansible is installed on your system. For installation instructions, please refer to the [Ansible documentation](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

### Installation

1. **Clone the Repository:**

```bash
git clone https://github.com/redkeysh/ansible-skeleton.git
cd ansible-skeleton
```

2.  **Configure Inventories:**
    
Edit the host files under the `inventories/` directory to reflect your environment details.
    
3.  **Customize Playbooks and Roles:**
    
 Modify the playbooks in the `playbooks/` directory and roles in the `roles/` directory according to your project requirements.
    

----------

## Usage

To run a playbook with a specific inventory, use the following command:

```bash
ansible-playbook -i inventory/sample_yml_inventory.yml
```

Replace `inventory/sample_yml_inventory.yml` with the appropriate inventory file for your environment.

----------

## Customization

-   **Inventories:** Customize the host entries in each inventory file to match your target environments.
    
-   **Roles:** Expand the roles with new tasks, handlers, variables, templates, and files as needed.
    
-   **Configuration:** Edit the `ansible.cfg` file to adjust settings such as roles path, inventory, and logging options.
    

----------

## Contributing

Contributions are welcome! Please refer to the CONTRIBUTING.md file for guidelines on how to contribute to this project.

----------

## License

This project is licensed under the MIT License. See the LICENSE file for details.

----------

## Contact

For any questions or suggestions, please open an issue or contact me.
