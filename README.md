
# Part 1: GNS3 configuration with Docker

### Install docker
```
sudo apt update
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu  $(lsb_release -cs)  stable"
sudo apt update
sudo apt-get install docker-ce

sudo usermod -a -G docker $(whoami)
```

### Pull Images

```
docker pull frrouting/frr

docker pull alpine
```

```
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