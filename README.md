# Manual for local build

## Package installation

### For Mac

```shell
brew install ruby
brew install rbenv
rbenv install 3.0.0
rbenv global 3.0.0
echo 'eval "$(rbenv init - $(basename $SHELL))"' >> ~/.profile
echo 'export PATH="$HOME/.gem/ruby/3.0.0/bin:$PATH"' >> ~/.profile
```

## Dependency installation

```shell
gem install --user-install bundler
bundle init
bundle add jekyll{,-sitemap,-feed,-seo-tag,-paginate} webrick
bundle install
```

## Run

```shell
bundle exec jekyll serve --trace
```
