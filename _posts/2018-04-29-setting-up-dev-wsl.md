---
layout: article
title:  "Setting Up Development on WSL (or just Linux)"
date:   2018-04-29 00:00:02 +0800
updated_date: 2018-06-22 15:05:50 +0800
group: "blog"
comments: true
---
![alt image](https://i1.wp.com/www.nextofwindows.com/wp-content/uploads/2017/07/image-3.png)
Setting up my development on WSL on Windows 10. If you're just using Linux, you can still follow along, except the installing of WSL part.
## Install Ubuntu WSL
<hr class='divider--fade' />

This guide uses the `Ubuntu flavor`. I haven't tried the others so I'm not sure if the process here can just be copied.

Enable **`Windows Subsystem for Linux`** from `Control Panel > Programs and Features > Turn Windows features on or off`

![enable wsl #2](https://iamdevlinph.github.io/blog/img/setting-up-wsl/enable_wsl.png)

### Get it from the store
![get ubuntu](https://iamdevlinph.github.io/blog/img/setting-up-wsl/get_ubuntu.png)

<span class="read-more">
Read more [here](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/)
</span>

### Copy and Pasting

![wsl-copy-paste](https://iamdevlinph.github.io/blog/img/setting-up-wsl/wsl-copy-paste.jpg)

This is off on init on my case.

### Fonts

Some characters don't work right out of the box. I suggest on using **DejaVu Sans Mono for Powerline**.

You can get it from [here](https://github.com/powerline/fonts/tree/master/DejaVuSansMono) along with [other fonts](https://github.com/powerline/fonts)

![wsl font](https://iamdevlinph.github.io/blog/img/setting-up-wsl/wsl_font.png)

## Git
<hr class='divider--fade' />

### Install Git
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-git.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-16-04)
</span>

### Set your indentity
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=git-identity.sh" type="text/javascript"></script>

### A better git log

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=git-lg.sh" type="text/javascript"></script>

Use it by running `git lg`

Colors: `normal, black, red, green, yellow, blue, magenta, cyan, white`

Attributes: `bold, dim, ul, blink, reverse`

<span class="read-more">
Read more [here](https://stackoverflow.com/a/15458378/4620773)
</span>

### Configure GIT to push on current branch

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=git-push-current-branch.sh" type="text/javascript"></script>

When doing `push` there will be no need to specify to which branch. Just run `git push origin` and it will push to the current branch. This will prevent accidental push to the wrong branch.

<span class="read-more">
Read more [here](https://makandracards.com/makandra/8039-git-how-to-configure-git-to-push-only-your-current-branch)
</span>

### Hub
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-hub.sh" type="text/javascript"></script>

`hub` is a superset of `git` just like how `typescript` is a superset of `javascript`.

With `hub` you can do a pull request without opening the github page by

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=hub-pr.sh" type="text/javascript"></script>

assuming you didn't alias `hub` to `git`.

<span class="read-more">
Read more [here](https://askubuntu.com/a/816541/634714)
</span>

## Generate SSH Keys and Copy to Clipboard
<hr class='divider--fade' />

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=generate-ssh-key-and-copy-clipboard.sh" type="text/javascript"></script>

If you want to get the fingerprint of the one on your machine for comparison

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=ssh-fingerprint.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://stackoverflow.com/a/32130465)
</span>

## ZSH Shell
<hr class='divider--fade' />

### Install ZSH

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-zsh.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)
</span>

### Oh my ZSH

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-oh-my-zsh.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://github.com/robbyrussell/oh-my-zsh#via-curl)
</span>


### Auto suggest

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-zsh-auto-suggest.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://github.com/zsh-users/zsh-autosuggestions#oh-my-zsh)
</span>

### Using plugins in ZSH

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=zshrc-plugins.sh" type="text/javascript"></script>

### Enjoy ZSH
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=use-zsh.sh" type="text/javascript"></script>

## Install Node
<hr class='divider--fade' />

### nvm way (no sudo)
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-nvm.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://github.com/creationix/nvm#installation)
</span>

### Normal Way (will require sudo)
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-node.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://nodesource.com/blog/installing-node-js-tutorial-ubuntu/)
</span>

#### Reinstall Node
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=reinstall-node.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://stackoverflow.com/a/33947181/4620773)
</span>

## Jekyll
<hr class='divider--fade' />

If you want to write a blog using `jekyll`

### Install ruby stuff
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-ruby.sh" type="text/javascript"></script>
### Gem installation directory on user account
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=gem-directory.sh" type="text/javascript"></script>
### Install jekyll
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-jekyll.sh" type="text/javascript"></script>
### Install bundle
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-bundle.sh" type="text/javascript"></script>
### Serve your Jekyll app
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=run-jekyll-app.sh" type="text/javascript"></script>

## tmux
<hr class='divider--fade' />

Install [tmux](https://github.com/tmux/tmux)
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-tmux.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://computingforgeeks.com/linux-tmux-cheat-sheet/)
</span>

### tmux config
Create a tmux configuration file
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=create-tmux.conf.sh" type="text/javascript"></script>

Copy the following configuration and paste inside the `.tmux.conf`
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=tmux.conf.sh" type="text/javascript"></script>

Apply modifications
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=tmux-apply.sh" type="text/javascript"></script>

Start tmux automatically
Add the following line on top of `.zshrc`
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=start-tmux-automatically.sh" type="text/javascript"></script>

### Enjoy tmux
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=start-tmux.sh" type="text/javascript"></script>

### tmux resurrect
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=tmux-resurrect.sh" type="text/javascript"></script>

### tmux key combinations
If you copied the configuration above, below will apply

| Name                   | Command(s)          |
| ---------------------- |-------------------- |
| Split Horizontally     | `Ctrl+a %`          |
| Split Vertically       | `Ctrl+a "`          |
| Close a pane           | `Ctrl+a x`          |
|                        | `exit`              |
| Copy a text selection  | `Shift + Highlight the text + Ctrl+c` |
| Paste a text           | `Shift + Right Click` |
|------------------------|---------------------|
| Save layout for tmux-ressurect | `Ctrl+a, Ctrl+s` |
| Load layout for tmux-resurrect | `Ctrl+a, Ctrl+r` |

`Ctrl+a` is called a **prefix**. You execute it first then followed by the character. The split horizontally command equates to **`Ctrl+a` > `Shift+5`**.

<span class="read-more">
Read more [here](https://lukaszwrobel.pl/blog/tmux-tutorial-split-terminal-windows-easily/) and [here](https://gist.github.com/dimitardanailov/d50d8c872446dc371a7d85bb93832260#file-tmux-conf)
</span>
