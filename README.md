# Ansible Practice Project – Templates, Fetch, Loops

## 📌 Overview

This project is created to practice core Ansible concepts:

* Jinja2 templates (.j2)
* Template module
* Fetch module
* Loops
* Handlers
* Basic playbook structure

The goal is to simulate real DevOps automation tasks.

---

## 🚀 Features

### ✅ Standardize SELinux Configuration

* Uses Jinja2 template (`selinux.j2`)
* Variables control SELinux mode and type
* Handler triggers reboot if configuration changes

### ✅ Custom MOTD (Message of the Day)

* Dynamic login banner using Jinja2
* Displays:

  * Hostname
  * IP address
  * OS information

### ✅ Backup Important Files

* Uses `fetch` module
* Loops through multiple files:

  * /etc/passwd
  * /etc/shadow
  * /etc/hosts
  * /etc/selinux/config
* Saves backups locally per host

---


## ▶️ Usage

Run playbooks:

ansible-playbook selinux.yml
ansible-playbook motd.yml
ansible-playbook backup.yml

---

## 🧠 Concepts Learned

* Infrastructure automation
* Configuration standardization
* Dynamic templates
* Conditional handlers
* Loop usage in Ansible

---

## 📜 License

This project is licensed under the MIT License.

