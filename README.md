```shell
sudo add-apt-repository ppa:nginx/stable
sudo apt-get update
# 安装 nginx 依赖库
sudo apt-get build-dep nginx
# 同步子模块内容
git submodule update --init --recursive
sudo dpkg-buildpackage -b
sudo dpkg --install nginx-extras_1.10.1-0+precise0_amd64.deb
```
