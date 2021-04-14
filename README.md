# みなさん、こんにちは！

该环境用于我自己的 Lua 环境搭建，感兴趣的老铁也可以 fork 后 build 一下



Lua 官网：[https://www.lua.org/](https://www.lua.org/)



分为 `windows` 和 `linux`

### Windows

可以从 [http://joedf.ahkscript.org/LuaBuilds/](http://joedf.ahkscript.org/LuaBuilds/) 下载已经编译好的 Lua ，解压后，将解压目录添加到环境变量中去，若只是临时使用，在命令行使用 `set path` 指令 (**只在当前终端有效**)

```shell
set path                           # 查看环境变量
set path =                         # 清空环境变量(用不着)
set path = X:\some_path            # 修改环境变量(用不着)
set path = X:\some_path;%path%     # 添加环境变量(就这个)
```

在本仓库`windows`目录下，提供了 `srlua-5.4.3_Win64_bin.zip` 和 `lua-5.4.3_Win64_bin.zip`，可`git`下来直接用

P.S. `srlua` 用于生成可执行 `lua` 脚本

### Linux

根据官方[指南](https://www.lua.org/download.html)

```shell
curl -R -O http://www.lua.org/ftp/lua-5.4.3.tar.gz
tar zxf lua-5.4.3.tar.gz
cd lua-5.4.3
make all test
```

在本仓库`linux`目录下，提供了`lua-5.4.3.tar.gz` 文件，可直接使用

