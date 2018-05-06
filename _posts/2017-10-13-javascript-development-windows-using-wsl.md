---
layout: article
title:  "JavaScript Development in Windows using Windows Subsystem for Linux (WSL)"
date: 2017-10-13 14:29:05 +0800
updated_date: 2017-10-13 14:29:05 +0800
group: "blog"
comments: true
---
Below is the collection of tools I use in my JavaScript Development life.

## Visual Studio Code
<hr class='divider--fade' />

![vscode](/img/js-dev-wsl/vscode_4.png)

[VS Code](https://code.visualstudio.com/) is an editor created by [Microsoft](https://github.com/Microsoft/vscode), and it looks great. And I've been using it since I started coding in AngularJS.

Aside from the minimalist look it offers, there are other features of VS Code that I enjoy using.

Like the [Git Integration](https://code.visualstudio.com/docs/editor/versioncontrol), but it also supports other version controls. With this, you'll be able to see some indications of your changes: added, modified, or deleted a line in your code.

You can see all files that you modified by pressing `Ctrl+Shift+G` and you can also compare your current file to the original one by selecting a file in the list.

VS Code also offers an [integrated terminal](https://code.visualstudio.com/docs/editor/integrated-terminal), thought I don't use it cause I prefer to use a separate terminal. You can change what terminal you want as default. In Windows, it can be `cmd`, `git bash` or even the `bash on windows`.

### Color Scheme & Font

The theme I have is called [An Old Hope Theme](https://marketplace.visualstudio.com/items?itemName=dustinsanders.an-old-hope-theme-vscode). And the font [Fira Code](https://github.com/tonsky/FiraCode) with it's cool looking equal and arrow symbols.

![fira code](/img/js-dev-wsl/fira_code_3.png)

<!-- ### VS Code Extensions
* [An Old Hope Theme](https://marketplace.visualstudio.com/items?itemName=dustinsanders.an-old-hope-theme-vscode) - color scheme
* [Beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify) - for beautifying SCSS
* [Bookmarks](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks) - allows for bookmarking lines
* [copy-json-path](https://marketplace.visualstudio.com/items?itemName=nidu.copy-json-path) - we're using i18n's written in `JSON` and object paths get too long copy manually
* [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - for linting JS
* [Git History (git log)](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) - compare current workspace file to a file in a commit
* [Insert Date String](https://marketplace.visualstudio.com/items?itemName=jsynowiec.vscode-insertdatestring) - Insert a datetime string formrat for blog purposes (jekyll)
* [JSCS Linting](https://marketplace.visualstudio.com/items?itemName=ms-vscode.jscs) - one of my projects is using JSCS. Nothing I can do about it ¯\_(ツ)_/¯
* [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) - sync VS Code settings, extensions, and stuff
* [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) - tooling for Vue.js
* [vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons) - icon pack
* [WakaTime](https://marketplace.visualstudio.com/items?itemName=WakaTime.vscode-wakatime) - tracking coding time -->

## HyperJS
<hr class='divider--fade' />

![hyperjs](/img/js-dev-wsl/hyperjs.png)

The terminal I'm using is the [Windows Subsystem for Linux](https://msdn.microsoft.com/en-us/commandline/wsl/about) inside [Hyper.js](https://hyper.is/). The shell is `zsh` and [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) as the framework.

It's a cross platform terminal emulator so it would work in Mac and Linux.

<!-- ### Packages
* [zsh]() - as the shell
* [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) - zsh framework
* [Git]() - Git
* [hub]() - extend Git
* [nvm]() - manage node versions -->
## Opera
<hr class='divider--fade' />

![opera](/img/js-dev-wsl/opera_1.png)

My browser of choice. It's based on Chromium. I like the built-in `adblocker` and the "picture in picture" feature when playing videos. It also has Messenger and WhatsApp on the sidebar integrated.

---
I will be integrating Disqus soon so you can leave some inquiries if you have.

I will write an in-depth look of each one, like the extensions I used, or some tips and tricks that I do.
