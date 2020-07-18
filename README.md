Blog [view](https://iamdevlinph.github.io/blog/)

# Setting up on WSL
1. Install
```
sudo apt-get install ruby ruby-dev build-essential
```

2. Gem installation directory on user account
```
echo '# Install Ruby Gems to ~/gems' >> ~/.zshrc
echo 'export GEM_HOME=$HOME/gems' >> ~/.zshrc
echo 'export PATH=$HOME/gems/bin:$PATH' >> ~/.zshrc
source ~/.zshrc
```
3. Install Jekyll
```
gem install jekyll bundler
```
More [here](https://jekyllrb.com/docs/installation/#ubuntu)

4. Install stuff
```
bundle install
```

# Development
Run `bundle exec jekyll serve` to run
