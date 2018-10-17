# shell重定向
1.stdin->标准输入->0


| stdin | 标准输入 | 0 |
| --- | --- | --- |
| stdout | 标准输出 | 1 |
| stderr | 标准错误 | 2 |

1. tar xj

-x:解压文件
-j:是否需要解压bz2格式压缩包

###下载示例
```
#!/bin/sh
source="ffmpeg-3.4"
if [ ! -r $source ]
then
    echo "需要下载ffmpeg"
    curl http://ffmpeg.org/releases/${source}.tar.bz2 | tar xj || exit 1
fi

```

2.1. 查看配置

```
./configure
```



