---
comments: true
---

# 开始

Endstone为Bedrock Dedicated Servers(官方服务器软件)提供了一个强大的插件API.如果你熟悉Python, 你可以使用 [`pip`](#使用pip安装) 来安装EndStone. 相反,
你可以使用 [`docker`](#使用docker).

## 安装

### 环境 <small>optional</small> { #环境 data-toc-label="环境" }

我们建议你安装 [虚拟环境].
如果您在虚拟环境中,您安装或升级的任何包
将是当地的环境.如果你遇到问题,你可以
只需删除并重新创建环境.建立起来很简单:

-   使用该命令创建一个虚拟环境:

    ```
    python3 -m venv venv
    ```

-   使用以下命令激活环境:

    === ":fontawesome-brands-windows: Windows"

        ``` sh
        . venv/Scripts/activate
        ```

    === ":fontawesome-brands-linux: Linux"

        ``` sh
        . venv/bin/activate
        ```


    你的终端应该在启动之前打印 `(venv)`.

-   使用以下命令退出环境:

    ```
    deactivate
    ```

### 使用pip安装 <small>recommended</small> { #使用pip安装 data-toc-label="使用pip安装" }

Endstone被发布成了一个 [Python package] 而且可以用 `pip`安装, 在[虚拟环境](#environment) 
安装则需要最后一步.打开终端执行以下命令来安装:

=== "Latest"

    ``` sh
    pip install endstone
    ```

### 使用docker

官方的 [Docker image] 是一个很好的方式来安装和使用EndStone. 使用以下命令拉取docker镜像(国内请自备魔法或者镜像:

=== "Latest"

    ```
    docker pull endstone/endstone
    ```

[Python package]: https://pypi.org/project/endstone/

[虚拟环境]: https://realpython.com/what-is-pip/#using-pip-in-a-python-virtual-environment

[Docker image]: https://hub.docker.com/r/endstone/endstone/