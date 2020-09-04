# ports
Personal package collection meant to be used on top of void.
# install
Clone the repo somewhere and export PORTSDIR in your shellrc as the path to where you cloned it.
# usage
```
# install
port-manager install packagename
port-manager i packagename

# uninstall
port-manager remove packagename
port-manager r packagename

# upgrade
port-manager upgrade packagename
port-manager u packagename
```

> Note: Upgrading is WIP
# package format
```
list/
  package_one/
    install
    uninstall
```
`install`/`uninstall` is run in the package's directory whenever a package is installed/uninstalled. `$BIN` will be set to where the user wants executable files to be placed.
