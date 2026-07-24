# 🚀 Ansible Playbook Collection

A collection of beginner-friendly Ansible playbooks demonstrating core automation concepts such as package installation, variables, loops, handlers, conditional execution, and task organization.

This repository is designed for learning Ansible fundamentals and can be used as a reference for automating Linux server configuration.

---

## 📂 Project Structure

```text
Ansible-Playbooks/
│── file.yml
│── handler.yml
│── install-package.yml
│── multipackage.yml
│── os_condition.yml
│── variable.yml
│── with_item.yml
└── README.md
```

---

## 📖 Playbook Description

| Playbook | Description |
|----------|-------------|

| **file.yml** | Creates, modifies, or manages files and directories using the Ansible `file` module. |
| **handler.yml** | Demonstrates Ansible handlers, which execute only when notified by a task. |
| **install-package.yml** | Installs a single package using the appropriate package manager. |
| **multipackage.yml** | Installs multiple packages in a single playbook. |
| **os_condition.yml** | Executes tasks based on the target operating system using conditional statements. |
| **variable.yml** | Shows how to define and use variables in Ansible playbooks. |
| **with_item.yml** | Demonstrates looping through multiple items using `with_items`. |

---

## ✨ Features

- ✅ Package Installation Automation
- ✅ Variables in Ansible
- ✅ Handlers and Notifications
- ✅ Conditional Task Execution
- ✅ Looping with `with_items`
- ✅ File and Directory Management
- ✅ Beginner-Friendly Examples

---

## 🛠️ Prerequisites

Before running these playbooks, ensure you have:

- Ansible installed
- Linux control node
- SSH access to managed hosts
- Inventory file configured

Verify Ansible installation:

```bash
ansible --version
```

---

## 📄 Inventory Example

```ini
[web]
192.168.1.10

[db]
192.168.1.20
```

Or

```ini
[servers]
server1 ansible_host=192.168.1.10
server2 ansible_host=192.168.1.11
```

---

## ▶️ Running Playbooks

Run any playbook using:

```bash
ansible-playbook -i inventory file.yml
```

Examples:

```bash
ansible-playbook -i inventory install-package.yml

ansible-playbook -i inventory multipackage.yml

ansible-playbook -i inventory variable.yml

ansible-playbook -i inventory os_condition.yml

ansible-playbook -i inventory handler.yml

ansible-playbook -i inventory with_item.yml
```

---

## 📚 Ansible Concepts Covered

- Playbooks
- Tasks
- Variables
- Loops
- Handlers
- Conditions (`when`)
- File Module
- Package Module
- Inventory Management

---

## 📸 Expected Output

Example:

```text
PLAY [Install Packages]

TASK [Install Apache]
changed: [server1]

TASK [Start Apache]
changed: [server1]

PLAY RECAP

server1 : ok=2 changed=2 unreachable=0 failed=0
```

---

## 🎯 Learning Objectives

By exploring these playbooks, you will learn how to:

- Automate Linux administration tasks
- Install and manage software packages
- Use variables effectively
- Execute tasks conditionally
- Restart services using handlers
- Work with loops
- Manage files and directories

---

## 📌 Technologies Used

- Ansible
- YAML
- Linux
- SSH

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push your branch.
5. Open a Pull Request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

## **Shubham Rasal**

- 💼 DevOps Engineer
- ☁️ AWS Certified Solutions Architect – Associate
- 🐧 Linux | Docker | Terraform | Jenkins | Git | Ansible

---

⭐ If you found this repository helpful, don't forget to **Star** it on GitHub!
