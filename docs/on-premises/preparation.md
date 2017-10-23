## Prepare Environments

This guide will step you through setting up your own on-premise version of 3Blades using [Docker](https://www.docker.com/), [Docker-Compose](https://docs.docker.com/compose/) and [Ansible](https://www.ansible.com/).

Before installing and running the 3Blades stack, you need to prepare your local and remote environments. Local environment refers to an instance where you will be running your Ansible playbook. Remote environment refers to an instance where the stack will run.

1. Launch remote instance using these requirements.

  * Ubuntu 16.04 AWS AMI
  * Minimum size: t2.Medium (2 CPU and 4 GB RAM)
  * Security group with the following inbound rules:
  * Open inbound ports: 22 and 80
  * SSH key for remote login
  * Minimum of 30 GB of disk space, more is recommended


!!! note "Supported Environments"
    3Blades should run on any Linux or Windows distribution that supports `Docker` and `Docker Compose`. However, we only officially support AWS EC2 instances with Ubuntu 16.04 at this time.


2. Clone 3Blades on premises repo from GitHub:

    `$ git clone https://github.com/3blades/onpremise`

3. Install `ansible` on your **local** computer. We recommended installing ansible from `virtualenv` environment:

    ```
    $ cd onpremise
    $ virtualenv env
    $ source env/bin/activate
    $pip install ansible
      ```
