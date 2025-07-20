install
=======

Shell scripts for macOS & Debian Linux system installation

This project is part of a series of setup tools designed to help users quickly build a clean and consistent development environment:

1. [mengbo/splite.zsh](https://github.com/mengbo/splite.zsh): A lightweight and modular ZSH configuration framework 
2. [mengbo/splite.vim](https://github.com/mengbo/splite.vim): A modular Vim configuration framework based on Vundle
3. [mengbo/install](https://github.com/mengbo/install): Shell scripts for macOS & Debian Linux software installation

By setting up Zsh and Vim in the recommended order and installing the required software, you can create a stable and uniform working environment across systems.

## splite.zsh

A lightweight ZSH configuration framework.

This project provides an `./install` script that automatically detects your operating system and runs the corresponding setup scripts from the `install.d` directory. It helps configure your Zsh environment, install essential tools, and set up useful plugins.

Once installation is complete, your `~/.zshrc` will be configured to load individual `.zsh` files from the `~/.zshrc.d/` directory. Each file is responsible for a specific task, making the configuration modular and easy to maintain.

Zsh plugins are stored in the `~/.zsh/` directory and can be updated at any time by running the `./update` script.

In addition, the file `~/.zshrc.d/90profile.zsh` will automatically source all `*.sh` scripts in the `~/.profile.d/` directory, which is useful for applying environment-level settings.

![splite.zsh](https://github.com/mengbo/splite.zsh/raw/main/screenshots/zsh.png)
## splite.vim

A modular Vim configuration framework based on [Vundle](https://github.com/gmarik/vundle).

This project breaks the configuration into multiple small files, with each one dedicated to setting up a single plugin. This structure makes it easier to understand, customize, and maintain your Vim environment—especially for beginners.

To get started, simply run the `./install` script to set up everything you need. Later, you can use the `./update` script to update your plugins.

![splite.vim](https://github.com/mengbo/splite.vim/raw/master/screenshots/macvim.png)

## install

Shell scripts for macOS & Debian Linux software installation. These scripts are designed to simplify the process of setting up software & development tools.
