# 说明 
本项目基于 [janeczku/calibre-web](https://github.com/janeczku/calibre-web)

致谢！

# Calibre-Web
致力于打造一个更好使用的电子书系统

[![License](https://img.shields.io/github/license/janeczku/calibre-web?style=flat-square)](https://github.com/janeczku/calibre-web/blob/master/LICENSE)
![Commit Activity](https://img.shields.io/github/commit-activity/w/janeczku/calibre-web?logo=github&style=flat-square&label=commits)
[![All Releases](https://img.shields.io/github/downloads/janeczku/calibre-web/total?logo=github&style=flat-square)](https://github.com/janeczku/calibre-web/releases)
[![PyPI](https://img.shields.io/pypi/v/calibreweb?logo=pypi&logoColor=fff&style=flat-square)](https://pypi.org/project/calibreweb/)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/calibreweb?logo=pypi&logoColor=fff&style=flat-square)](https://pypi.org/project/calibreweb/)
[![Discord](https://img.shields.io/discord/838810113564344381?label=Discord&logo=discord&style=flat-square)](https://discord.gg/h2VsJ2NEfB)

## 功能

- 中文支持更友好
- 

## 安装

#### 通过 pip 命令安装(推荐)
1. Create a virtual environment for Calibre-Web to avoid conflicts with existing Python dependencies
2. Install Calibre-Web via pip: `pip install calibreweb` (or `pip3` depending on your OS/distro)
3. Install optional features via pip as needed, see [this page](https://github.com/janeczku/calibre-web/wiki/Dependencies-in-Calibre-Web-Linux-and-Windows) for details
4. Start Calibre-Web by typing `cps`

*Note: Raspberry Pi OS users may encounter issues during installation. If so, please update pip (`./venv/bin/python3 -m pip install --upgrade pip`) and/or install cargo (`sudo apt install cargo`) before retrying the installation.*

Refer to the Wiki for additional installation examples: [manual installation](https://github.com/janeczku/calibre-web/wiki/Manual-installation), [Linux Mint](https://github.com/janeczku/calibre-web/wiki/How-To:-Install-Calibre-Web-in-Linux-Mint-19-or-20), [Cloud Provider](https://github.com/janeczku/calibre-web/wiki/How-To:-Install-Calibre-Web-on-a-Cloud-Provider).

## 运行

1. Open your browser and navigate to `http://localhost:8083` or `http://localhost:8083/opds` for the OPDS catalog
2. Log in with the default admin credentials
3. If you don't have a Calibre database, you can use [this database](https://github.com/janeczku/calibre-web/raw/master/library/metadata.db) (move it out of the Calibre-Web folder to prevent overwriting during updates)
4. Set `Location of Calibre database` to the path of the folder containing your Calibre library (metadata.db) and click "Save"
5. Optionally, use Google Drive to host your Calibre library by following the [Google Drive integration guide](https://github.com/janeczku/calibre-web/wiki/G-Drive-Setup#using-google-drive-integration)
6. Configure your Calibre-Web instance via the admin page, referring to the [Basic Configuration](https://github.com/janeczku/calibre-web/wiki/Configuration#basic-configuration) and [UI Configuration](https://github.com/janeczku/calibre-web/wiki/Configuration#ui-configuration) guides

#### 默认用户名和密码:
- **Username:** admin
- **Password:** admin123

## 环境需求

- Python 3.5+
- [Imagemagick](https://imagemagick.org/script/download.php) for cover extraction from EPUBs (Windows users may need to install [Ghostscript](https://ghostscript.com/releases/gsdnld.html) for PDF cover extraction)
- Optional: [Calibre desktop program](https://calibre-ebook.com/download) for on-the-fly conversion and metadata editing (set "calibre's converter tool" path on the setup page)
- Optional: [Kepubify tool](https://github.com/pgaskin/kepubify/releases/latest) for Kobo device support (place the binary in `/opt/kepubify` on Linux or `C:\Program Files\kepubify` on Windows)

