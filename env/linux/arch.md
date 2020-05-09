
# Table of Contents

1.  [Arch / Manjaro](#org301ca03)
    1.  [System](#org7efadb1)
    2.  [v2ray](#orgba72400)
    3.  [Wine](#org8a0d4c6)
    4.  [Symbol links](#org592a87b)
    5.  [NutStore](#orgafddf36)
    6.  [Gnome Plugins](#org89a3261)
    7.  [rsync](#org3008848)
    8.  [Softwares](#org368c94e)
    9.  [Cli tools](#org0e6ef97)
    10. [Input Method](#orge6790ac)
    11. [Shell](#orgb648ab9)
    12. [Golang](#org47fcc37)
    13. [Docker](#orgf616a75)
    14. [KeePassXC](#org68bd9b6)
    15. [Kubernetes](#org59b83d0)
    16. [Ref](#org519d9e7)

-   [Index](index)


<a id="org301ca03"></a>

# Arch / Manjaro


<a id="org7efadb1"></a>

## System

-   yay

    pacman -S yay
    
    yay -S v2ray

-   [cannot find strip library required for object file stripping in arch linux](http://hongouru.blogspot.com/2016/04/solved-cannot-find-strip-library.html)
-   pacman color: [pacman color](https://wiki.archlinux.org/index.php/Color_output_in_console#pacman)
-   cn repo: [cn repo](https://github.com/archlinuxcn/repo)
-   sound
    -   声音断了: 重联蓝牙设备
    -   pavucontrol


<a id="orgba72400"></a>

## v2ray

-   v2ray
-   qv2ray
-   v2raya


<a id="org8a0d4c6"></a>

## Wine

1.  fakeroot
2.  [manjaro下体验企业微信](https://zhuanlan.zhihu.com/p/91718319) (!)
3.  [用docker跑企业微信](https://github.com/BoringCat/docker-WXWork)(!)
4.  [Ubuntu 16.04 WINE 企业微信](http://elkpi.com/topics/2018/04/ubuntu-16-04-wine-wxwork.html)
5.  deepin-wine
    -   wechat
        -   [解决Linux下微信透明窗口的问题](https://manateelazycat.github.io/linux/2019/09/29/wechat-transparent-window.html)
        -   add it to .xprofile
        -   [weixin无法粘贴文字图片](https://github.com/countstarlight/deepin-wine-wechat-arch/issues/4)
6.  playonlinux


<a id="org592a87b"></a>

## Symbol links

-   sync/profile -> profile
-   sync/bashrc -> bashrc
-   sync/gitconfig -> gitconfig


<a id="orgafddf36"></a>

## NutStore

-   PT Mono


<a id="org89a3261"></a>

## Gnome Plugins

-   clipboard
-   ScreenShot
-   Weather
-   Sound


<a id="org3008848"></a>

## rsync

-   \`rsync -av &#x2013;del src/ dest\`


<a id="org368c94e"></a>

## Softwares

-   evolution
-   gnome-todo
-   nutstore
-   ao(microsfot todo)
-   deepin-music
-   urxvt
-   sublime
-   chrome
    -   [force dark mode](https://www.laptopmag.com/articles/google-chrome-78-forced-dark-mode)


<a id="org0e6ef97"></a>

## Cli tools

-   vim
-   socat
-   youtube-dl
-   base-devel
-   fakeroot
-   npm
    -   cnpm
    -   [npm配置国内镜像资源+淘宝镜像](https://blog.csdn.net/qq_39207948/article/details/79449633)
-   pip 
    
        mkdir ~/.pip 
        touch ~/.pip/pip.conf
        
        # contents
        [global]
        index-url = https://pypi.tuna.tsinghua.edu.cn/simple


<a id="orge6790ac"></a>

## Input Method

-   ibus ibus-libpinyin
-   ibus-setup: [ibus setup](https://wiki.archlinux.org/index.php/IBus#Installation)


<a id="orgb648ab9"></a>

## Shell

-   bash: [bash-git-promt](https://github.com/magicmonty/bash-git-prompt)
    -   oh-my-bash
-   zsh: ohmyzsh
    -   [best theme](https://github.com/romkatv/powerlevel10k#oh-my-zsh)


<a id="org47fcc37"></a>

## Golang

-   go
-   godef: [godef install](https://packagecontrol.io/packages/Godef)
-   ccat: \`go get -u github.com/jingweno/ccat\`


<a id="orgf616a75"></a>

## Docker

-   docker
-   \`sudo gpasswd -a yayu docker\`
-   image mirror: [azk8s](http://mirror.azk8s.cn/help/quay-proxy-cache.html)
-   quay mirror: [qiniu](https://blog.csdn.net/zsd498537806/article/details/85157560)


<a id="org68bd9b6"></a>

## KeePassXC

-   remove gnome-keyring
-   dark theme: [use qt env to set dask theme](https://github.com/keepassxreboot/keepassxc/issues/804)


<a id="org59b83d0"></a>

## Kubernetes

-   [Installing Kubernetes on ArchLinux](https://gist.github.com/StephenSorriaux/fa07afa57c931c84d1886b08c704acfe)
-   如果systemd文件找不到，找旧版本的kubernetes
-   kubernetes-helm
-   [flannel](https://github.com/coreos/flannel)


<a id="org519d9e7"></a>

## Ref

-   [Manjaro安装，配置，美化指南](http://zryabc.xyz/index.php/archives/257/)
-   [zsh simple config](https://gist.github.com/Pitometsu/5871629a886902816c39)

