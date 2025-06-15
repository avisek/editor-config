# Editor Configuration

My unified configuration files for Cursor and VSCode.

## Clone repository

```sh
git clone https://github.com/avisek/editor-config.git ~/editor-config
```

## Settings and keybindings (MacOS)

### Backup existing configs (optional)

```sh
mv ~/Library/Application\ Support/Cursor/User/settings.json{,.bak}
mv ~/Library/Application\ Support/Cursor/User/keybindings.json{,.bak}
mv ~/Library/Application\ Support/Code/User/settings.json{,.bak}
mv ~/Library/Application\ Support/Code/User/keybindings.json{,.bak}
```

### Remove existing configs (optional)

```sh
rm ~/Library/Application\ Support/Cursor/User/settings.json
rm ~/Library/Application\ Support/Cursor/User/keybindings.json
rm ~/Library/Application\ Support/Code/User/settings.json
rm ~/Library/Application\ Support/Code/User/keybindings.json
```

### Symlink (recommended)

```sh
ln -sf ~/editor-config/settings.json ~/Library/Application\ Support/Cursor/User/
ln -sf ~/editor-config/keybindings.json ~/Library/Application\ Support/Cursor/User/
ln -sf ~/editor-config/settings.json ~/Library/Application\ Support/Code/User/
ln -sf ~/editor-config/keybindings.json ~/Library/Application\ Support/Code/User/
```

### Or just copy

```sh
cp ~/editor-config/settings.json ~/Library/Application\ Support/Cursor/User/
cp ~/editor-config/keybindings.json ~/Library/Application\ Support/Cursor/User/
cp ~/editor-config/settings.json ~/Library/Application\ Support/Code/User/
cp ~/editor-config/keybindings.json ~/Library/Application\ Support/Code/User/
```

## Extensions

### Export

```sh
code --list-extensions > extensions.list
```

### Import

```sh
cat extensions.list | xargs -L 1 code --install-extension

# Windows (PowerShell)
# Get-Content extensions.list | ForEach-Object { code --install-extension $_ }
```
