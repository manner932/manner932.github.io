# Manner Bohan Su 的学术主页

正式网址（启用 GitHub Pages 后）：https://manner932.github.io/

网站源文件与维护入口：https://github.com/manner932/manner932.github.io/tree/main

本次学术主页使用 `main` 分支；仓库原有的 `master` 分支保留旧博客模板。维护时请先确认分支选择为 `main`。

英文、四个独立页面，无付费主题，无额外插件。CV、论文和教学笔记使用外部链接。网页正文、样式和上传的照片会在公开仓库中公开。

## 第一次上线

1. 登录 GitHub，创建公开仓库，名称必须为 `manner932.github.io`。
2. 上传本文件所在文件夹中的**内容**到仓库根目录，不要把整个文件夹作为一层子目录上传。根目录应该直接看到 `_config.yml`、`index.md` 等文件。需要上传 `_layouts` 和 `assets` 两个文件夹，可在网页上传区拖入文件及文件夹。
3. 保存到 `main` 分支。
4. 打开仓库的 **Settings → Pages**，Source 选择 **Deploy from a branch**，Branch 选择 **main**，文件夹选择 **/(root)**，点击 **Save**。
5. 等待 GitHub 完成发布，再访问上面的正式网址。更新不是即时生效，需等发布完成。

当前照片、CV、论文、课程和笔记尚未提供，页面会明确显示 forthcoming 或 will be added here。收到材料后替换提示即可。

## 日常修改

在仓库中打开对应文件，点击铅笔图标编辑，完成后点击 **Commit changes**，直接保存到 `main`。GitHub 会自动更新网站。

可以直接点击以下编辑入口：

- [修改简介](https://github.com/manner932/manner932.github.io/edit/main/index.md)
- [修改论文列表](https://github.com/manner932/manner932.github.io/edit/main/research.md)
- [修改授课和助教经历](https://github.com/manner932/manner932.github.io/edit/main/teaching.md)
- [修改教学笔记](https://github.com/manner932/manner932.github.io/edit/main/others.md)
- [修改 CV 链接或照片路径](https://github.com/manner932/manner932.github.io/edit/main/_config.yml)

| 内容 | 编辑文件 |
| --- | --- |
| 自我介绍 | `index.md` |
| 论文列表 | `research.md` |
| 授课和助教经历 | `teaching.md` |
| Teaching notes | `others.md` |
| CV 链接、照片路径 | `_config.yml` |

页面文件顶部两条 `---` 之间是页面设置。日常更新只修改第二条 `---` 下面的正文，不要删除或改动顶部设置。

### 添加或更新 CV 链接

打开 `_config.yml`，将空的 `cv_url` 改成你的外部分享地址，保留英文双引号，例如：

```yaml
cv_url: "https://你的云盘分享地址"
```

请使用 HTTPS 链接。分享权限由你在外部平台设置；若希望所有访客可阅读，需要允许访客访问。用未登录云盘的浏览器验证链接是否按你的预期工作。若更新文件后分享地址不变，网站无需修改。

### 添加照片

将照片命名为 `portrait.jpg`，上传到仓库的 `assets` 文件夹。然后把 `_config.yml` 中的照片路径改为：

```yaml
photo: "/assets/portrait.jpg"
```

可以使用 PNG，但文件名和路径必须与上传的文件一致。照片会保持原始宽高比。推荐竖向肖像，宽度约 600–1000 像素；上传前去除不需要公开的定位信息。也可以填写可直接加载的 HTTPS 图片地址。

### 添加论文

在 `research.md` 中移除占位提示，按以下结构粘贴实际信息：

```markdown
### 论文英文标题

With 合作者姓名. Working paper, 年份.

[Paper](https://论文外部链接)
```

独著时删除 With 那句话；年份和论文状态只填写真实信息。添加第二篇时复制同样的结构。显示顺序与文件中的顺序一致。

### 添加课程

在 `teaching.md` 的 Instructor 或 Teaching Assistant 标题下，用实际经历替换提示：

```markdown
- **课程英文名** — 学校英文名, Fall 2026.
```

建议同一类别把最近的课程放在最前面。

### 添加教学笔记

在 `others.md` 的 Teaching Notes 标题下移除提示并增加：

```markdown
- **笔记英文标题** — 一句简短介绍。 [PDF](https://笔记外部链接)
```

PDF 保存在你选择的外部平台，网页只保留链接。

## 更新后检查

1. 查看仓库的 Actions 或 Settings → Pages，确认本次发布成功。
2. 打开网站检查内容；若仍显示旧版，刷新页面。
3. 点击修改过的链接，用手机检查排版。
4. 如果云盘要求登录或申请权限，确认这与你预期的访问方式一致。

## 误改后如何恢复

打开误改的文件，点击 **History**，找到修改前的版本，查看并复制它的内容。回到当前文件，点击编辑，将内容替换为旧版本并保存。网站会自动重新发布。

保存失败或网站没有更新时，先查看发布状态和报错；不要反复修改 `_layouts`、样式文件或页面顶部设置。日常维护只需正文、链接和照片路径。
