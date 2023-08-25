# ansible

Developed and implemented an automation project using Ansible to streamline the configuration and management of
UDP load balancing with HAproxystats in a production environment. The project aimed to enhance system performance,
ensure high availability, and provide real-time monitoring of load-balancing activities.

In the previous version of this project, in ansible script (site.yaml), the Python Flask service is initiated as a systemd service instead of running through the shell. Running through systemd is always preferred in a production environment over the shell.
