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


ssh-keygen -t rsa -C "email@"

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
