# 星光笔记 · 示例文档

这是一个完全虚构的个人文档练习项目，不包含真实业务或公司资料。

在线文档：https://hyacinth11.github.io/starlight-docs-demo/

## 网页维护

打开 docs/ 中的 Markdown 文件，点击编辑并提交到 main；GitHub Actions 会自动构建并发布网站。

## 本地维护（认证可用后）

```powershell
git clone git@github.com:Hyacinth11/starlight-docs-demo.git
cd starlight-docs-demo
# 编辑 docs/ 中的文档，然后执行：
git add docs/ mkdocs.yml
git commit -m "docs: update demo"
git push
```

如果你之前已有未推送的本地示例，请先保留它，不要强制推送覆盖网页版本；建议另选目录重新 clone 本仓库。

## 本地预览（可选）

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe -m mkdocs serve
```

文档源文件位于 docs/；主题和导航在 mkdocs.yml；发布工作流在 .github/workflows/docs.yml。自动发布不依赖你本机的 SSH 私钥。
