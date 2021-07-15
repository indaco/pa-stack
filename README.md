# Process Automation Stack

## Fully automated provisioned Process Automation platform

This project provides docker images of the latest [Camunda](https://camunda.com/) Platform CE as Process Automation platform and [Portainer](https://www.portainer.io/).

Although both Camunda and Portainer provide Docker images, the rational behind this project is to have a standalone environment, configured with what is needed only then, I can be up and running in zero time.

For that reason, my choice is to provide it with Vagrant and Ansible using a docker-compose service.

## Prerequisites

The following software have to be installed on you machine

- VirtualBox
- Vagrant
- Ansible
- Git (optional)

Follow the relative guides on how to install those based on your OS.

## How-To

### Step 1 - Clone the project repository

First thing to be done is to get the source code for this project from GitHub. If you have `git` installed on your machine, just do a `git clone` otherwise go the [project page](https://github.com/indaco/pa-stack) and "Download`

```bash
git clone https://github.com/indaco/pa-stack.git
```

### Step 2 - Provisioning the software stack as docker-compose

Move into the `provisioning` folder and run the provisioning of the VM with Vagrant.

```bash
cd pa-stack/provisioning
vagrant up
```

### Step 3 - Access to Camunda

Once the Ansible playbook finish the setup:

**Camunda** is accessible at `http://localhost:8080`. Default credentials, as stated on the [Camunda Platform Docker Images repository](https://github.com/camunda/docker-camunda-bpm-platform) for admin access to the webapps are:

- Username: demo
- Password: demo

### Step 4 - Access to Portainer

Portainer is accessible at `http://localhost:9000`
