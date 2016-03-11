# Node.js

## Linux installation

```
wget https://nodejs.org/dist/v5.8.0/node-v5.8.0-linux-x64.tar.xz
sudo tar -C /usr/local --strip-components 1 -xf node-v5.8.0-linux-x64.tar.xz
```

The node and npm binaries will be installed to `/usr/local/bin`.

Source: http://www.hostingadvice.com/how-to/install-nodejs-ubuntu-14-04/#standard-binary-packages

## nvm

```
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash
```

Don't use homebrew or npm to install nvm.
