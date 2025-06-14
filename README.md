# My configuration files for VSCode and Cursor

## Creating symlinks

```sh
rm ~/Library/Application\ Support/Code/User/settings.json
rm ~/Library/Application\ Support/Cursor/User/settings.json

ln -s ~/Web/Editor-Config/settings.json ~/Library/Application\ Support/Code/User/settings.json
ln -s ~/Web/Editor-Config/settings.json ~/Library/Application\ Support/Cursor/User/settings.json

rm ~/Library/Application\ Support/Code/User/keybindings.json
rm ~/Library/Application\ Support/Cursor/User/keybindings.json

ln -s ~/Web/Editor-Config/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
ln -s ~/Web/Editor-Config/keybindings.json ~/Library/Application\ Support/Cursor/User/keybindings.json
```
