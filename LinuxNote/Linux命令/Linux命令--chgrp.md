# Linux笔记

​				——Linux命令

## chgrp

#### 说明

​		改变文件的组所有权，切换文件所属组，设置方式采用群组名称或群组识别码皆可

#### 语法

​		chgrp -Option --help --version 所属群组 文件或目录

|        Option         |                        说明                        |
| :-------------------: | :------------------------------------------------: |
|    -R(--recursive)    |  递归处理，将指定目录下的所有文件及子目录一并处理  |
| -h(--no-dereference)  | 只对符号连接的文件作修改，而不更动其他任何相关文件 |
|     -v(--verbose)     |                  显示指令执行过程                  |
|     -c(--changes)     |        效果类似"-v"参数，但仅回报更改的部分        |
| -f(--quiet或--silent) |                   不显示错误信息                   |
|        --help         |                      在线帮助                      |
|       --version       |                    显示版本信息                    |

![chgrp](image/chgrp.png)