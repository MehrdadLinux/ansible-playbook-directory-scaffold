<div align="center">

![Wave divider](https://readme-svg-wave-divider-generator.vercel.app/wave?type=sine&width=1200&height=200&amplitude=40&frequency=2&layers=3&color_top=d93d37&color_bottom=0d1117&opacity=1&flip=true&gradient=true&mirror=true&animate=true&speed=6&text=Ansible&text_bottom=Playbook+Skeleton&text_color=ffffff&text_bottom_color=ff7070&text_size=102&text_bottom_size=31&text_style=bold&text_stroke_color=0d1117&text_stroke_width=10&text_scale_x=100&text_scale_y=100&text_x=50&text_y=45&text_gap=50&text_align=middle)
<h1 align="center">
    ${\color{red}Ansible}$ ${\color{green}Playbook }$ ${\color{red}Skeleton}$
  <br>
</h1>

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
│   ├── myproject/      # Example role
│   │   ├── tasks/      # Role tasks
│   │   ├── handlers/   # Role handlers
│   │   ├── templates/  # Jinja2 templates
│   │   ├── files/      # Static files
│   │   ├── vars/       # Role-specific variables
│   │   ├── defaults/   # Default variables
│   │   ├── meta/       # Role metadata
├── inventories/        # Inventory files (e.g., production, staging)
|   ├── hosts
|   ├── production
|   ├── staging
├── group_vars/         # Group-specific variables
├── host_vars/          # Host-specific variables
├── playbooks/          # Playbook YAML files
├── ansible.cfg         # Ansible configuration file
├── requirements.yml    # Role dependencies
|── myproject.yml       # Role dependencies
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
ansible-playbook -i inventory/hosts myproject.yml -e "ansible_root=[Your_Path] project_name=[PlayBookName]"
example : ansible-playbook -i inventory/hosts myproject.yml -e "ansible_root=/tmp/1 project_name=ansible_project"
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
![Wave divider](https://readme-svg-wave-divider-generator.vercel.app/wave?type=sine&width=1200&height=70&amplitude=20&frequency=2&layers=3&color_top=000000&color_bottom=d93d37&opacity=1&flip=false&gradient=false&mirror=true&animate=true&speed=6&text=&text_bottom=&text_color=ffffff&text_bottom_color=ff7070&text_size=102&text_bottom_size=31&text_style=bold&text_stroke_color=0d1117&text_stroke_width=10&text_scale_x=100&text_scale_y=100&text_x=50&text_y=45&text_gap=50&text_align=middle)
Happy automating with Ansible! 🎉
