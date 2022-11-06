## 功能扩展

资源管理器热键自定义

```
// 编辑窗口情况下

ctrl + ; : 聚集到资源管理器
ctrl + ' : 聚集到第一个编辑窗口

// 聚焦到资源管理器情况下

a : 新建文件
A : 新建文件夹
r : 重命名文件
d : 删除文件
x : 剪切文件
y : 复制文件
p : 粘贴
```

keybindings.json 配置

```json
[
  {
    "key": "ctrl+;",
    "command": "workbench.view.explorer",
    "when": "viewContainer.workbench.view.explorer.enabled"
  },
  {
    "key": "ctrl+'",
    "command": "workbench.action.focusFirstEditorGroup"
  },
  {
    "key": "a",
    "command": "explorer.newFile",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "A",
    "command": "explorer.newFolder",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "r",
    "command": "renameFile",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "d",
    "command": "deleteFile",
    "when": " explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus "
  },
  {
    "key": "x",
    "command": "filesExplorer.cut",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "y",
    "command": "filesExplorer.copy",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !inputFocus"
  },
  {
    "key": "p",
    "command": "filesExplorer.paste",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceReadonly && !inputFocus"
  },
]

```
