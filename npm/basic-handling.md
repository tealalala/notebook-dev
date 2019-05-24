# Basic Handling: Install, Uninstall, Upgrade & List

## Materials
* brew
  * npm v6.9.0 - install with brew

## Instructions
In terminal:

### Step 1: Update `npm`
```
brew upgrade npm       # upgrade npm with brew
```

### Step 2: Install New and Upgrade Existing Packages
- $1 = package name, new
- $2 = package name, upgrade

```
npm install -g $1

# update local package
npm upgrade -g $2

# update global packages
npm outdated -g --depth=0
npm update -g

```

### Step 3: List all `npm` packages in global and local
```
# global list - lists main package, no dependencies
npm list -global --depth=0      # longhand
npm list -g --depth=0           # shorthand

# local list - lists main package, no dependencies
npm list -local --depth=0       # longhand
npm list -l --depth=0           # shorthand - lists more details on pkg
```
