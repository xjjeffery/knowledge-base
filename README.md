# Knowledge Base

这是一个使用 [MkDocs](https://www.mkdocs.org/) 构建的静态网站，部署在 GitHub Pages 上。作为自己的在线知识库，记录并分享自己的学习和工作经验。

**为什么使用 MkDocs**:

- 使用 Markdown 作为标记语言，虽没有 Sphinx 的 RestructuredText 强大，但容易上手，且对中文较为友好。
- 丰富的 Markdown 扩展，足以满足日常文档需求。
- 配置文件使用 YAML，相比 Sphinx 使用 Python 源码进行配置相对简单。
- 强大的离线搜索功能，以及基本的中文关键词搜索支持。
- 标题 permalink anchor 支持 Unicode 字符（Sphinx 仅支持 ASCII）。

## Features

- 由 MkDocs 提供支持的简洁、响应式设计
- 易于编辑的 Markdown 内容
- 已部署到 GitHub Pages 上，可免费托管
- 本项目使用 [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) 主题
- 添加插件以增强功能，使用的插件如下：
    - [mkdocs-material](https://squidfunk.github.io/mkdocs-material/)
    - [mkdocs-glightbox](https://github.com/blueswen/mkdocs-glightbox)
    - [mkdocs-git-revision-date-localized-plugin](https://github.com/zhaoterryy/mkdocs-git-revision-date-plugin)
    - [mkdocs-statistics-plugin](https://github.com/TonyCrane/mkdocs-statistics-plugin/tree/600d5b582bbff1aa209f59cab986b3a6563d470a)
    - [mkdocs-changelog-plugin](https://github.com/TonyCrane/mkdocs-changelog-plugin/tree/b90ffb47c85e451dd82ce2b0d8779a0f35bea8a0)
    - [mkdocs-open-in-new-tab](https://github.com/JakubAndrysek/mkdocs-open-in-new-tab)
    - [jieba](https://github.com/fxsjy/jieba)

## Quick start

MkDocs 工具支持各种插件来扩展静态文档，但这些插件都是基于 Python 开发的，因此安装时尽量隔离环境，避免修改原生 Python 环境。这里建议使用 conda 虚拟环境，创建一个使用 conda 服务博客的环境。推荐使用两个工具：[Mamba](https://mamba.readthedocs.io/en/latest/) 和 [Anaconda](https://www.anaconda.com/)。

```bash
conda create -n mkdocs-env python=3.12
```

所有插件和依赖项都通过 `requirements.txt` 自动安装。

```bash
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
```

运行 MkDocs serve

```bash
mkdocs serve
```

打开浏览器 `http://localhost:8000` 来预览该网站。

## License

本项目采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证（详情请参阅 LICENSE 文件），搬运部分遵循原作者规定的许可。