# wiki
A Personal Wiki

## Installation Instructions

```
git clone (path to wiki)
sudo apt-get update 
sudo apt-get install libicu-dev g++ build-essentials gem make
sudo gem install bundle

bundle install

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
