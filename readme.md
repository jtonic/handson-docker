The handson-docker is about learing the docker - containerization technology.
=


#### Goals:
1. Docker
    1. Learn the dockers CLI commands
    1. Learn the docker-machine CLI commands
    1. The anatomy of the Dockerfile
    1. docker-compose commands
    1. docker-compose.yml file 
    1. docker swarm - cluster of dockers
    1. docker mvn plugin
1. Ansible
1. Vagrant
1. sh scripting
1. ubuntu commands

#### Tasks
1. **[V]** Ansible for installing a nginx web server in a vagrant vm
    1. **[V]** no security configuration for nginx
    1. **[V]** TLS configuration (443 => 8443)
1. Manually build a docker image
1. Building a docker command with build command
1. Tag a built image
1. Create the docker-compose.yml for oracle java8/db/wl


####Notes
1. To generate the TLS certificate and key files use the following command (tested on Mac OS)

        $ openssl req -x509 -nodes -days 3650 -newkey rsa:2048 \
            -subj   /CN=localhost \
            -keyout ansible/playbook/files/nginx.key \
            -out    ansible/playbook/files/nginx.crt

