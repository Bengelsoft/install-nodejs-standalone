# install-node-standalone
Bash script for download standalone Nodejs for Windows and Linux

This standalone bash script is based on [install-node](https://github.com/zeit/install-node) with a few changes.

The script will install a specific version of Nodejs in the sub-directory './node/bin'.
## Example
```bash
sh node-install-standalone.sh --force
```

```bash
PATH=$PATH:$PWD/node/bin
```

Now it is possible to run NPM or NPX commands in your shell without installing Nodejs.

```bash
npm init
```

## Options:

| argument | explanation | example | default | 
|---|---|---|---|
| -v or --version | Download a specific version of Nodejs | ``` sh node-install-standalone.sh --version 8 ``` | latest | 
| -b or --base-url | The download locations of the Nodejs binaries | ``` sh node-install-standalone.sh --base-url http://mirror.example.com ``` | https://nodejs.org/dist |
| -f or --force | Skip confirm | ``` sh node-install-standalone.sh --force ``` ||
