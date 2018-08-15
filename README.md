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

```bash
./release --notebook pandoc-zhtw.ipynb
```

### 问题解答

#### 如何调整纸张和页边距？

在`pm-template.latex`用`LaTeX`语法调整。

