# VSCode Settings Documentation

My personal Visual Studio Code configuration with custom keybindings and settings.

## Table of Contents
- [Installation](#installation)
- [Key Bindings](#key-bindings)
- [Settings](#settings)
- [Extensions](#extensions)

## Installation

### macOS
```bash
# Backup existing settings
cp ~/Library/Application\ Support/Code/User/settings.json ~/Library/Application\ Support/Code/User/settings.json.backup
cp ~/Library/Application\ Support/Code/User/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json.backup

# Download settings from GitHub
curl -o ~/Library/Application\ Support/Code/User/settings.json https://raw.githubusercontent.com/Radhitndrm/VSCode-Settings/main/settings.json
curl -o ~/Library/Application\ Support/Code/User/keybindings.json https://raw.githubusercontent.com/Radhitndrm/VSCode-Settings/main/keybindings.json
```

## Key Bindings

### General Navigation
| Shortcut | Command | Description |
|----------|---------|-------------|
| `Cmd+E` | Toggle Explorer | Open/close file explorer |
| `Cmd+Shift+X` | Open Extensions | Open VS Code extensions |
| `Cmd+Shift+I` | Toggle Copilot Chat | Open/close Copilot chat panel |
| `Cmd+Shift+J` | Toggle Panel | Show/hide bottom panel |

### Terminal
| Shortcut | Command | When |
|----------|---------|------|
| `Cmd+\`` | Toggle Terminal | Always |
| `Cmd+Shift+\`` | New Terminal | Always |
| `Cmd+W` | Close Terminal | When terminal focused |
| `Cmd+Shift+A` | Focus Next Terminal | When terminal focused |
| `Cmd+Shift+B` | Focus Previous Terminal | When terminal focused |
| `Cmd+Shift+N` | New Terminal | When terminal focused |
| `Cmd+Shift+D` | Kill Terminal | When terminal focused |

### File Explorer (when focused)
| Shortcut | Command | Description |
|----------|---------|-------------|
| `A` | New File | Create new file |
| `Shift+A` | New Folder | Create new folder |
| `R` | Rename | Rename file/folder |
| `D` | Delete | Delete file/folder |
| `Enter` | Open File | Open selected file |
| `L` | Open File | Open selected file (vim-style) |

### Editor
| Shortcut | Command | Description |
|----------|---------|-------------|
| `Cmd+Shift+V` | Split Editor Right | Split editor to the right |

### Vim Mode Keybindings

#### Insert Mode
| Shortcut | Command |
|----------|---------|
| `jj` | Escape to normal mode |

#### Normal Mode - Navigation
| Shortcut | Command | Description |
|----------|---------|-------------|
| `Space+H` | Focus Left Group | Move to left editor split |
| `Space+J` | Focus Below Group | Move to editor below |
| `Space+K` | Focus Above Group | Move to editor above |
| `Space+L` | Focus Right Group | Move to right editor split |
| `Ctrl+H` | Previous Tab | Go to previous tab |
| `Ctrl+L` | Next Tab | Go to next tab |
| `Alt+,` | Previous Editor | Previous editor in history |
| `Alt+.` | Next Editor | Next editor in history |
| `Alt+C` | Close Editor | Close current editor |

#### Normal Mode - Editing
| Shortcut | Command | Description |
|----------|---------|-------------|
| `Space+V` | Vertical Split | Split editor vertically |
| `Space+S` | Horizontal Split | Split editor horizontally |
| `Space+W` | Save File | Save current file |
| `Space+Q` | Quit | Close current editor (force) |
| `Space+X` | Close Editors in Group | Close all editors in group |
| `Space+N` | Match Tag | Jump to matching HTML tag |
| `Space+F` | Open Link | Follow link under cursor |
| `Space+P` | Format Document | Format current document |
| `Space+C+A` | Quick Fix | Show quick fix menu |
| `;;` | Append Semicolon | Add semicolon at end of line |
| `,,` | Append Comma | Add comma at end of line |

#### Normal Mode - Navigation & Search
| Shortcut | Command | Description |
|----------|---------|-------------|
| `j` | Move Down | Move down (respects word wrap) |
| `k` | Move Up | Move up (respects word wrap) |
| `n` | Next Search Result | Jump to next search result (centered) |
| `N` | Previous Search Result | Jump to previous search result (centered) |
| `Ctrl+D` | Half Page Down | Scroll half page down (centered) |
| `Ctrl+U` | Half Page Up | Scroll half page up (centered) |
| `vv` | Select All | Select entire file |
| `Esc` | Clear Search | Clear search highlighting |
| `[d` | Previous Error | Go to previous diagnostic |
| `]d` | Next Error | Go to next diagnostic |
| `gh` | Peek Definition | Show definition preview |
| `gj` | Go to Definition | Jump to definition |
| `Alt+O` | Alternate File | Switch to alternate file |
| `Alt+S` | Save | Save file |

#### Normal Mode - Advanced
| Shortcut | Command | Description |
|----------|---------|-------------|
| `u` | Undo | Undo last change |
| `Ctrl+R` | Redo | Redo last undone change |
| `J` | Join Lines | Join lines (preserves cursor) |
| `Shift+H` | Disabled | Previous editor (disabled) |
| `Shift+L` | Disabled | Next editor (disabled) |
| `Ctrl+F` | New Terminal | Open new terminal |

#### Visual Mode
| Shortcut | Command | Description |
|----------|---------|-------------|
| `<` | Outdent | Decrease indentation |
| `>` | Indent | Increase indentation |
| `J` | Move Lines Down | Move selected lines down |
| `K` | Move Lines Up | Move selected lines up |
| `Space+C` | Toggle Comment | Toggle line comment |

### Quick Open
| Shortcut | Command | When |
|----------|---------|------|
| `Cmd+J` | Next Item | In quick open menu |
| `Cmd+K` | Previous Item | In quick open menu |

### Suggestions
| Shortcut | Command | When |
|----------|---------|------|
| `Cmd+J` | Next Suggestion | When suggestions visible |
| `Cmd+K` | Previous Suggestion | When suggestions visible |

### Code Folding
| Shortcut | Command |
|----------|---------|
| `Alt+K` | Fold | Fold code block |
| `Alt+J` | Unfold | Unfold code block |

### Emmet
| Shortcut | Command |
|----------|---------|
| `Cmd+Shift+5` | Match Tag | Jump to matching tag |

## Settings Highlights

### Editor
- **Font**: MonoLisa Trial
- **Font Size**: 16px
- **Line Height**: 42px
- **Font Ligatures**: Enabled
- **Line Numbers**: Relative
- **Minimap**: Disabled
- **Default Formatter**: Prettier

### UI
- **Activity Bar**: Hidden
- **Status Bar**: Visible
- **Menu Bar**: Hidden
- **Breadcrumbs**: Enabled
- **Command Center**: Hidden
- **Layout Control**: Disabled
- **Color Theme**: Vercel Cursor Theme
- **Icon Theme**: Material Icon Theme
- **Product Icon Theme**: Material Product Icons

### Terminal
- **Font**: MonoLisa Trial
- **Font Size**: 15px
- **Line Height**: 1.5
- **Default Profile (Linux)**: fish

### Vim
- **Leader Key**: Space
- **Handle Keys**: Ctrl+C, Ctrl+V, Ctrl+X, Ctrl+D, Ctrl+P, Ctrl+A, Ctrl+Y, Ctrl+W enabled

### Formatting
- **Format on Save**: Enabled
- **Trim Trailing Whitespace**: Enabled
- **Insert Final Newline**: Enabled
- **Trim Final Newlines**: Enabled

### Other Settings
- **Tab Completion**: On
- **Suggest on Commit Character**: Disabled
- **Enable Preview**: Disabled
- **Multi-Cursor Modifier**: Cmd/Ctrl
- **Snippet Suggestions**: Top
- **Detect Indentation**: Disabled
- **Hover**: Disabled
- **Lightbulb**: Disabled
- **Git Decorations**: Disabled

## Required Extensions

- **VSCodeVim** - Vim emulation
- **Prettier** - Code formatter
- **Laravel Blade** - Blade template support
- **Intelephense** - PHP language support
- **Volar** - Vue language support
- **Material Icon Theme** - File icons
- **GitHub Copilot** - AI pair programming

## Theme

- **Color Theme**: Vercel Cursor Theme
- **Icon Theme**: Material Icon Theme  
- **Product Icons**: Material Product Icons

