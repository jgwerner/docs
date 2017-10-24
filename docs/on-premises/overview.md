## Environment

These instructions are to allow developers and customers install 3Blades stack on-premises. It has been tested with AWS EC2 Ubuntu 16.04 instances but should work with other ones as well. A few notes about how this installation works:

* Uses Ansible Playbook to download, install, and configure artifacts, such as Docker engine.
* Docker images are pulled from DockerHub.
* All images communicate with each other using Docker links.
* All services and data stores run in separate containers.

You could do all of this with docker-compose. As a matter of fact, the Ansible playbook does use docker-compose to launch and link services. However, we enhance docker-compose with Ansible to automate dependency setup, seed database, and provide additional configuration options.

## Services

The services run when installing and launching the 3Blades server are (in alphabetical order):

  * API based on Django
  * Celery, run with Django
  * Events service using custom Docker image
  * Traefik reverse proxy server
  * PostgresSQL database
  * RabbitMQ message broker
  * Redis cache
  * Search with Elasticsearch backend
