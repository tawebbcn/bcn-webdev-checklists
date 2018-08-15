#  Common issues

## VS Code

- `code` command not working
  - see [vs code configuraion](./module1.md).
  - if problem persists there is an issue with .zshrc/.bashrc
- *'Visual Studio Code is unable to watch for file changes in this large workspace'* notification
  - common issue in linux happening in module 2 & 3, see [fix](https://code.visualstudio.com/docs/setup/linux#_visual-studio-code-is-unable-to-watch-for-file-changes-in-this-large-workspace-error-enospc)
- vscode warnings in html files
  - caused by `html-lint` extension, disable it
- vscode formatting inconsistently
  - caused by `prettier` or `beautify`, uninstall it

## Node

- `bad option --inspect-brk` when trying to debug in vs code
  - old version of node being used
  - confirm with node --version
  - if issue is itermittent then multiple versions of node might be installed
    - confirm with nvm list
    - make sure the latest one is always used by running `nvm default alias 10.x.x` where the version needs to be the most up to date installed in the computer
    - if no recent version is installed, run `nvm install node` to install the most recent one

## NPM packages

- unable to install bcrypt(linux)
  - in fresh linux installations, a few packets are missing that are essential to bcrypt
  - run `sudo apt-get install g++ make`
