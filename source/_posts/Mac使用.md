---
title: Mac使用
date: 2017-04-08 22:15:56
tags: Mac
---

## 前言
对于一直在用Windows开发的我来说直接上手Mac有点麻烦且又要学习使用Mac，当然最大的阻碍还是不习惯，但是这是3、4天前的感受，短短几天时间我就深深体会到了Mac的优雅强大，工作开发起来简直不要太爽，要离不开的感觉，有种以前用windows开发都在浪费时间的感觉，哈哈，不过Mac对程序员还真是友好，故此记录下Mac的一些东西，随便写写玩了

## 常用软件
- 编程
    + XCode
    + homebrew  
    + oh my zsh
    + VSCode
    + CheatSheet 
    + Chrome
- 其他
    + QQ
    + 微信
    + AppCleaner
    + the unarchiver
    + istat menus

### homebrew

#### 常用命令
```
brew search [TEXT|/REGEX/]
brew (info|home|options) [FORMULA...]
brew install FORMULA...
brew update
brew upgrade [FORMULA...]
brew uninstall FORMULA...
brew list [FORMULA...]

brew update && brew cask install react-native-debugger
```

#### 安装列表
install和cask install的区别
> brew主要用来下载一些不带界面的命令行下的工具和第三方库来进行二次开发，brew cask主要用来下载一些带界面的应用软件，下载好后会自动安装，并能在mac中直接运行使用
> brew install curl可以安装curl第三方库，这样你在开发时就可以使用它的库来进行开发
> brew cask install chrome可以安装谷歌浏览器应用程序，可直接运行brew偏管理第三方库和命令行工具方面的东东brew cask可以看作是苹果官方app store的补充

- install
    + git
    + git-flow
    + nginx
    + node
- cask install
    + java
    + react-native-debugger

## 重装系统
比Windows要操作简单，主要介绍U盘重装

- 准备工作
    + 备份
    + U盘
    + 下载OS
        * AppSotre上下载即可，下载完后别安装
        * 如从网盘下载的，请将解压后获得的 "Install OS X Yosemite.app"(显示为"安装 OS X Yosemite.app")移动到「应用程序」文件夹里面
- 格式化U盘
    + 应用程序 -> 实用工具 -> 磁盘工具
    + 将U盘「抹掉」(格式化)
        * Mac OS X 扩展（日志式）格式
        * GUID 分区图方案
        * 命名为「Sierra」(注意：这个盘符名称将会与后面的命令一一对应，如果你改了这盘符的名字，必须保证后面的命令里的名称也要一致)
- 输入终端命令开始制作启动盘
    + 应用程序 -> 实用工具 -> 终端
    + 将下面的一段命令复制并粘贴进去
    ```
    sudo /Applications/Install\ macOS\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Sierra --applicationpath /Applications/Install\ macOS\ Sierra.app --nointeraction
    ```
    + 回车并执行该命令，输入管理员密码开始制作过程，等待Done
- U盘启动安装Mac OS X
    + 关机
    + 按下电源键开机，当听到“噹”的一声时，按住 Option 键不放，直到出现启动菜单选项
    + 格式化系统盘
    + 退回U盘重装

## 操作
- 隐藏文件设置
    + 显示
        `defaults write com.apple.finder AppleShowAllFiles -bool true`
    + 隐藏
        `defaults write com.apple.finder AppleShowAllFiles -bool false`

## 其他
http://www.iplaysoft.com/osx-yosemite-usb-install-drive.html
http://freemacsoft.net//
http://reactide.io/

## 参考链接
https://www.zhihu.com/question/22624898/answer/105234217



