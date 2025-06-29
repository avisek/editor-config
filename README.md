# Editor Configuration

My unified and symlinked configuration files for Cursor and VSCode.

> [!IMPORTANT]
> Use [Git Bash](https://git-scm.com/downloads) on Windows.

## Clone the repository

```sh
git clone https://github.com/avisek/editor-config.git ~/editor-config
```

## Settings and keybindings

<details>
  <summary>

### Backup existing configs (optional)

  </summary>

```sh
# Linux
mv ~/.config/Cursor/User/settings.json{,.bak}
mv ~/.config/Cursor/User/keybindings.json{,.bak}
mv ~/.config/Code/User/settings.json{,.bak}
mv ~/.config/Code/User/keybindings.json{,.bak}

# MacOS
mv ~/Library/Application\ Support/Cursor/User/settings.json{,.bak}
mv ~/Library/Application\ Support/Cursor/User/keybindings.json{,.bak}
mv ~/Library/Application\ Support/Code/User/settings.json{,.bak}
mv ~/Library/Application\ Support/Code/User/keybindings.json{,.bak}

# Windows
mv ~/AppData/Roaming/Cursor/User/settings.json{,.bak}
mv ~/AppData/Roaming/Cursor/User/keybindings.json{,.bak}
mv ~/AppData/Roaming/Code/User/settings.json{,.bak}
mv ~/AppData/Roaming/Code/User/keybindings.json{,.bak}
```

</details>

<details>
  <summary>

### Remove existing configs (optional)

  </summary>

```sh
# Linux
rm ~/.config/Cursor/User/settings.json
rm ~/.config/Cursor/User/keybindings.json
rm ~/.config/Code/User/settings.json
rm ~/.config/Code/User/keybindings.json

# MacOS
rm ~/Library/Application\ Support/Cursor/User/settings.json
rm ~/Library/Application\ Support/Cursor/User/keybindings.json
rm ~/Library/Application\ Support/Code/User/settings.json
rm ~/Library/Application\ Support/Code/User/keybindings.json

# Windows
rm ~/AppData/Roaming/Cursor/User/settings.json
rm ~/AppData/Roaming/Cursor/User/keybindings.json
rm ~/AppData/Roaming/Code/User/settings.json
rm ~/AppData/Roaming/Code/User/keybindings.json
```

</details>

### Symlink (recommended)

```sh
# Linux
ln -sf ~/editor-config/settings.json ~/.config/Cursor/User/
ln -sf ~/editor-config/keybindings.json ~/.config/Cursor/User/
ln -sf ~/editor-config/settings.json ~/.config/Code/User/
ln -sf ~/editor-config/keybindings.json ~/.config/Code/User/

# MacOS
ln -sf ~/editor-config/settings.json ~/Library/Application\ Support/Cursor/User/
ln -sf ~/editor-config/keybindings.json ~/Library/Application\ Support/Cursor/User/
ln -sf ~/editor-config/settings.json ~/Library/Application\ Support/Code/User/
ln -sf ~/editor-config/keybindings.json ~/Library/Application\ Support/Code/User/

# Windows
ln -sf ~/editor-config/settings.json ~/AppData/Roaming/Cursor/User/
ln -sf ~/editor-config/keybindings.json ~/AppData/Roaming/Cursor/User/
ln -sf ~/editor-config/settings.json ~/AppData/Roaming/Code/User/
ln -sf ~/editor-config/keybindings.json ~/AppData/Roaming/Code/User/
```

<details>
  <summary>

### Or just copy

  </summary>

```sh
# Linux
cp ~/editor-config/settings.json ~/.config/Cursor/User/
cp ~/editor-config/keybindings.json ~/.config/Cursor/User/
cp ~/editor-config/settings.json ~/.config/Code/User/
cp ~/editor-config/keybindings.json ~/.config/Code/User/

# MacOS
cp ~/editor-config/settings.json ~/Library/Application\ Support/Cursor/User/
cp ~/editor-config/keybindings.json ~/Library/Application\ Support/Cursor/User/
cp ~/editor-config/settings.json ~/Library/Application\ Support/Code/User/
cp ~/editor-config/keybindings.json ~/Library/Application\ Support/Code/User/

# Windows
cp ~/editor-config/settings.json ~/AppData/Roaming/Cursor/User/
cp ~/editor-config/keybindings.json ~/AppData/Roaming/Cursor/User/
cp ~/editor-config/settings.json ~/AppData/Roaming/Code/User/
cp ~/editor-config/keybindings.json ~/AppData/Roaming/Code/User/
```

</details>

## Extensions

### Export

```sh
cursor --list-extensions > ~/editor-config/extensions.list
# Or
code --list-extensions > ~/editor-config/extensions.list
```

### Import

```sh
xargs -L 1 cursor --install-extension < ~/editor-config/extensions.list
xargs -L 1 code --install-extension < ~/editor-config/extensions.list
```
