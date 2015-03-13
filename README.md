# wiki
A Personal Wiki

## Installation Instructions

```
sudo apt-get update 
sudo apt-get install -y git libicu-dev g++ build-essential gem make ruby1.9.3 zlib1g-dev

sudo gem install bundle

git clone https://github.com/Kevin-M-Smith/wiki.git
cd wiki
bundle install
sudo bundle exec gem build gollum-site.gemspec 
sudo gem install gollum-site

cd ../
git clone https://github.com/Kevin-M-Smith/wiki.wiki.git
cd wiki.wiki
gollum-site generate

```

## Travis Notes

### Language
```
language: ruby
```

### Send to Containerized Worker
```
sudo: false
```

### Caching

```
cache:
- bundler
- apt
```
