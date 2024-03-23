
## docker install debian 12 bookworm
- `echo $(lsb_release -cs)` → bookworm


```shell
# remove previous versions of docker
sudo apt remove docker docker-engine docker.io
snap remove docker

# install prerequisites
sudo apt install -y apt-transport-https ca-certificates curl gnupg2 software-properties-common

# add download.docker.com repository (to /etc/apt/sources.list.d)
# $(lsb_release -cs) --> mantic  [ubuntu 23.10], or --> bookworm [debian 12]
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"
sudo apt update

# install docker 
sudo apt install -y docker-ce

```


- check
```shell
systemctl status docker
docker run -d nginx:1-alpine
```
