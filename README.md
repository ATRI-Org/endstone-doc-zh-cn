<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/EndstoneMC/endstone/releases">
    <img src="https://static.wikia.nocookie.net/minecraft_gamepedia/images/4/43/End_Stone_JE3_BE2.png" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Endstone</h3>

<p align="center">
   使用 Python 和 C++ 等编程语言为基岩版专用服务器编写插件？没问题！
</p>

[![Windows](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml)
[![Linux](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml)
[![Documentation](https://github.com/EndstoneMC/endstone/actions/workflows/docs.yml/badge.svg)](https://endstone.dev/)
[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.21.3%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
[![PyPI - Version](https://img.shields.io/pypi/v/endstone)](https://pypi.org/project/endstone)
[![Python](https://img.shields.io/pypi/pyversions/endstone?logo=python&logoColor=white)](https://www.python.org/)
[![GitHub License](https://img.shields.io/github/license/endstonemc/endstone)](LICENSE)
[![Codacy Badge](https://img.shields.io/codacy/grade/8877402fc70b40f5a8c4b325d890e3f7?logo=codacy)](https://app.codacy.com/gh/EndstoneMC/endstone/dashboard)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![Discord](https://img.shields.io/discord/1230982180742631457?logo=discord&logoColor=white&color=5865F2)](https://discord.gg/xxgPuc2XN9)

</div>

## 📄 目录

- [📖 介绍](#-介绍-)
- [🎯 特征](#-特征-)
- [🛠️ 开始](#%EF%B8%8F-开始-)
- [🌟 插件](#-插件-)
- [🙌 贡献代码](#-贡献代码-)
- [🎫 License](#-license-)

## 📖 介绍 [🔝](#-目录-)

我们非常高兴地宣布 Endstone 项目的启动。Endstone 为 Bedrock 专用服务器提供插件 API，支持
Python 和 C++ 语言。这使开发人员能够利用各种特性和功能增强 Bedrock 专用服务器。
功能。

## 🎯 特征 [🔝](#-目录-)

- **跨平台**: 我们同时支持 Windows 和 Linux 平台,目前,我们是唯一一个原生支持这两个平台的 BDS 服务器软件,无需Wine.
- **Feature-rich**: All up-to-date Minecraft features are at your fingertips! We make sure to keep Endstone aligned with
  the latest game updates.
- **Hassle-free**: Ready to use right out of the box. Start the Endstone server with just one line of command. No extra
  tools required.
- **High-level API**: We provide a high-level friendly API akin to Bukkit plugin developers. Save yourself the hassle of
  dealing with the dot-and-cross of the low-level system API and hooks, we've done the difficult part for you!
- **Starter-friendly**: No C++ knowledge? No problem! Craft your plugins using Python, your favourite.
- **Performance-in-mind**: For the performance savants, you can, of course, write (or rewrite) your plugins in C++ to
  squeeze out
  every bit of performance.

## 🛠️ 开始 [🔝](#-目录-)

开始使用前，请确认您使用的是以下兼容操作系统之一：

- Windows 10 10.0.15063 或更高版本
- Windows Server 2016 或更高版本
- Debian 11 或更高版本
- Ubuntu 20.04 或更高版本

还请确保您的系统已安装**Python 3.9 或更高版本**。

有几种安装 Endstone 的方法：

### 🐍 PyPi

[![Wheel](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)

可以使用 pip 直接从 PyPi 安装 Endstone。打开终端，执行以下命令安装
并启动
Endstone 服务器：

``shell
pip install endstone
endstone
``

### 🐳 Docker

[![Docker](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml)
[![Docker - Pulls](https://img.shields.io/docker/pulls/endstone/endstone)](https://hub.docker.com/r/endstone/endstone)
[![Docker-映像大小](https://img.shields.io/docker/image-size/endstone/endstone)](https://hub.docker.com/r/endstone/endstone)

要试用最新 Docker 映像中的 Endstone，请使用以下命令：

``shell
docker pull endstone/endstone
docker run --rm -it -p 19132:19132/udp endstone/endstone
``

这将拉取最新的 Endstone 映像，并在终端中交互运行。

### 🔨 从源代码本地构建

对于高级用户，你可以从源代码本地构建 Endstone。

首先，克隆版本库：

``shell
git clone https://github.com/EndstoneMC/endstone.git
cd endstone
``

然后，你就可以构建轮子并安装到本地机器上了：

``shell
pip install .
endstone
``

**请注意，从源代码构建需要在系统中安装工具链。**

|                                  | Windows                       | Linux    |
|----------------------------------|-------------------------------|----------|
| Build System                     | CMake                         | CMake    |
| Generator                        | Ninja                         | Ninja    |
| C/C++ Compiler **(Recommended)** | MSVC 193 (Visual Studio 2022) | Clang 15 |
| C/C++ Compiler (Minimum)         | MSVC 191 (Visual Studio 2017) | Clang 5  |
| Standard Library                 | MSVC STL                      | libc++   |

## 🌟 插件 [🔝](#-目录-)

目前，Endstone 项目正在积极开发中，我们邀请您查看我们的路线图。在您等待期间
何不偷看一下我们的示例插件，它们展示了插件 API 的友好性。如果您有
有使用 Bukkit 的经验，就会发现 API 的使用特别直观：

- [C++ Example Plugin](https://github.com/EndstoneMC/cpp-plugin-template)
- [Python Example Plugin](https://github.com/EndstoneMC/python-plugin-template)

| Milestone                                | Duration   | Core | Since  |
|------------------------------------------|------------|------|--------|
| **🔌 Plugin Loader**                     | 1-2 months | ✅    | v0.1.0 |
| **⌨️ Command System**                    | 2-3 months | ✅    | v0.2.0 |
| **🔐 Permission System**                 | 2-3 months | ✅    | v0.3.0 |
| **🎈 Event System**                      | 2-3 months | ✅    | v0.4.0 |
| **🖼 Form & Scoreboard API**             | 1-2 months | 🚧   |        |
| **👤 Player & Actor API**                | 2-3 months | 🚧   |        |
| **🔩 Item API**                          | 1-2 months | ⏳    |        |
| **🧱 Block API**                         | 1-2 months | ⏳    |        |
| **📦 Inventory API**                     | 2-3 months | ⏳    |        |
| **⭐ Advanced Features & Refinements**    | 4-6 months | ⏳    |        |
| **🔬 Beta Testing & Community Feedback** | 3 months   | ⏳    |        |
| **🚀 Official Release & Support**        | -          | ⏳    |        |

这里有一个图例为您提供指导：

- ✅: 任务已完成。呜呼！🎉
- 🚧: 任务正在进行中。我们正在执行！💪
- ⏳: 下一个任务。激动人心的事情即将发生！🌠

## 🙌 贡献代码 [🔝]（#-目录-）

我们热烈欢迎大家为 Endstone 项目献计献策！如果您热衷于使用 Python 和 C# 来增强 Bedrock 专用
服务器，并对如何改进 Endstone 有想法，您可以通过以下几种方式作出贡献：

### 报告错误

如果您在使用 Endstone 时遇到任何错误，请在我们的
我们的 GitHub 存储库中打开一个 [issue]() 问题。确保包含错误的详细描述和重现步骤。

### 提交拉取请求

我们感谢您的代码贡献。如果您修复了一个错误或实现了一个新功能，请提交拉取请求！
请确保您的代码遵循我们的编码标准，并尽可能包含测试。

## 🎫 License [🔝](#-目录-)

The Endstone project is licensed under the [Apache-2.0 license](LICENSE).
