# Basic Handling: Install and Uninstall

## Materials
* Brew v2.0.4

## Instructions
In terminal:

### Step 1: Prep Brew
```
brew doctor       # diagnose errors
brew cleanup      # clean up old packages
```

### Step 2: Install iTerm2
- $1 = package name, new

```
brew cask info atom
brew cask install atom
brew cask info atom
$1 --version      # bash: check new package version
which $1          # where package is located
```

### Step 3: Upgrade Existing Packages
```
brew cask upgrade $1
brew cask info $1     # brew: check package package version
$1 --version          # check upgraded package version
which $1              # where package is located
```
