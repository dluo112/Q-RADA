# 上传与后续发布

这个目录已经是独立的本地 Git 仓库，默认分支为 `main`，包含初始提交。论文原目录不需要上传。

## 使用 Git 上传

1. 在 GitHub 或其他 Git 托管平台新建一个空仓库。建议命名为 `Q-RADA`，不要在平台上预先生成 README、许可证或 `.gitignore`。
2. 在本地 `Q-RADA` 目录打开终端，将下面的示例地址替换为你实际创建的仓库地址：

```powershell
git remote add origin https://github.com/YOUR_ACCOUNT/Q-RADA.git
git push -u origin main
```

如果已经配置过 `origin`，可以用 `git remote -v` 查看，再用 `git remote set-url origin <实际地址>` 修改。

## 使用网页上传

解压仓库目录旁的 `Q-RADA-upload.zip`，进入其中的 `Q-RADA` 文件夹，将其内容按目录结构上传。压缩包不包含 `.git`；网页上传不需要本地提交历史。仓库根目录应直接包含 `README.md`、`assets/`、`docs/`、`results/` 等内容。

## 当前材料

- 英文和中文 README，英文版是 GitHub 默认首页。
- 方法主图、动机图、区域曲线、参数敏感性与 token 分配图，含 PNG 和原始矢量 PDF。
- 8 组实验表格，共 93 行结果，含可阅读的 Markdown、CSV 和原始 LaTeX 摘录。
- 手稿 BibTeX 引用、素材来源和校验信息。

README 中的作者、标题、联系人和结果以 `zdy.tex` 为依据。目前没有公开论文链接或正式发表信息，因此没有填写期刊录用状态、DOI、arXiv 地址或发表年份。

## 后续添加代码

将实现、依赖、推理与评测脚本加入仓库后，更新 README 的发布进度和复现说明。当前没有替作者指定 MIT、Apache 或其他许可证；发布代码时应按你确定的授权方式添加相应 `LICENSE`。

```powershell
git add .
git commit -m "Release Q-RADA implementation"
git push
```
