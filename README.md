📌 Overview

This project demonstrates a role-based Ansible architecture built using ansible-galaxy best practices.

It simulates real-world DevOps automation scenarios including:

Configuration standardization

Login banner management

Secure system file backup

Centralized user provisioning

The project is structured using reusable Ansible roles to reflect production-grade infrastructure design.

🏗 Project Architecture
ansible-project/
│
├── inventory
├── ansible.cfg
├── site.yml
│
└── roles/
    ├── selinux/
    ├── motd/
    ├── backup/
    └── users/

Each role contains modular components such as:

tasks/

handlers/

templates/

defaults/

This structure mirrors enterprise automation standards.

🚀 Roles & Real-World Use Cases
🔐 SELinux Role

Standardizes SELinux configuration across servers using templating and handlers.

Why it matters:
Ensures consistent security policy enforcement across environments (dev, staging, production).

🖥 MOTD Role

Deploys a dynamic login banner showing:

Hostname

IP address

OS version

Why it matters:
Prevents operational mistakes by clearly identifying connected servers.

📦 Backup Role

Uses the fetch module to securely back up critical system files.

Why it matters:
Provides rollback safety before patching or major configuration changes.

👤 Users Role

Automates user creation across multiple servers using loops.

Why it matters:
Enables consistent user provisioning across environments.

▶️ Usage

Run full automation:

ansible-playbook site.yml

Run syntax check:

ansible-playbook site.yml --syntax-check
🧠 Concepts Demonstrated

Role-based automation design

Infrastructure as Code (IaC)

Jinja2 templating

Idempotent configuration management

Conditional handlers

Loop-driven automation

Modular and scalable structure

📈 Production Readiness

This project is:

Scalable

Reusable

Maintainable

Environment-configurable

The architecture supports integration into CI/CD pipelines and enterprise automation workflows.

📜 License

MIT License
