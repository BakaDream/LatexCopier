# LaTeX 公式复制助手
![icon](https://github.com/BakaDream/LatexCopier/blob/master/icon.png?raw=true)
[![GitHub 版本](https://img.shields.io/github/v/release/BakaDream/LatexCopier?style=flat-square)](https://github.com/BakaDream/LatexCopier) [![许可证](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square)](LICENSE) [![兼容性](https://img.shields.io/badge/浏览器扩展-Tampermonkey%20/%20Violentmonkey-green.svg?style=flat-square)](https://www.tampermonkey.net/)

一个实用的浏览器脚本，帮助快速复制网页数学公式到 Word 或获取 LaTeX 源码。

## 主要功能

- **双击复制公式**：在支持的网站上直接双击数学公式
- **两种粘贴模式**：
  - **Word 兼容模式**：生成 MathML，可直接粘贴到 Microsoft Word
  - **纯源码模式**：直接复制 LaTeX 原始代码
- **实时预览**：鼠标悬停时显示公式源代码
- **自动适配**：支持常见学术/问答网站的公式渲染方式

## 当前支持网站

| 网站名称       | 支持状态 | 测试版本   |
|----------------|----------|------------|
| 中文维基百科   | ✅ 稳定  | 2025.03    |
| 知乎           | ✅ 稳定  | 2025.03    |
| ChatGPT        | ✅ 稳定  | 2025.03    |
| DeepSeek       | ✅ 稳定  | 2025.03    |
| Stack Exchange | ✅ 稳定  | 2025.03    |

## 安装使用

### 前置要求
- 浏览器扩展：[Tampermonkey](https://www.tampermonkey.net/) 或 [Violentmonkey](https://violentmonkey.github.io/)

### 安装步骤
1. [点击此处安装脚本](https://update.greasyfork.org/scripts/531420/LatexCopier.user.js)
2. 刷新已支持的网站页面
3. 双击任意数学公式开始使用

### 模式切换
通过用户脚本菜单切换模式


## 技术实现

- **公式识别**：基于 DOM 结构的网站特定适配规则
- **格式转换**：使用 MathJax 3 进行 LaTeX → MathML 转换
- **剪贴板操作**：纯 JavaScript 实现内容复制
- **配置持久化**：通过 GM API 保存用户偏好设置

## 参与改进

欢迎通过以下方式帮助改进项目：
- 报告新网站的公式无法复制的情况
- 提交适配新网站


# 开发
```
git clone https://github.com/BakaDream/LatexCopier.git
cd LatexCopier
```


## 开源协议

本项目采用 GPLv3 协议开源。

## 问题反馈

遇到问题或建议？请通过以下渠道联系：
- [GitHub Issues](https://github.com/BakaDream/LatexCopier/issues)
