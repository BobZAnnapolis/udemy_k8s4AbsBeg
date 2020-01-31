VirtualBox
	copy down Ubuntu, install
	create user, enable sudo

on VMs
========
 hostname
 ifconfig
 cd
 sudo apt-get install -y apt-utils net-tools apt-transport-https ca-certificates vim curl software-properties-common
 echo "colorscheme desert" >.vimrc
 vim .bashrc  -- add aliases
 . .bashrc
 sudo apt-get purge openssh-server
 sudo snap install docker.io {docker} 
 sudo apt-get install -y openssh-server docker_compose 
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
 sudo usermod -a -G docker rjzawis
 reboot
 service ssh status
 ping www.google.com
 apt list --upgradable
 sudo apt upgrade -y
 sudo apt-get update -y
 docker run hello-world
 docker images
 docker ps

kube-apiserver on MASTER
kubelet on WORKERS - this is how they 'talk'

etcd on MASTER
controller, scheduler on MASTER

kubectl cmd used to deploy 'run' containers, get 'cluster-info', get 'nodes' info

