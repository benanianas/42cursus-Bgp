
# Virtual Machine Setup

### Install docker
```
sudo apt update
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu  $(lsb_release -cs)  stable"
sudo apt update
sudo apt-get install docker-ce
```

### Install gns3

```
sudo add-apt-repository ppa:gns3/ppa
sudo apt update                                
sudo apt install gns3-gui gns3-server
```

### Add user to these groups

```
sudo usermod -a -G docker $(whoami)
sudo usermod -a -G ubridge $(whoami)
sudo usermod -a -G libvirt $(whoami)
sudo usermod -a -G kvm $(whoami)
sudo usermod -a -G wireshark $(whoami)
```
# Part 1

### Pull Images

```
docker pull frrouting/frr
docker pull alpine
```

`And run commands in folder p1`


# Notes

```
ip addr add 10.12.12.69/16 dev enp0s3
#ospf
#ospfd
#bgp
#bgpd

#is-is
#is-isd

#evpn
#evpet
#vxlan(vni) / vlan(id) 
```
