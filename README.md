# wiki
A Personal Wiki

## Installation Instructions

```
sudo apt-get update 
sudo apt-get install -y git libicu-dev g++ build-essential gem make ruby1.9.3

sudo rm /usr/bin/ruby
sudo ln -s /usr/bin/ruby1.9.3 /usr/bin/ruby

sudo gem install bundle

git clone https://github.com/Kevin-M-Smith/wiki.git
cd wiki
bundle install
sudo gem install gollum-site

cd ../
git clone https://github.com/Kevin-M-Smith/wiki.wiki.git
cd wiki
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
