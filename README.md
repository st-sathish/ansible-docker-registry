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