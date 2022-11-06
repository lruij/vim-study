
## 优化操作


自定义按键映射

```
H : 替代 ^
L : 替代 g_

space + n + f : 新建文件
space + n + d : 新建文件夹

```

在 settings.json 进行配置 vim 插件按键映射

```json

{
    "vim.normalModeKeyBindings": [
        {
            "before": ["H"],
            "after": ["^"]
        },
        {
            "before": ["L"],
            "after": ["g", "_"]
        }
    ],
    "vim.operatorPendingModeKeyBindings": [
        {
            "before": [
                "H"
            ],
            "after": [
                "^"
            ]
        },
        {
            "before": [
                "L"
            ],
            "after": [
                "g",
                "_"
            ]
        }
    ],
    "vim.normalModeKeyBindingsNonRecursive": [
        {
            "before": [
                "<Leader>",
                "n",
                "f"
            ],
            "commands": [
                "explorer.newFile"
            ]
        },
        {
          "before": [
            "<Leader>",
            "n",
            "d"
          ],
          "commands": [
            "explorer.newDirectory"
          ]
        }
    ]
}


```
