# Linux笔记

​				——Linux命令

## init

#### 说明

​		手动输入命令执行相关操作

#### 语法

​		init Number

| Number |                  说明                   |
| :----: | :-------------------------------------: |
|   0    | 停机（initdefault不能为0,否则不停关机） |
|   1    |               单用户模式                |
|   2    |          多用户，没有NFS不联网          |
|   3    |      完全多用户模式(标准的运行级)       |
|   4    |                没有用到                 |
|   5    |      X11 （xwindow) 图形化界面模式      |
|   6    | 重启（initdefault不能为6,否则不停重启） |

![chgrp](image/init.png)