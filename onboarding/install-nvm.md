# Install Node Version Manager (nvm)

Run the following command in the Terminal application:

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
```

This downloads a script and runs it. The script clones the nvm repository to `~/.nvm`, and attempts to add the source lines from the snippet below to the correct profile file (`~/.bash_profile`, `~/.zshrc`, `~/.profile`, or `~/.bashrc`).

When installing on a new macOS machine, you may receive the following message:

```
=> Profile not found. Tried ~/.bashrc, ~/.bash_profile, ~/.zshrc, and ~/.profile.
=> Create one of them and run this script again
```

This is because these files do not exist by default. Since macOS 10.15, the default shell is `zsh` and nvm will look for `.zshrc` to update. Therefore, adding `~/.zshrc` is the best option. To add this file, run the commany `touch ~/.zshrc` and run the nvm install script again.

Once the script has finished executing, `~/.zshrc` should containt the following:

```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```

You can check to make sure by opening the file in VS Code by running `code ~/.zshrc`. If the file does not include the code above, add it and save the file.

Now quit your Terminal application and launch it again. To verify nvm has installed successfully, run `command -v nvm`, which should output `nvm`.

For complete nvm installation and troubleshooting documentation, please refer to the [nvm GitHub repository](https://github.com/nvm-sh/nvm).

### Potential issues

* [HEAD detached at FETCH_HEAD](https://github.com/nvm-sh/nvm/issues/2486)
