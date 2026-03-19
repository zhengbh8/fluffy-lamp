# 毕业论文项目仓库

本仓库用于撰写和管理毕业论文文档。你可以在此维护正文、插图、参考文献及相关材料，并通过版本控制记录修改历史。

## 使用方式

1. 在 `thesis/thesis.md` 中填写论文的各章节内容，或在 `thesis/chapters/` 下为每章创建独立的 Markdown 文件，最终合并到 `thesis/thesis.md` 输出。
2. 如需导出为 PDF，可使用 [Pandoc](https://pandoc.org/)：
   ```bash
   pandoc thesis/thesis.md -o thesis/thesis.pdf --from markdown --toc
   ```
   文档包含中文时，建议追加 `--pdf-engine=xelatex -V mainfont=\"Noto Serif CJK SC\"` 或其他系统可用字体以避免乱码。
3. 将图片、图表等资源放入 `thesis/assets/`。
4. 使用分支与 Pull Request 组织修改和评审，确保重要变更都有记录。

## 目录结构

- `thesis/thesis.md`：论文主文件（Markdown 模板）。
- `thesis/chapters/`：可选的分章节草稿目录。
- `thesis/assets/`：插图、图表等资源。
- `LICENSE`：许可协议（MIT）。

## 贡献与协作

- 建议每次修改前创建新分支，完成后通过 Pull Request 合并。
- 在提交中简要说明修改的章节或内容，便于回溯。
- 如果需要多人协作，可在 PR 中进行评审与讨论。

## 背景

此仓库的目标是提供一个简洁的论文写作版本控制环境，帮助你专注于内容创作，同时保留完善的历史记录和协同能力。
