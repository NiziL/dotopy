# Dotypasta

Dotypasta let you easily fetch, save and apply dotfiles.  
Inspired by [chezmoi](https://chezmoi.io)

## Features roadmap

- [ ] `dotypasta load nizil` clone `https://github.com/nizil/dotfiles` to `$HOME/.local/share/dotypasta` 
  - [ ] option `--hub [github | gitlab | bitbucket ... ]` to select the git host 
  - [ ] option `-t <tag>` to load a specific tag
  - [ ] option `--ssh` to clone the repository using ssh
  - [ ] option `--apply` to directly apply the configuration
- [ ] `dotypasta app <appname>` show you the files copied for `appname` as defined in `$HOME/.local/share/dotypasta/dotypasta.conf`
  - [ ] `dotypasta app <appname> -a <files>...` add all files to the `appname` configuration
  - [ ] `dotypasta app <appname> -d <files>...` delete all files from the `appname` configuration
- [ ] `dotypasta diff` show you the difference between the loaded dotfiles and your current configuration
  - [ ] option `--app <appname>` to see the difference for a specific app
- [ ] `dotypasta apply` apply the configuration from `$HOME/.local/share/dotypasta`
  - [ ] option `--app <appname>` to apply the configuration for a specific app
- [ ] `dotypasta save` copy all the dotfiles defined in `dotypasta.conf` from the host to `$HOME/.local/share/dotypasta`, then commit and push
  - [ ] option `--app <appname>` to backup dotfiles for a specific app
  - [ ] option `-t <tag>` to add a git tag
