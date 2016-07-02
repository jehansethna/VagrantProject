# VagrantProject
Automated Vagrant box for development purposes.

#### **Vagrant Setup** 
##### System Requirements & Setup
In order to use, the vagrant based development environments must meet the following requirements.

* **4GB RAM** or greater.
* Supports hardware virtualization extensions.

In order to use this environment perform the following steps.

1. Enable the Virtualization Extensions in your BIOS.
2. Install [VirtualBox]
3. Install Vagrant
4. Clone this repository using wither SSH or HTTPS.
5. `cd VagrantProject`
6. `vagrant up`
7. `vagrant ssh` if you are running Linux, otherwise use putty.

Login credentials are as follows:
* **User:** vagrant
* **Password:** vagrant

#### **Environment Details**

The environment contains the following software,

1. Python-pip
2. Boto3 for AWS development purposes.
3. Chef
4. Tmux
5. GIT



