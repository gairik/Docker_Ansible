# Docker_Ansible
Create your own Ansible lab with Docker containers

#### Build the master using
```
cd Anisble_master
docker build . -t ansible_master
```

#### Build the client using
```
cd Anisble_client
docker build . -t ansible_client
```

#### Run the client using 
```
 docker run -d -it ansible_client bash
```
#### Add docker IPs to the /etc/ansible/hosts file
```
docker inspect bridge
```
get the ips and then vim the file /etc/ansible/hosts file and add the end of file

```
[web]
172.17.0.4
172.17.0.3
172.17.0.2
```
#### ~/.vimrc
```
set tabstop=2 shiftwidth=2 expandtab cursorcolumn
```
