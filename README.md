### README for DjangoSetup Ansible Project

---

# DjangoSetup

This project automates the setup of a Django project using Ansible. The playbook installs required packages, sets up a Python virtual environment, installs dependencies, creates the project directory, and runs the Django server.

## Project Structure

```
ansible-django-setup/
├── setup_django.yml
└── README.md
```

## Prerequisites

- Ubuntu 20.04 or later
- Python 3.6 or later
- Ansible 2.9 or later
- sudo privileges

## Installation Instructions

### Step 1: Update System Packages

Update your package list to ensure all packages are up to date.

```bash
sudo apt update
```

### Step 2: Install Ansible

Install Ansible using the package manager.

```bash
sudo apt install ansible -y
```

### Step 3: Create Project Directory

Create a directory for the Ansible project and navigate into it.

```bash
mkdir ~/ansible-django-setup
cd ~/ansible-django-setup
```

### Step 4: Create the Ansible Playbook

Create a new file named `setup_django.yml` and add the following content:


### Step 5: Ensure Requirements File Exists

Make sure the `requirements.txt` file exists in the specified path (`/home/goodarzi/Documents/ansible1/simpl8/requirements.txt`). This file should list all the Python packages your Django project depends on.

### Step 6: Run the Ansible Playbook

Execute the Ansible playbook to set up the Django project.

```bash
ansible-playbook setup_django.yml
```

This command will perform the following actions:
1. Install required system packages.
2. Create a Python virtual environment.
3. Install the Python packages specified in `requirements.txt`.
4. Create the Django project directory.
5. Run the Django server.

## Usage

Once the playbook has been successfully executed, your Django project will be set up and the development server will be running. You can access the server in your web browser at `http://localhost:8000`.

## Troubleshooting

- Ensure you have `sudo` privileges, as some tasks require elevated permissions.
- Verify the paths specified in the playbook are correct.
- Check the `requirements.txt` file for any missing dependencies or incorrect package versions.

## License

This project is licensed under the MIT License.

---

By following these instructions, you should be able to automate the setup of your Django project using Ansible efficiently. If you encounter any issues, refer to the troubleshooting section or consult Ansible and Django documentation for further assistance. 🚀🔧