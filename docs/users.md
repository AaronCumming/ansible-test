# Developer User Setup

This playbook is used to create developer accounts on the system and provision them with proper SSH access.
Run this playbook when onboarding new developers or preparing a server for development use.

## Tasks

### Create Developer Users

Creates two users, dev1 and dev2, each with their own home directory.

### Assign to Developer Group

Adds both users to the developer group, ensuring they have the correct permissions.
The group assignment is appended to avoid overwriting existing group membership.

### Generate SSH Keys

Generates a 2048-bit SSH key pair for each user and stores the private key in their respective ~/.ssh/id_rsa locations.
This allows secure, key-based authentication for both developer accounts.