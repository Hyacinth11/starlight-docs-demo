# 快速开始

## 1. 修改一段文字

用任意文本编辑器打开 `docs/index.md`，例如把“月亮收纳盒”改成“彩虹收纳盒”，保存文件。

## 2. 提交并推送

在项目目录运行：

```powershell
git status
git add docs/index.md
git commit -m "docs: update fictional project name"
git push
```

## 3. 检查发布

在 GitHub 仓库的 **Actions** 中查看 `Publish documentation`，等 build 和 deploy 都成功，再打开网站刷新。

## 可选：本地预览

首次准备环境：

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

启动预览：

```powershell
.\.venv\Scripts\python.exe -m mkdocs serve
```

打开终端显示的本地地址。按 `Ctrl+C` 停止。

## 新增页面

在 `docs/` 下新增 `.md` 文件，然后把路径加入 `mkdocs.yml` 的 `nav` 配置，提交两个文件即可。
