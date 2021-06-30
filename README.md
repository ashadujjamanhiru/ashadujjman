### Docker Engine Install on CentOS-8 ###
------------------------------------------------

Step1: Uninstall old versions
-----------------------------

$ sudo yum remove docker \
                   docker-client \
                   docker-client-latest \
                   docker-common \
                   docker-latest \
                   docker-latest-logrotate \
                   docker-logrotate \
                   docker-engine

Step2: Installation methods
----------------------------

   1. Install using the repository
   -------------------------------

$ sudo yum install -y yum-utils
$ sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo

--------### Install Docker Engine ###-----------
### Install the latest version of Docker Engine and containerd ###
---------------------------------------------------------------
 # sudo yum install docker-ce docker-ce-cli containerd.io

######## Start Docker ##########
----------------------------------

$ sudo systemctl start docker

### Verify that Docker Engine is installed correctly by running the hello-world image ###
-----------------------------------------------------------------------------------------
$ sudo docker run hello-world

######## Check Docker Container ##########
------------------------------------------

$ docker ps  (Show running container)
$ docker ps  (Show All container)
