# Homebrew - The missing package manager for OS X

## What is a Package Manager?

A package manager is simply a tool that helps us install, update, and remove software on our computers.  Package managers are usually CLI programs that are fast and flexible, making it very easy to install other CLI applications.

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

## Brew Cask

_Brew Cask_ is an extention to _Brew_ that allows us to install GUI apps such as the Google Chrome browser or the Sublime Editor. You can install Brew Cask by copying and pasting the following line into your terminal window:

```bash
brew install caskroom/cask/brew-cask
```

## Caskroom Versions

Sometimes we want to install software that is not *yet* in general release (aka "Beta" software). This software is available to Brew Cask via the _versions_ tap. Simply copy and paste the following into your terminal to enable _brew cask versions_:

```bash
brew tap caskroom/versions
```

## Install and Run Some Fun Apps

Let's test out `brew` by installing some fun CLI apps:

### Cowsay:

```bash
brew install cowsay
cowsay 'Welcome to WDI!'
cowsay 'Eat more chicken.'
```

### Figlet

```bash
brew install figlet
figlet 'Welcome to WDI!'
```

### Fortune

```bash
brew install fortune
fortune
fortune | cowsay
fortune | figlet
```

## Summary

_Homebrew_ makes installing CLI programs very easy on a MAC. _Homebrew Cask_ adds support for GUI programs as well.
We will be using `brew` throughout this class to install more CLI programs (such as PostgreSQL and MongoDB).

## References

* [Brew](http://brew.sh/)
* [Brew Cask](https://caskroom.github.io/)
