# CS 310: Final Project

## Summary

For a fictional company named Craftroast, we used Ansible for the declarative confiuration, created and deployed a Bagisto E-Commerce site with docker, created and configured developer and admin accounts, configure SSH access, and Grafana for monitoring.

## Usage

To run the project configuration:

1.	Install Ansible on the control machine
        sudo apt install ansible

2.	Run the Bagisto Docker setup playbook
    This pulls and starts the official Bagisto E-Commerce container:
        ansible-playbook bagisto_setup.yml

3.	Run the developer user setup playbook
    This creates the two required developer accounts and generates SSH keys:
        ansible-playbook developer_users.yml
4.	Verify the setup by navigating to CraftRoast’s site in a browser:
        http://localhost:8082

## Resources
Anasible docs for docker:
https://docs.ansible.com/projects/ansible/latest/collections/community/docker/docsite/scenario_guide.html#envvar-DOCKER_TLS

Anasible docs for accounts:
https://docs.ansible.com/projects/ansible/latest/collections/ansible/builtin/user_module.html


Grafana Docker image:
https://hub.docker.com/r/grafana/grafana

Bagisto docs:
https://devdocs.bagisto.com/getting-started/installation.html#🐳-docker-installation
    