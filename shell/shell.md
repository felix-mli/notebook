**获取当前脚本的绝对路径**

```shell
#!/bin/bash
path=`realpath $0`
echo $path
```

**获取脚本所在目录路径的命令**

```shell
#!/bin/bash
path=`realpath $0`
echo $path
a=`dirname $path`
echo $a
```

**停止 udev 的执行队列**

```shell
# 停止 udev 的执行队列可以防止 udev 自动检测和配置设备。这在你需要手动加载或卸载内核模块时特别有用。
udevadm control --stop-exec-queue
```

**echo**

```shell
# -n 取消末尾的回车符
echo -n hello world
# -e 解析单双引号里面的转义字符
echo -e "Hello\nWorld"
```

