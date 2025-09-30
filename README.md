# Ansible Practice

This repository contains a set of simple Ansible playbooks for practicing and learning Ansible automation.

## 📂 Project Structure

```
ansible-practice/
│
├── ansible.cfg
├── inventory/
│   └── hosts.ini
├── playbooks/
│   ├── webserver_setup.yml
│   ├── update_packages.yml
│   └── docker_setup.yml
└── README.md
```

---

## 📜 Playbooks

### **1. webserver_setup.yml**
Sets up a basic web server:
- Updates package lists
- Installs Nginx
- Creates a custom `index.html`
- Starts and enables Nginx service

### **2. update_packages.yml**
Updates all packages on the target hosts.

### **3. docker_setup.yml**
Installs Docker, starts the Docker service, and runs a basic Nginx container.

---

## 🚀 How to Use

1. Clone the repository:
```bash
git clone https://github.com/zeynepatceken/ansible-practice.git
cd ansible-practice
```

2. Edit your inventory file (`inventory/hosts.ini`) to match your environment.

3. Run a playbook:
```bash
ansible-playbook playbooks/webserver_setup.yml
```

Replace the playbook name with the one you want to execute.

---

## ⚙ Requirements

- Ansible installed on the control node
- SSH access to target hosts
- Python installed on target hosts

---

## 📌 Notes
- The `ansible.cfg` file is configured to use `inventory/hosts.ini` by default.
- You can disable host key checking by editing `ansible.cfg`.

---

## 📖 Learn More
- [Ansible Documentation](https://docs.ansible.com/)
