3安装go－sqlite3

## Mac OS X
1. 通过 Homebrewn 安装：

``` sh
brew install pkgconfig
brew install sqlite3
```

2. 通过 port 安装：
``` sh
sudo port pkgconfig
sudo port install sqlite3
``

3. 如果你在安装后的使用过程遇到 PKG_CONFIG_PATH 有关的问题，可以参考：Mac OS X Lion 安装sqlite3问题。

## Ubuntu
Ubuntu下的安装总是简单到爆，执行以下命令即可：

``` sh
sudo apt-get install pkg-config
sudo apt-get install sqlite3  
sudo apt-get install libsqlite3-dev
```

##Windows

Windows下的安装也非常简单

1. 到 SQLite3 的[下载页面](http://www.sqlite.org/download.html)，下载 Windows 下的预编译包 DLL 的压缩包（sqlite-dll-win32-x86-XXX.zip）。  
2. 然后将里面的 DLL 文件拷贝到 system32 目录下即可。  

另外，如果你已经安装 TMD 版的 GCC 编译器（http://tdm-gcc.tdragon.net/），那么你就不用再安装而可以直接进入下一步！
3. 最后，你就可以通过 go get 命令来安装 go-sqlite3 这个包啦：

``` sh
go get github.com/mattn/go-sqlite3
```

转自 http://sudochina.com/archives/2/2/5.html
