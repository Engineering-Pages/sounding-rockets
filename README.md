# Hosting

## Setup

```
# Install rbenv (Ruby version manager)
brew install rbenv

# Install latest Ruby
rbenv install 3.2.0
rbenv global 3.2.0

# Add to your shell profile (~/.zshrc or ~/.bash_profile)
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc

# Reload shell
source ~/.zshrc

# Now install bundler and jekyll
gem install bundler jekyll
```

## Setup docs/ as a Jekyll project
```
cd docs

# Create a Gemfile if you don't have one
echo 'source "https://rubygems.org"' > Gemfile
echo 'gem "github-pages", group: :jekyll_plugins' >> Gemfile

bundle install
```

## Run
```
bundle exec jekyll serve
```

