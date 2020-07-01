# Linux笔记

​				——Linux命令

## groupadd

#### 说明

​		创建一个新的组

#### 语法

​		groupadd Option 组名

| Option |                             说明                             |
| :----: | :----------------------------------------------------------: |
|   -g   | 这个值必须是唯一的，除非使用-o选项。但必须是非负的。默认值是使用大于或等于GID_MIN的最小值，并且大于每个其他组 |
|   -K   | 重写/etc/login.defs默认值（GID_MIN，GID_MAX和其他）。可以指定多个K选项。示例：-K GID_MIN=100 –K GID_MAX=499。注意：-K GID_MIN=10,GID_MAX=499不能工作 |
|   -o   |               此选项允许添加一个非唯一的GID值                |
|   -p   |           为新组使用此加密过的密码。默认为禁用密码           |
|   -r   | 创建一个系统组。新的系统组数字标识符在SYS_GID_MIN到SYS_GID_MAX范围内选择，定义在login.defs中而不是GID_MIN到GID_MAX |
|   -R   |            将修改应用到CHROOT_DIR目录，并使用配置            |
|   -f   | 如果指定的组已经存在，此选项将失明了仅以成功状态退出。当与-g一起使用，并且指定的GID_MIN已经存在时，选择另一个唯一的GID（即-g关闭） |

#### 退出值

- 0 成功
- 2 无效的命令语法
- 3 给了选项一个无效的参数
- 4 GID不唯一（没有使用-o）
- 9 组名不唯一
- 10 无法更新组文件

![chgrp](image/groupadd.png)

###### 注：组名最长32个字符

###### /etc/group 组账户信息、/etc/gshadow 安全组账户信息、/etc/login.defs Shadow密码套件配置