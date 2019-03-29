[![CircleCI](https://circleci.com/gh/FastCGI-Archives/fcgi2.svg?style=svg)](https://circleci.com/gh/FastCGI-Archives/fcgi2)

FastCGI Developer's Kit
-----------------------

Copyright (c) 1996 Open Market, Inc.
See the file "[LICENSE.TERMS](LICENSE.TERMS)" for information on usage and redistribution
of this file, and for a DISCLAIMER OF ALL WARRANTIES.

Documentations
--------------

- [FastCGI Developer's Kit Documentations](http://fastcgi-archives.github.io/fcgi2/doc/overview.html)

Basic Directions
----------------
ARM-Linux:
    ./autogen.sh  #生成Makefile文件
    ./configure --host=交叉编译工具前缀名 --prefix=安装路径
    sudo -i       #为避免找不到交叉编译器，切换权限
    make
    make install

    一种编译方式举例：
   arm-linux-gcc  main.c -o main -L /opt/fcgi-arm/lib -lfcgi

Unix:

    ./autogen.sh
    ./configure
    make
    make install

Win32:

    nmake -f Makefile.nt

    (or use the MSVC++ project files in the Win32 directory)


CHANGES
-------

This repository are a fork from the original fastcgi sdk from [FastCGI.com](https://fastcgi-archives.github.io/) that are now down, the new place of FastCGI.com are at https://fastcgi-archives.github.io/.

For more detail regarding changes, please consult the [git log available](https://github.com/FastCGI-Archives/fcgi2/commits/master). 

