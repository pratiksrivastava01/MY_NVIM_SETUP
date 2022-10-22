
## Installing Neovim

## Linux

If you’re running Ubuntu or any other Linux distro, you can use its package manager as such

```bash
sudo apt install neovim
```

## macOS

Same goes with macOS’ [Homebrew](https://brew.sh/):
```bash
brew install neovim
 ```

 ## Windows

 On Windows, you can use one of the package managers such as [Chocolatey](https://chocolatey.org/):

 ```bash
brew install neovim
 ```

 Or [Scoop](https://scoop.sh/).

 ```bash
scoop install neovim
  ```
If you're having any problem with installation, please visit [the installation Wiki](https://github.com/neovim/neovim/wiki/Installing-Neovim)



## Setting Up neovim

Just like Vim, Neovim is quite simple and doesn’t include any fancy plugins out of the box, so we are going to have to install them. Firstly, let’s install a plugin manager:

## Unix (Linux/macOS)

```bash
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim - create-dirs \
 https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
 ```


 ## Windows (PowerShell)

 ```bash
 md ~\vimfiles\autoload
$uri = 'https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
(New-Object Net.WebClient).DownloadFile(
  $uri,
  $ExecutionContext.SessionState.Path.GetUnresolvedProviderPathFromPSPath(
    "~\vimfiles\autoload\plug.vim"
  )
)
```

## Editing the config file

For macOS and Linux, the Neovim config file is located in
```bash
 ~/.config/nvim/init.vim.
 ```



 ```bash
 mkdir ~/.config/nvim
 ```

 And for Windows



 ```bash
 mkdir ~/AppData/Local/nvim
 ```

 And paste the following code in the config file located in the directory specified above, called init.vim. This allows you to configure plugins by adding references to their GitHub repositories like so:
 