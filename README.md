## 离线安装requests库

1、下载安装包
1.1 检查requests模块所需依赖包

在可以上网且已经安装python的机器上检查requests模块需要哪些依赖包，如果这些依赖包未安装，直接安装requests也不能使用。

使用命令：pip show requests

发现需要chardet，idna，urllib3，certifi

检查这几个包是否已安装，如果未安装，则也需要手工安装。
1.2 下载requests所需依赖包

在网站 https://www.lfd.uci.edu/~gohlke/pythonlibs 上找到相应的程序，下载并传输至目标机器。


    certifi-2019.9.11-py2.py3-none-any.whl

    chardet-3.0.4-py2.py3-none-any.whl

    idna-2.8-py2.py3-none-any.whl

    requests-2.22.0-py2.py3-none-any.whl

    urllib3-1.25.6-py2.py3-none-any.whl

安装模块

将以上下载的文件传到测试环境。离线装模块。

安装命令为 pip install XXXXX.whl

切记，先安装依赖包，如果直接安装requests，由于有依赖包，还是会去连外网找依赖包。
