## 中文编辑Notebook转PDF

使用`markdown`语法编辑，`SoS Notebook`开发环境，`pandoc`编译。

### `SoS Notebook`开发环境

1. 安装：https://vatlab.github.io/sos-docs/#Local-installation
2. 打开样例：

```bash
jupyter notebook pandoc-zhtw.ipynb &> /dev/null &
```

### `markdown`语法编辑

见示例文档`pandoc-zhtw.ipynb`：请参考这里的语法编辑达到PDF示例`pandoc-zhtw.pdf`的效果。

### `pandoc`编译

`release`脚本用SoS语言编写，使用预先提供的`docker`容器。用户电脑上不用安装`LaTeX`和`pandoc`。安装`docker`后直接运行下命令即可：

```bash
./release --notebook pandoc-zhtw.ipynb
```

如果有权限问题运行不了，首先让`release`可执行：

```
chmod +x release
```

之后就可以用上面一行命令编译了。

### 问题解答

#### 如何调整纸张和页边距？

在`pm-template.latex`用`LaTeX`语法调整。

