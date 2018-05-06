---
layout: article
title:  "Setting Up Development on WSL"
date:   2018-04-29 00:00:02 +0800
updated_date: 2018-05-07 01:26:44 +0800
group: "blog"
comments: true
---
![alt image](https://i1.wp.com/www.nextofwindows.com/wp-content/uploads/2017/07/image-3.png)
Setting up my development on WSL on Windows 10.
## Install WSL
<hr class='divider--fade' />
Open a `command prompt`

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-wsl.sh" type="text/javascript"></script>

If you'll get an error like `0x8007019e` make sure to enable `Windows Subsystem for Linux`

<span class="read-more">
Read more [here](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/)
</span>

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

<span class="read-more">
Read more [here](https://askubuntu.com/a/816541/634714)
</span>

## Generate SSH Keys and Copy to Clipboard
<hr class='divider--fade' />

<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=generate-ssh-key-and-copy-clipboard.sh" type="text/javascript"></script>

## Install Node
<hr class='divider--fade' />
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-node.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://nodesource.com/blog/installing-node-js-tutorial-ubuntu/)
</span>

#### Reinstall Node
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=reinstall-node.sh" type="text/javascript"></script>

<span class="read-more">
Read more [here](https://stackoverflow.com/a/33947181/4620773)
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

## Jekyll
<hr class='divider--fade' />

If you want to do write some blog using `jekyll`

### Install ruby stuff
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-ruby.sh" type="text/javascript"></script>
### Gem installation directory on user account
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=gem-directory.sh" type="text/javascript"></script>
### Install jekyll
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-jekyll.sh" type="text/javascript"></script>
### Install bundle
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-bundle.sh" type="text/javascript"></script>
