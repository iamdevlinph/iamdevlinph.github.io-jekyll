---
layout: article
title:  "In Depth: Ubuntu on Windows (WSL) using Hyper.js"
date:   2017-10-31 00:13:51 +0800
group: "blog"
comments: true
---
<!-- typical intro section -->
This will expound the Hyper.js section of my [JavaScript Development Environment]({{site.url}}/javascript-development-windows-using-wsl) entry.

## Requirements
* Windows 10 Fall Creators Update (FCU)
* Bash on Ubuntu on Windows (WSL)
* Hyper.js

## Windows 10 FCU
<hr class='divider--fade' />
For this entry, we will be using the latest version of Windows 10 at the time of this writing. To verify if you have the update. Press `WinKey+R` and type `winver`.

![FCU](https://res.cloudinary.com/dfrhytey3/image/upload/v1509382579/in%20depth%20wsl/2017-10-31_003252_1.png)

Verify that you have `Version 1709`.

### Why FCU
Before FCU came, we just have the file `bash.exe` which is the `Ubuntu` itself. During this time, you cannot set a default shell by running `chsh -c /usr/bin/fish|zsh`.

FCU brings the `wsl.exe` file which is very nice. You can now set a default shell on start-up but you'll have to use this file instead of `bash.exe`.

Read more in the [issue](https://github.com/Microsoft/WSL/issues/2199) that I created regarding this.

## Ubuntu on Windows
<hr class='divider--fade' />

[WSL](https://msdn.microsoft.com/en-us/commandline/wsl/about), in a nutshell, is Linux on Windows, but in this case it's Ubuntu. On this point onwards, make sure that you are using the `wsl.exe` file.

![Ubuntu](https://res.cloudinary.com/dfrhytey3/image/upload/v1509383372/in%20depth%20wsl/2017-10-31_010917.png)

Below are some of the packages that I have installed. Before installing, upgrade your Ubuntu first.

{% highlight shell %}
sudo apt-get update
sudo apt-get upgrade
{% endhighlight %}

### ZSH Shell
{% highlight Console %}
#install
sudo apt-get install zsh
#set as default
chsh -c /usr/bin/zsh
#verify
zsh --version
{% endhighlight %}

### [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) ZSH Framework

* [zsh]() - as the shell
* [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) - zsh framework
* [Git]() - Git
* [hub]() - extend Git
* [nvm]() - manage node versions
