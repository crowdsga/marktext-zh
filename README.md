# 说明

fork marktext/marktext的develop分支，用chinayangxiaowei/marktext-chinese-language-pack的替换来进行汉化

# 如何构建

先装好依赖  

```
sudo apt update  
sudo apt install build-essential clang flex bison g++ gawk gcc-multilib g++-multilib gettext git libncurses-dev libssl-dev python3-distutils rsync unzip zlib1g-dev file wget
```

Python 版本大于v3.6 Node.js 版本大于v16 但小于v17，可以装16.20  

nodejs 可以通过nvm进行版本控制

安装yarn

```
npm install yarn
```

下载项目

```
git https://github.com/crowdsga/marktext-zh.git
cd marktext
```

安装项目依赖

```
yarn install
```

安装ts依赖

```
 yarn add ts-node 
 yarn add typescript 
```

设置语言 

```
windows：              set lang=zh-cn  
mac or linux:         export lang=zh-cn 
```

编译 yarn build

```
yarn run build 
```

（RPM包还需要安装依赖，sudo apt-get install rpm）

 编译好的程序在build 


