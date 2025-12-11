# Bagisto Setup Test

This playbook is used to verify that the Bagisto container can be successfully pulled and started on the local system.

Use this playbook before running other deployments or configuration tasks.

## Tasks

#### Pull Image

Pulls the Bagisto Docker image (webkul/bagisto:2.3.6) to ensure it is available locally.

### Start Container

Starts the Bagisto container using the pulled image and maps port 8082 on the host to port 80 inside the container.

### Show Output

Displays debug output to confirm the container started correctly.