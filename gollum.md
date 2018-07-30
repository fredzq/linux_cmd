参考：
    https://github.com/gollum/gollum/wiki/Installation

sudo apt-get install ruby ruby-dev make zlib1g-dev libicu-dev build-essential git cmake
sudo apt-get ruby-bundler
二进制文件安装
    sudo gem install gollum

源码安装
下载源码
    git clone https://github.com/gollum/gollum
    cd gollum
修改安装源
    修改源码目录下的Gemfile文件
    改为  source 'https://ruby.taobao.org/'
执行安装
    bundle install
运行
    bundle exec bin/gollum