# Linux笔记

​				——Linux命令

## groupmod

#### 说明

​		用于更改群组识别码或名称

#### 语法

​		groupmod [-g <群组识别码> <-o>] [-n <新群组名称>] [群组名称]

| Option |             说明             |
| :----: | :--------------------------: |
|   -g   |   设置将要使用的群组识别码   |
|   -n   |    设置将要使用的群组名称    |
|   -o   | 此选项允许重复使用群组识别码 |

![chgrp](image/groupmod.png)

###### 注：组名最长32个字符