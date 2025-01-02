# Ansible Playbook Skeleton

## Overview
Ansible Playbook Skeleton is a starter template designed to help you create Ansible playbooks with the recommended directory structure. This repository provides a solid foundation for organizing your playbooks and adhering to best practices, making your workflow more efficient and maintainable.

## Features
- Predefined directory layout based on Ansible best practices.
- Example files to guide you in setting up roles, tasks, and configurations.
- Ready-to-use structure for scalable and reusable playbooks.

## Directory Structure
The project follows the recommended Ansible directory structure:

```
ansible-playbook-skeleton/
├── roles/              # Directory for role definitions
│   ├── myproject/   # Example role
│   │   ├── tasks/      # Role tasks
│   │   ├── handlers/   # Role handlers
│   │   ├── templates/  # Jinja2 templates
│   │   ├── files/      # Static files
│   │   ├── vars/       # Role-specific variables
│   │   ├── defaults/   # Default variables
│   │   ├── meta/       # Role metadata
├── inventories/        # Inventory files (e.g., production, staging)
|   ├── hosts/
├── group_vars/         # Group-specific variables
├── host_vars/          # Host-specific variables
├── playbooks/          # Playbook YAML files
├── ansible.cfg         # Ansible configuration file
├── requirements.yml    # Role dependencies
|── myproject.yml    # Role dependencies
├── README.md           # Project documentation
```

## Getting Started
### Prerequisites
Ensure you have the following installed:
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

### Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/MehrdadLinux/ansible-playbook-skeleton.git
   ```
2. Navigate to the project directory:
   ```bash
   cd ansible-playbook-skeleton
   ```
3. Customize the directory structure and example files to fit your project.
4. Start writing your playbooks and roles!

### Example
Here’s an example of running a playbook:
```bash
ansible-playbook -i inventories/production playbooks/site.yml
```

## Contributing
Contributions are welcome! If you have suggestions for improvements or want to report a bug, please open an issue or submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- Inspired by Ansible's [Sample-directory-layout](https://docs.ansible.com/ansible/latest/tips_tricks/sample_setup.html#sample-directory-layout).
- And Inspired by Ansible's [Best Practices](https://docs.ansible.com/ansible/2.8/user_guide/playbooks_best_practices.html#directory-layout).
- Thanks to the open-source community for providing guidance and feedback.

## Contact
For questions or support, feel free to reach out to [MehrdadLinux@gmail.com] or create an issue in this repository.

---

Happy automating with Ansible! 🎉
