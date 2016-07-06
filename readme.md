# Homebrew - The missing package manager for OS X

## What is a Package Manager?

A package manager is simply a tool that helps us install, update, and remove software on our computers.  Package managers are usually CLI programs that are fast and flexible.

## What is Homebrew?

_Homebrew_ (often referred to simply _Brew_) is a package manager optimized for installing CLI programs onto a MAC running OSX.

Here is a list of some of the programs we can install using `brew`:

* cowsay
* figlet
* fortune
* git
* git-extras
* imagemagick
* mongodb
* node
* postgresql
* tree

## How do we install Homebrew?

Simply copy and paste the following into your _Terminal_ window (at the BASH prompt) and hit `Enter`:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Now you should be able to run brew. Try asking brew for it's version number:

```bash
brew --version
```

## Add Extensions to Brew

### Brew Cask

Copy and Paste the following line into your terminal window:

```bash
brew install caskroom/cask/brew-cask
```

### Caskroom Versions

```bash
brew tap caskroom/versions
```

## Install and Run Some Fun Apps

```bash
brew install cowsay
cowsay 'Welcome to WDI!'
cowsay 'Eat more chicken.'
```

```bash
brew install figlet
figlet 'Welcome to WDI!'
```

```bash
brew install fortune
fortune
fortune | cowsay
fortune | figlet
```

## References

* [Brew](http://brew.sh/)
* [Brew Cask](https://caskroom.github.io/)
