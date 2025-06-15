# My configuration files for Cursor and VSCode

## Creating symlinks

```sh
# Remove existing
rm ~/Library/Application\ Support/Cursor/User/settings.json
rm ~/Library/Application\ Support/Cursor/User/keybindings.json
rm ~/Library/Application\ Support/Code/User/settings.json
rm ~/Library/Application\ Support/Code/User/keybindings.json

# Symlink
ln -s ~/Web/Editor-Config/settings.json ~/Library/Application\ Support/Cursor/User/settings.json
ln -s ~/Web/Editor-Config/keybindings.json ~/Library/Application\ Support/Cursor/User/keybindings.json
ln -s ~/Web/Editor-Config/settings.json ~/Library/Application\ Support/Code/User/settings.json
ln -s ~/Web/Editor-Config/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json

# Or just copy
cp ~/Web/Editor-Config/settings.json ~/Library/Application\ Support/Cursor/User/settings.json
cp ~/Web/Editor-Config/keybindings.json ~/Library/Application\ Support/Cursor/User/keybindings.json
cp ~/Web/Editor-Config/settings.json ~/Library/Application\ Support/Code/User/settings.json
cp ~/Web/Editor-Config/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
```
