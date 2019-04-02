# Basic Handling: Install, Uninstall and Upgrade

## Materials
* Gatsby CLI v2.4.17

## Instructions
In terminal:

### Step 1: Prep Brew
```
brew doctor       # diagnose errors
brew cleanup      # clean up old packages
```

### Step 2: Install & Upgrade Gatsby Globally
- $1 = package name, new
- $2 = package name, upgrade

```
# install globally
npm install -g gatsby-cli   # global installation
which $1                    # where gatsby is located

# upgrade globally
npm upgrade -g gatsby-cli   # global upgrade
```

### Step 3: Uninstall Gatsby Globally
```
npm uninstall -g gatsby-cli
```
