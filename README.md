## Install ansible

#### Update packages
```sh
sudo apt-get update
```

#### This package will give us to easily work with PPA
```sh
sudo apt-get install software-properties-common
```

#### Add ansible into PPA
```sh
sudo apt-add-repository ppa:ansible/ansible
```

#### Install ansible 
```sh
sudo apt-get update
sudo apt-get install ansible
```

#### Check Version
```sh
ansible --version
```


## Automatic Configuration Management tool to install necessary softwares.

### Note:
<p> Before run ansible playbook, make sure ansible get installed and double checked the version</p>

<p> This playbook install all the default necessary softwares in a stage or production in a matter of an hour to make developers 
work easily to concentrate on application side</p>

### Basic syntax to run ansible playbook

```sh
ansible-playbook -K -i $hosts_file.hosts $playbook.yml
```

### Below is our example
```sh
ansible-playbook -K -i all-in-one.hosts all-in-one.yml
```

### Library
<p> If you face any error while installing nginx please install below command to install missing dependencies </p>

```sh
sudo apt-get install libpcre3 libpcre3-dev zlib1g zlib1g-dev libssl-dev
```

#### Tutorial link
```sh
https://www.exoscale.com/syslog/setup-private-docker-registry/

https://blog.docker.com/2013/07/how-to-use-your-own-registry/

https://github.com/docker/docker.github.io/blob/master/registry/deploying.md
```
