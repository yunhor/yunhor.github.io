sudo apt install fcitx-table-wbpy
Ctrl+Alt+T （默认终端快捷键）打开终端，输入一下命令：
首先更改系统语言环境为英文
export LANG=en_US
然后更改设置
xdg-user-dirs-gtk-update
接着更改回中文语言环境
export LANG=zh_CN.UTF-8
再次执行
xdg-user-dirs-gtk-update
此时再次弹出界面，选择“保留旧的名称”

ssh-keygen -t rsa -C "email"

sudo add-apt-repository ppa:git-core/ppa  
sudo apt-get update  
sudo apt-get install git  
[ -d /usr/share/fonts/opentype ] || sudo mkdir /usr/share/fonts/opentype
sudo git clone --depth 1 --branch release git@github.com:adobe-fonts/source-code-pro.git /usr/share/fonts/opentype/scp
sudo fc-cache -f -v
 
sudo add-apt-repository ppa:ubuntu-elisp/ppa
sudo apt update
sudo apt install emacs-snapshot emacs-snapshot-el

mv ~/.emacs.d ~/Documents/.emacs.d.bak
git clone git@github.com:syl20bnr/spacemacs.git ~/.emacs.d
git checkout --track origin/develop
git pull --rebase

$xz -d ***.tar.xz
$tar -xvf  ***.tar 或

 tar xvJf  ***.tar.xz

sudo mv node-v7.2.0-linux-x64 /opt/node
ln -s /opt/node/bin/node /usr/local/bin/node
ln -s /opt/node/bin/npm /usr/local/bin/npm
node --version

vi ~/.bashrc
export NODE_HOME=/opt/node
export PATH=$PATH:$NODE_HOME/bin
export NODE_PATH=$PATH:$NODE_HOME/lib/node_modules
source ~/.bashrc
设置PATH后，hexo等全局插件运行才不会找不到文件。

tar zvxf go-
mv go- ~/
export GOROOT=$HOME/go
export GOBIN=$GOROOT/bin
# export GOARCH=386
# export GOOS=linux
export GOPATH=$HOME/gorepos
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
go version

vi ~/.emacs.d/init.el
(require 'package)
(setq package-archives '(("gnu"   . "http://elpa.zilongshanren.com/gnu/")
                         ("org"   . "http://elpa.zilongshanren.com/org/")
                         ("melpa" . "http://elpa.zilongshanren.com/melpa/")))
(package-initialize)

go 插件

go get -u -v github.com/nsf/gocode
go get -u -v github.com/rogpeppe/godef
go get -u -v github.com/zmb3/gogetdoc
go get -u -v github.com/golang/lint/golint
go get -u -v github.com/lukehoban/go-outline
go get -u -v sourcegraph.com/sqs/goreturns
go get -u -v golang.org/x/tools/cmd/gorename
go get -u -v github.com/tpng/gopkgs
go get -u -v github.com/newhook/go-symbols
go get -u -v golang.org/x/tools/cmd/guru
go get -u -v github.com/cweill/gotests/...


go get -u github.com/dougm/goflymake

输入下面命令安装pavucontrol：
 #sudo apt install pavucontrol
#pavucontrol
打开选项卡后进行:
"回放"-->系统下面的选项-->内置音频模拟立体声
"输出设备"-->port：headphone(unplugged) 模拟耳机

$ sudo apt-add-repository ppa:ubuntu-elisp/ppa
sudo apt upgrade
sudo apt update
$ sudo apt install emacs-snapshot emacs-snapshot-el

mv ~/.emacs.d ~/.emacs.bak
git clone git@github.com:syl20bnr/spacemacs.git ~/.emacs.d

git checkout --track checkversion/develop

emacs --insecure
安装Source Code Pro 字体
只clone release 分支，很重要，否则字体是乱码,体积也很大
[ -d /usr/share/fonts/opentype ] || sudo mkdir /usr/share/fonts/opentype
git clone --depth 1 --branch release git@github.com:adobe-fonts/source-code-pro.git scp 
sudo mv /usr/share/fonts/opentype/scp
sudo fc-cache -f -v

由于码农的洁癖，老版本必须删除。先查看安装包的名称：
dpkg -S emacs
再全部删除：
apt-get remove emacs24-bin-common emacs24-common emacs24-common-non-dfsg emacs24-nox
gsettings set com.canonical.Unity.Launcher launcher-position Bottom


安装WPS for Linux。下载地址：http://community.wps.cn/download/。选择alpha版deb包。

   Linux 64 bit需要通过安装32 bit的库来获得支持。

   #sudo apt-get install ia32-libs

   但是输入命令后系统提示ia32-libs软件包缺失，需要用lib32ncurses5和lib32z1代替。于是运行

   #sudo apt-get install lib32ncurses5

   #sudo apt-get install lib32z1。

   再dpkg安装程序安装包

   #sudo dpkg -i wps-office_10.1.0.5672~a21_amd64.deb
   提示wps-office 依赖于 libpng12-0；然而：未安装软件包 libpng12-0。该软件包已丢失可用ttf-mscorefonts-installer代替。

   要先运行下面的命令将已安装的wps-office卸载：

   #apt-get -f install

   然后安装依赖关系：

   #sudp apt-get install ttf-mscorefonts-installer

   之后libpng12-0依赖关系还是出错，到下面的地址下载libpng12-0然后安装：

   https://packages.debian.org/zh-cn/wheezy/amd64/libpng12-0/download。

   #sudo dpkg -i libpng12-0_1.2.49-1+deb7u2_amd64.deb

   安装好后到Dash中搜索WPS启动并锁定到启动器，会报错显示缺失字体：

   Symbol，Wingdings，Wingdings2，Wingdings3，MT-Extra

   进入home文件夹，按Ctrl+h显示所有文件夹，查看有没有.fonts文件夹，如果没有就创建一个，然后到网上下载相关字体放入该文件夹中

7.安装vim编辑器。sudo apt-get install vim

8.安装unrar。sudo apt-get install rar unrar

9.删除Amazon的链接：sudo apt-get remove unity-webapps-common

10.安装Git：sudo apt-get install git

11.主题美化，安装Unity Tweak Tool：到Ubuntu软件中心搜索Unity Tweak Tool并安装

### wps for linux 安装出错 
### flyspell 出错的解决方案
    sudo vi /etc/aspell.conf 
    lang en
