# 使用python学习写爬虫

本项目主要讲述一些基本爬虫程序的编写，主要包含环境搭建、常用数据抓取库（`urllib`、`requests`、`pyspider`）用法

html解析库`pyquery`、`beautifulsoup` 常见用法

Python版本：`Python3.6.3`


## 环境配置

将本项目拉取到`root`目录下

### docker环境

如果熟悉docker，可以自己编译docker镜像，在[Lesson-1](Lesson-1)文件夹下，执行命令

    docker build -t python-spider-env .

编译完成后，用如下命令启动

    docker run -itd -p 8888:8888 -p 5000:5000 -p 8080:8080 -v /root/Learn-Use-Python-Write-Spider:/data python-spider-env

启动后可在浏览器里访问`http://localhost:8888`打开jupyter，默认登陆密码为: `88888888`


### 系统安装

如果不熟悉docker，可以在`Lesson-1`目录下执行`pip install -r requirements.txt` 来安装所需扩展包

使用 `jupyter-notebook` 启动 jupyter，在默认的终端会提示

    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://localhost:8888/?token=...
请复制完整带有完整`token`的连接地址打开，直接启动没有修改密码，只能靠token登陆

## 课程内容

* [环境配置](Lesson-1)