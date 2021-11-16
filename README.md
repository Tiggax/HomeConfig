# HomeConfig
my dotfiles sync

This was made following [this](https://www.atlassian.com/git/tutorials/dotfiles) site.

## Summary

### Syncing to new machine:
add alias to your new .bashrc
```
echo "alias homeconfig='/usr/bin/git --git-dir=$HOME/.homeconfig/ --work-tree=$HOME'" >> $HOME/.bashrc
```
bash to restart bashrc
```
bash
```
clone your repository
```
git clone --bare URL $HOME/.homeconfig
```
check if it works
```
homeconfig checkout
```
if it thorows errors -> remove the conflicting files / overwrite them.(i'ts a new system anyway)
