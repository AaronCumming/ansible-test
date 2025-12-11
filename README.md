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
	•	Bagisto Docker Installation Docs – used to deploy the E-Commerce container
	•	Ansible Module Documentation – used for user creation, SSH key generation, and Docker management (user, docker_image_pull, docker_container)
    