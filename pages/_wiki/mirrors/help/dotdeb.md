---
---

# （旧）Dotdeb 镜像使用帮助

Dotdeb 已经停止维护，帮助不再更新。

---

### 使用说明

1\. 添加下面两行到 `/etc/apt/sources.list` ，并将 `jessie` 替换为自己所使用的版本名称：

     deb http://mirrors.ustc.edu.cn/dotdeb jessie all
     deb-src http://mirrors.ustc.edu.cn/dotdeb jessie all

2\. 可选项：

- 如果你想在 Debian Squeeze 上安装 PHP5.4 的话，再添加下面这两行：

  deb http://mirrors.ustc.edu.cn/dotdeb squeeze-php54 all
  deb-src http://mirrors.ustc.edu.cn/dotdeb squeeze-php54 all

- 如果你想在 Debian Wheezy 上安装未启用 Zend Thread Safety 的 PHP5.6 的话，再添加下面这两行：

  deb http://mirrors.ustc.edu.cn/dotdeb wheezy-php56 all
  deb-src http://mirrors.ustc.edu.cn/dotdeb wheezy-php56 all

- 如果你想在 Debian Wheezy 上安装启用 Zend Thread Safety 的 PHP5.6 的话，再添加下面这两行：

  deb http://mirrors.ustc.edu.cn/dotdeb wheezy-php56-zts all
  deb-src http://mirrors.ustc.edu.cn/dotdeb wheezy-php56-zts all

- 如果你想在 Debian Wheezy 上安装 PHP5.5 的话，再添加下面这两行：

  deb http://mirrors.ustc.edu.cn/dotdeb wheezy-php55 all
  deb-src http://mirrors.ustc.edu.cn/dotdeb wheezy-php55 all

3\. 然后导入合适的 GnuPG key

     wget https://www.dotdeb.org/dotdeb.gpg
     cat dotdeb.gpg | sudo apt-key add -

4\. 运行 apt-get update

### 相关链接

- 官方主页：<http://www.dotdeb.org/>

- 镜像列表：<http://www.dotdeb.org/mirrors/>

- 官方源使用指南：<https://www.dotdeb.org/instructions/>
