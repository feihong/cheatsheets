# Visual Studio Code

## Shortcuts

| **Command** | **Shortcut** |
|----------|----------|
| Edit settings | `Cmd + ,` |

## Settings

```json
{
    "editor.rulers": [
        80,
        120
    ],
    "editor.tabSize": 2,
    "editor.minimap.enabled": false,
    "editor.formatOnSave": true,
    "editor.renderWhitespace": "all",
    "files.insertFinalNewline": true,
    "files.trimTrailingWhitespace": true,
    "window.zoomLevel": 0,
    "workbench.startupEditor": "newUntitledFile",
    "explorer.confirmDragAndDrop": false,
    "git.ignoreMissingGitWarning": true,
    "javascript.format.enable": true,
    "reason.diagnostics.tools": [
        "merlin",
        "bsb"
    ],
    "reason.path.bsb": "/usr/local/bin/bsb",
    "reason.codelens.enabled": true,
    "files.associations": {
        "*.atd": "ocaml"
    },
    "diffEditor.renderSideBySide": false,
    "reason_language_server.autoRebuild": false,
    "workbench.colorTheme": "Default Light+"
}
```

## Commands

Install extension from vsix file

    code --install-extension path/to/my-extension.vsix

## Extensions to install

- reason-vscode (config prefix: reason)
