---
layout: article
title:  "Setting Up Development on WSL"
date:   2018-04-29 00:00:02 +0800
group: "blog"
comments: true
---
![alt image](https://i1.wp.com/www.nextofwindows.com/wp-content/uploads/2017/07/image-3.png)
Setting up my development on WSL on Windows 10.
## Install WSL
<hr class='divider--fade' />
Open a `command prompt`


``` javascript
lxrun /install /y
```

## Git
<hr class='divider--fade' />

1 Install Git

```javascript
sudo apt-get update
sudo apt-get install git

# verify
git --version
```
More [here](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-16-04)

2 A better git log

``` javascript
git config --global alias.lg "log --color --graph --pretty=format:'%C(bold yellow)%h%Creset -%C(bold cyan)%d%Creset %s %C(bold cyan)(%cr) %C(bold red)<%an>%Creset' --abbrev-commit"
```
Use it by running `git lg`

Colors: `normal, black, red, green, yellow, blue, magenta, cyan, white`

Attributes: `bold, dim, ul, blink, reverse`

<span class="read-more">
Read more [here](https://stackoverflow.com/a/15458378/4620773)
</span>

3 Configure GIT to push on current branch

``` javascript
git config --global push.default current
```

<span class="read-more">
Read more [here](https://makandracards.com/makandra/8039-git-how-to-configure-git-to-push-only-your-current-branch)
</span>

### Hub
``` javascript
# Install binary and documentation
wget https://github.com/github/hub/releases/download/v2.2.9/hub-linux-amd64-2.2.9.tgz
tar zvxvf hub-linux-amd64-2.2.9.tgz
sudo ./hub-linux-amd64-2.2.9/install

# Skipped autocomplete and alias

# Cleanup
rm -rf hub-linux-amd64-2.2.9
```

<span class="read-more">
Read more [here](https://askubuntu.com/a/816541/634714)
</span>

## Install Node
<hr class='divider--fade' />

``` javascript
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y nodejs

# verfiy
node -v
npm -v

# update npm
npm i -g npm
```

<span class="read-more">
Read more [here](https://nodesource.com/blog/installing-node-js-tutorial-ubuntu/)
</span>

## Generate SSH Keys and Copy
<hr class='divider--fade' />

``` javascript
ssh-keygen -t rsa -C "your_email@example.com"

# Copy key to clipboard
cat ~/.ssh/id_rsa.pub
```

## ZSH Shell
<hr class='divider--fade' />
1 Install ZSH

``` javascript
sudo apt-get install zsh

# verify
zsh --version

# set as default
chsh -s $(which zsh)
```
<span class="read-more">
Read more [here](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)
</span>

2 Oh my ZSH

``` javascript
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

<span class="read-more">
Read more [here](https://github.com/robbyrussell/oh-my-zsh#via-curl)
</span>


3 Auto suggest

``` javascript
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

<span class="read-more">
Read more [here](https://github.com/zsh-users/zsh-autosuggestions#oh-my-zsh)
</span>
