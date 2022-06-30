# Ansible in the project

"As part of the project, you need to create an Ansible Playbook that will provision the environment that your application needs to run."

## Run nginx server (For the reverse Proxy)

- restart
  service / systemd
- configuration
  template / copy
- install
  apt

## Jenkins

- install
  - Provided Script
    shell
  - More manual install in Jenkins Advanced
    user
    command / copy / community.general.sudoers
    apt
    shell / get_url
    copy / systemd daemon-reload, start, enable

## GCP instances

ansible-doc google.cloud.gcp_compute_instance

## Docker

### Docker engine
- install
  write a play 
  - curl to bash
    shell
  - Manual install 
    apt  apt_key apt_repository

### Docker Compose
community.docker.docker_compose
shell / command

### Docker Swarm
community.docker.docker_swarm
shell / command