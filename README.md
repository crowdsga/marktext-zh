# 说明
fork marktext/marktext的develop分支，用chinayangxiaowei/marktext-chinese-language-pack的替换来进行汉化
# 如何构建
先装好依赖 \
sudo apt update \
sudo apt install build-essential clang flex bison g++ gawk \
gcc-multilib g++-multilib gettext git libncurses-dev libssl-dev \
python3-distutils rsync unzip zlib1g-dev file wget

Python 版本大于v3.6 
Node.js 版本大于v16 但小于v17，可以装16.20 
npm install yarn

git clone https://github.com/marktext/marktext.git

cd marktext

安装项目依赖 yarn install 
开始编译 yarn run build
（RPM包还需要安装依赖，sudo apt-get install rpm）
编译好的程序在build
