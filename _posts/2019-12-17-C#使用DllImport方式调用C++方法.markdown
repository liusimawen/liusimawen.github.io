---
layout: post
title:  "C#使用DllImport方式调用C++方法"
date:   2019-12-17
categories: jekyll update
---
# 数据类型对应
    C++                 C#   <br>
   const char*         string <br>
   入参 char *         stringbuilder <br>
   返回值 char*        IntPtr <br>
    long (4字节)         int32(4字节)   ---这条非常容易忽略，但是非常重要 <br>
# EntryPoint获取
可使用dumpbin工具，通过dumpbin -exports [dllpath]方式查看