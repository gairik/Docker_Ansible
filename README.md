# Docker_Ansible
Create your own Ansible lab with Docker containers

#### Run the client using 
```
 docker run -d -it ansible_client bash
```
#### Add docker IPs to the /etc/ansible/hosts file
```
docker inspect bridge
```
get the ips and then vim the file /etc/ansible/hosts file

```
[web]
172.17.0.4
172.17.0.3
172.17.0.2
```
