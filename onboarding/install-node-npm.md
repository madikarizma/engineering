# Install Node and npm

Please note this [recommendation by npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm#using-a-node-version-manager-to-install-node-js-and-npm):

> We strongly recommend using a Node version manager like nvm to install Node.js and npm. We do not recommend using a Node installer, since the Node installation process installs npm in a directory with local permissions and can cause permissions errors when you run npm packages globally.

If you haven't already, [install Node Version Manager (nvm)](install-nvm.md) before proceeeding.

---

#### Install the latest version of Node:

```
nvm install node
```

You'll need to reference this version in the next step.

#### Command nvm to use the Node version that was installed:

```
nvm use node
```

#### Install npm

```
nvm install-latest-npm
```

---

There are many ways to use nvm, such as install specific versions or . Please refer to the [nvm GitHub repository](https://github.com/nvm-sh/nvm) for more information.
