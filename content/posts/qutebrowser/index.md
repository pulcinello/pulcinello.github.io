+++
title = 'qutebrowser'
date = 2025-05-01T14:27:13+08:00
draft = true
+++

自Chrome转向Manifest V3后，我转投Firefox已有一段时间。作为主力浏览器，Firefox于我已无可挑剔。但我一直想要一个轻量的浏览器以作备用，在某台旧机器上，这一需求尤为迫切。

在软件仓库内一顿翻找后，[qutebrowser](https://qutebrowser.org/)——这个市占率可能不足0.1%的浏览器，成了我最后的选择。

## 为何选择qutebrowser

qutebrowser基于[QtWebEngine](https://wiki.qt.io/QtWebEngine)（而QtWebEngine则基于Chromium），支持三大桌面操作系统。该浏览器始于2013年，是瑞士人Florian Bruhin在大学时期开展的个人项目，如今依旧仰赖他业余时间的开发和社区的捐助。受限于社区规模与资源，qutebrowser至今没有插件系统，在标签页分组等功能上也有所欠缺。甚至在书签/历史记录管理这样基础的功能上，qutebrowser的实现也相当简陋。然而，对比主流浏览器，qutebrowser亦有其独到之处，主要在于：

- 键盘驱动，支持vim式的模态操作。
- 极简的界面，提供沉浸式的网页浏览体验。
- 以python脚本作为配置文件，方便多平台管理。

诚然，Firefox靠着CSS主题、[Tridactyl](https://github.com/tridactyl/tridactyl)这样的插件也能达成类似的效果，对应功能上的结合却远不如qutebrowser那般紧密，版本更迭时引起的配置/插件失效的问题亦时有发生。

也可直接跳到文末，我提供了一份配置样例，供有兴趣者入门使用。

## qutebrowser初印象

对Emacs用户而言，其hackable之姿可谓昭然若揭

## 像配置vim一样配置你的浏览器
```
qutebrowser
├── autoconfig.yml
├── bookmarks
│   └── urls
├── config.py
├── configs
│   ├── aliases.py
│   ├── interface.py
│   ├── keymaps.py
│   ├── options.py
│   └── theme.py
├── greasemonkey
├── qsettings
│   └── QtProject.conf
├── quickmarks
└── userscripts
    ├── gh-read-all.js
    ├── localhost
    ├── markdownit
    ├── open_or_search
    ├── qr
    └── readability
```

按键的功能随模式的变化而变化。

In qutebrowser, all keybindings are mapped to commands.

config-write-py

config-diff

use [glance](https://github.com/glanceapp/glance) as homepage

config.unbind

## 使用技巧与建议

### 广告过滤
[cjxlist](https://github.com/cjx82630/cjxlist)
[xinggsf/Adblock-Plus-Rule: uBlock Origin 乘风广告过滤规则](https://github.com/xinggsf/Adblock-Plus-Rule)

### 油猴

### mpv

### 使用用户脚本扩充浏览器功能


## 参考阅读

- 我的配置样例
