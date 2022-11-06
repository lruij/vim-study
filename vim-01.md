## 环境准备

1、vscode 安装 `vim` 插件
2、mac 电脑设置键盘`按键重复`和`重复前延迟`到最高

## 终端配置

To enable key-repeating, execute the following in your Terminal, log out and back in, and then restart VS Code

**启用 按键重复**

```bash
$ defaults write com.microsoft.VSCode ApplePressAndHoldEnabled -bool false              # For VS Code
$ defaults write com.microsoft.VSCodeInsiders ApplePressAndHoldEnabled -bool false      # For VS Code Insider
$ defaults write com.visualstudio.code.oss ApplePressAndHoldEnabled -bool false         # For VS Codium
$ defaults write com.microsoft.VSCodeExploration ApplePressAndHoldEnabled -bool false   # For VS Codium Exploration users
$ defaults delete -g ApplePressAndHoldEnabled                                           # If necessary, reset global default
```

## 技巧扩展


**安装 im-select 解决 Normal 模式下切换输入法问题**


```
https://github.com/daipeihust/im-select#macos
```

配置 settings.json

```json
{
  "vim.autoSwitchInputMethod.enable": true,
  "vim.autoSwitchInputMethod.defaultIM": "com.apple.keylayout.ABC",
  // 获取 im-select 安装路径: which im-select
  "vim.autoSwitchInputMethod.obtainIMCmd": "/opt/homebrew/bin/im-select",
  "vim.autoSwitchInputMethod.switchIMCmd": "/opt/homebrew/bin/im-select",
}

```
