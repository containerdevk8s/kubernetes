# Repository configuration

In order to setup the kubernetes repository for your distribution, follow the instructions below.

## Ubuntu distributions

#### Xenial x86_64

```bash
curl -s -L https://$USER.github.io/${REPO}/gpgkey | \
  sudo apt-key add -
curl -s -L https://${USER}.github.io/${REPO}/ubuntu16.04/nvidia-kubernetes.list | \
  sudo tee /etc/apt/sources.list.d/nvidia-kubernetes.list
sudo apt-get update
```
