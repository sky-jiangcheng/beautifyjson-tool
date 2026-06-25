# JSON 格式化工具

一个现代化的 JSON 格式化与对比工具，纯前端单文件实现，无需后端。

**在线使用**: https://sky-jiangcheng.github.io/beautifyjson-tool/

## 功能

### 格式化与压缩
- **格式化** — 2 空格缩进，语法高亮，可交互的 collapsible 树形视图
- **压缩** — 单行紧凑输出
- **自动修复** — 缺失括号时自动补全

### 交互式 JSON 树
- 对象/数组节点可展开/折叠（`▼` / `▶` 切换）
- 折叠时显示节点摘要（`{3 键}` / `[5 项]`）
- 行号列同步滚动

### 列表/详情视图
- 数组类型 JSON 自动切换为左右分栏模式
- 左侧列表项带预览摘要，点击切换右侧详情
- 列表面板可折叠

### JSON 对比
- 结构化递归比对（非文本行比对），按键/索引匹配
- 差异高亮：绿色 = 新增，红色 = 删除，黄色 = 修改
- 左右双树独立渲染，保留展开/折叠交互
- 滚动同步，支持交换左右

### 历史记录
- 格式化后可保存到本地历史（localStorage）
- 点击加载历史记录并自动格式化
- 最多同时选中 2 条进行对比
- 侧边栏可折叠

### 主题切换
- 暗色模式（GitHub Dark）
- 亮色模式（GitHub Light）
- 偏好存入 localStorage，刷新保持

### 快捷键

| 快捷键 | 操作 |
|--------|------|
| `Ctrl+Enter` | 格式化 |
| `Ctrl+S` | 保存到历史 |
| `Ctrl+D` | 下载 JSON 文件 |
| `Escape` | 关闭弹窗/对比视图 |

macOS 上使用 `Cmd` 替代 `Ctrl`。

### 拖放
支持拖拽 `.json` 文件到输入区域自动加载并格式化。

## 技术栈

- 纯 HTML/CSS/JavaScript，无框架依赖
- 语法高亮: highlight.js
- 存储: localStorage

## 部署

本项目为纯静态站点，部署到任意静态托管服务即可：

```bash
# 本地开发
python3 -m http.server 8000

# GitHub Pages
# 在仓库 Settings > Pages 中启用，选择 main 分支
```

## 文件结构

```
index.html   — 完整应用 (HTML + CSS + JS)
README.md    — 项目说明
```
