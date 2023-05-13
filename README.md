# ansible

In this task, I am working with a basic Python-Flask application called application.py. The application is set up behind an HAproxy, which functions as a load balancer among three development servers known as devA, devB, and devC. To access the entire network, a bastion host is created as an SSH entry point.

The deployment consists of a total of five servers, hosted on City Cloud. The bastion host and HAproxy have floating IP addresses, while the dev servers only have private IP addresses.

To deploy the Flask application on the dev servers and enable load balancing, we utilize the site.yaml Ansible playbook. The playbook installs the application on the dev servers and configures the HAproxy load balancing settings.

For testing purposes, we can use the curl command to send a request to the HAproxy's IP address. The response should include the current time and the hostname of the responding server.
