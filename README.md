# 说明

fork [marktext/marktext](https://github.com/marktext/marktext)的develop分支，用[chinayangxiaowei/marktext-chinese-language-pack](https://github.com/chinayangxiaowei/marktext-chinese-language-pack)的替换来进行汉化

# 如何构建

先装好依赖  

```
sudo apt update  
sudo apt install build-essential clang flex bison g++ gawk gcc-multilib g++-multilib gettext git libncurses-dev libssl-dev python3-distutils rsync unzip zlib1g-dev file wget
```

Python 版本大于v3.6 

Node.js 版本大于v16 但小于v17，可以装16.20  

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

# 编译好的文件

| 名称                       | SHA256                                                           |
| ------------------------ | ---------------------------------------------------------------- |
| marktext-amd64.deb       | 2475670984D9B1877C36C9C5FBAAFD780779C1C96C6E9C7AA9B840A70FA3B60D |
| marktext-ia32-win.zip    | 1D038D58BDE4CF71C2B5487D90F36D3392E6526AA204A467F689B9BDC554946F |
| marktext-setup.exe       | D354F3E31F9F4597B4CA1705000C008ECD17DA5D21585EC7353FC7D982914166 |
| marktext-x64.tar.gz      | 3D60F4DCA46D56AB94BBF96018DE9B921008712D16849EE8009AC5CF7F2849BC |
| marktext-x64-win.zip     | CB8239070B085A623747A5D1F06F31C4123F4AA7944A01210D016BB49B4E4E3A |
| marktext-x86_64.AppImage | 16ED79896768E67995FA62DF552056C918F2DDDC4F896CBEECF953E7AD9B3DBE |
| marktext-x86_64.rpm      |                                                                  |
