# setup-ml-infrastructure

This repository will help you to set up all needed infrastructure for end-to-end ML project

## Prerequisites

If you use Linux, you can install ansible via `sudo apt install -y ansible`
For MacOS you can install ansible via python `pip3 install ansible`

## Usage

1. Create file `hosts` on the root of project and fill up it with all hosts you want to set up.

    Example for K8S setup:

    ```text
    [masters]
    master ansible_host=<hostIP_1> ansible_user=root
    [workers]
    worker1 ansible_host=<hostIP_2> ansible_user=root
    worker2 ansible_host=<hostIP_3> ansible_user=root
    [all:vars]
    ansible_python_interpreter=/usr/bin/python3
    ```

> :warning:
>The minimal working hosts file should contain **[masters]** section and **[all:vars]** section from example

2. 

## TODO list

- [ ] nginx as a reverse proxy
- [ ] Jupyter HUB + conda
- [ ] MLFlow
- [ ] Airflow
- [ ] Hadoop File System
- [ ] Spark + Pyspark
- [ ] K8S
