# wiki
A Personal Wiki

## Installation Instructions

```
sudo apt-get update 
sudo apt-get install libicu-dev g++ build-essentials gem make
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
