# Self Hosted Nginx For Static Websites

This playbook allows you to self-host an Nginx proxy with podman containers and systemd Quadlets.

It was tested on Fedora 41.

The playbook will create a base directory where the nginx configuration is stored.

To support multiple Nginx instances each instance has a directory with the instance name inside the
base directory. The instance directory contains the nginx.conf file and a public directory which contains the website's static content. 

References:
- https://gideonwolfe.com/posts/sysadmin/hugonginx/