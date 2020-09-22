# UOS Config


## Externel Monitor

```bash
sudo  apt  autoremove  -y  nvidia-*
sudo  apt  install  -y  nvidia-driver  nvidia-smi  nvidia-settings  deepin-nvidia-prime
```

Link: [亲测可用，目前最简单的笔记本双显卡I+N驱动方案 ](https://bbs.chinauos.com/post/1196?id=1196&type_id=0&from=4&forum_name=%E6%A1%8C%E9%9D%A2%E4%B8%AA%E4%BA%BA%E7%89%88&subject=%E4%BA%B2%E6%B5%8B%E5%8F%AF%E7%94%A8%EF%BC%8C%E7%9B%AE%E5%89%8D%E6%9C%80%E7%AE%80%E5%8D%95%E7%9A%84%E7%AC%94%E8%AE%B0%E6%9C%AC%E5%8F%8C%E6%98%BE%E5%8D%A1I%20N%E9%A9%B1%E5%8A%A8%E6%96%B9%E6%A1%88)

## Latest Emacs
```bash
sudo apt-get install software-properties-common
sudo apt-get update

wget -q http://emacs.ganneff.de/apt.key -O- | sudo apt-key add
sudo add-apt-repository "deb http://emacs.ganneff.de/ buster main"
sudo apt-get update
sudo apt-get install emacs-snapshot
```

## ZSH
```bash
sh github/sync/zsh/ohmyzsh-install.sh

# font
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf

# p10k
git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
# Set ZSH_THEME="powerlevel10k/powerlevel10k" in ~/.zshrc.
```

## z.lua

see `linux-zshrc`


## packages

* tree
* htop
* lua5.3
* docker-ce
* hugo


## kubernetes

### Docker

```bash
sudo usermod -aG docker $USER
# logout now

# edit /etc/docker/daemon.json
```

```json
{
        "data-root": "/opt/docker"
}

```

```bash
sudo systemctl restart docker
```

### kubeadm

```bash
sudo apt-get update && sudo apt-get install -y apt-transport-https curl
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
cat <<EOF | sudo tee /etc/apt/sources.list.d/kubernetes.list
deb https://apt.kubernetes.io/ kubernetes-xenial main
EOF
sudo apt-get update
sudo apt-get install -y kubelet kubeadm kubectl
sudo apt-mark hold kubelet kubeadm kubectl
```

add `kubectl` to zsh plugin list 

### installation

```bash
kubeadm config images pull  --image-repository=registry.cn-hangzhou.aliyuncs.com/google_containers
# global proxy
kubeadm init --pod-network-cidr=10.244.0.0/16
## DO: remove no cidr
kubectl apply -f <cilium-file>
```
