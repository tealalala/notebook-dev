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

### Step 2: Install New Packages
- $1 = package name, new
- $2 = package name, upgrade

```
brew install $1
brew info $1      # brew: check new package version
$1 --version      # bash: check new package version
which $1          # where package is located
```

### Step 3: Upgrade Existing Packages
```
brew upgrade $2
brew info $2      # brew: check package package version
$2 --version      # check upgraded package version
which $1          # where package is located
```
