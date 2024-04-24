---
title: How to Install Astronvim 
pubDate: 2024-04-23
categories: ['tutorial']
tags: ['vim']
description: ''
---


### How to Install AstroNvim inside Ubuntu WSL

![](https://cdn-images-1.medium.com/max/800/1*uuejACZNmTv6Lj7QS0H9Dw.png)

AstroNvim Homepage

### **What is AstroNvim?**

AstroNvim is one of the best Neovim distributions. It is a configuration designed to make Neovim function like an IDE.

There are essential dependencies for AstroNvim, including Nerd Fonts, Neovim, and NodeJS.

**Nerd Fonts**

Nerd Fonts is patched font that include icons. It is used in AstroNvim to display icons and symbols, enhancing its visual appeal.

**Neovim**

Neovim is a fork of Vim aim at improving developer experience and facilitating plugin integration.

**NodeJS**

NodeJS is a JavaScript runtime environment and needed for certain language servers, especially Javascript and Typescript.

### **Hands-on**

1.  Update & upgrade system

    sudo apt update && sudo apt upgrade -y

2. Setting Nerd Fonts

Install Nerd Fonts inside your Windows, and configure it on Terminal.

![](https://cdn-images-1.medium.com/max/800/1*pvfsmha7MCNeVfGyz4HYuw.png)

Setup Nerd Font on Terminal

3. Install zsh

It considered as optional, but it connected with another setup.

    sudo apt install zsh

4. Install oh-my-zsh

One of the best Zsh configuration.

    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

5. Install Node Version Manager (NVM)

    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | zsh

6. Install latest Node.js

    nvm install —lts

7. Install Neovim PPA Repo

    sudo add-apt-repository ppa:neovim-ppa/unstable

8. Install Neovim

    sudo apt install neovim

9. Clone the AstroNvim Repo

    git clone --depth 1 https://github.com/AstroNvim/template ~/.config/nvim   rm -rf ~/.config/nvim/.git   nvim

Voila!

![](https://cdn-images-1.medium.com/max/800/1*-yH6KROCofJz81uOtOcdjA.png)
