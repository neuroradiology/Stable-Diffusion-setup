# [Tutorial] Complete Guide to ControlNet for Stable Diffusion Automatic1111 Web UI Extension
* How to download and install Stable Diffusion Automatic1111 Web UI
* How to download and install ControlNet extension for Automatic1111 Web UI
* How to use ControlNet features such as Canny, Tiling, 

## Full tutorial video link for this guide will be added once published

## Prerequisites

**Full tutorial for python and git installation with venv**

https://youtu.be/B5U7LJOvH6g

**Download and install Python 3.10.x (3.10.6, 3.10.9, 3.10.11) and git**

3.10.9 > https://www.python.org/ftp/python/3.10.9/python-3.10.9-amd64.exe

git > https://git-scm.com/downloads

## Installation

Bat script that automatically installs Automatic1111 Web UI
* https://www.patreon.com/posts/auto-installer-84773926

Bat script that automatically installs ControlNet and downloads all models
* https://www.patreon.com/posts/automatic-and-84875387

All Patreon posts index
* https://github.com/FurkanGozukara/Stable-Diffusion/blob/main/Patreon-Posts-Index.md

Our Discord channel for help (free - 3000+ members) 
* https://discord.com/servers/software-engineering-courses-secourses-772774097734074388

### Step 1

Install Automatic1111 Web UI

Clone the official repo into any folder you want to install. If you are not expert clone into C drive
* https://github.com/AUTOMATIC1111/stable-diffusion-webui

```
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
```

Edit webui-user.bat file and add this argument :
```
set COMMANDLINE_ARGS=--xformers
```
You can find all arguments for below link
* https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Command-Line-Arguments-and-Settings

Double click and start webui-user.bat for fresh clean install

### Step 2
Updating xformers to latest. Start a new cmd inside web ui folder and type below code. All shown in the tutorial video so watch it
```
call .\venv\Scripts\activate.bat
pip install xformers==dev
```
Look for latest xformers and install it e.g. All shown in the tutorial video so watch it
```
pip install xformers== 0.0.21.dev551
```
### Step 3
Clone main ControlNet repo (https://github.com/Mikubill/sd-webui-controlnet) into this folder : ```\automatic_web_ui\extensions```
```
git clone https://github.com/Mikubill/sd-webui-controlnet
```
From below link download the models you wish to use and put them inside ```automatic_web_ui\extensions\sd-webui-controlnet\models folder```
* https://huggingface.co/lllyasviel/ControlNet-v1-1/tree/main

Restart Automatic1111 Web UI and you will be ready to use

Follow the video for more information and detailed how to steps

### Used Versions

ControlNet Commit 
```
git checkout 5fc952793aa97bdd0078574b3be8bc98e1fcf2cd
```
Automatic1111 Web UI Commit
```
git checkout baf6946e06249c5af9851c60171692c44ef633e0
```
Pip Freeze Below
