# Linux Fundamentals with Vagrant

This repository demonstrates basic Linux system administration tasks using a Vagrant virtual machine running Ubuntu. Below are the tasks, screenshots, and explanations.

## Task 1: Set Up a Vagrant Server
I initialized a Vagrant virtual machine with Ubuntu 22.04 and connected to it via SSH. The screenshot shows the `vagrant init`, `vagrant up`, and `vagrant ssh` commands, confirming successful login to the VM.

![Vagrant Initialization and Login](images/screenshot1_vagrant_init.png)

## Task 2: Explore the Linux File System
I created a folder structure `/home/vagrant/projects/devops` using the `mkdir -p` command. The `ls -R` command shows the created folders. This helps organize project files in a logical structure.

![Folder Structure](screenshot2_folder_structure.png)

## Task 3: Manage File Permissions and Ownership
I created a file `example.txt` and changed its permissions to `600` (owner read/write only) using `chmod`. I also changed its ownership to `root` using `chown`. The screenshot shows the commands and the final `ls -l` output, where permissions (`-rw-------`) mean only the owner can access it, and ownership shows `root root`.

![Permissions and Ownership](screenshot3_permissions.png)

## Task 4: Install and Configure a Package
I installed the `tree` package using `apt` after updating the package list. The `tree --version` command confirms the installation. The screenshot shows the installation process and version output.

![Package Installation](screenshot4_package_install.png)

## Task 5: Test Remote Connectivity
I used `ping -c 4 google.com` to test network connectivity. The screenshot shows the ping results, with response times indicating the VM is connected to the internet. This is useful for verifying network access.

![Ping Result](screenshot5_ping.png)