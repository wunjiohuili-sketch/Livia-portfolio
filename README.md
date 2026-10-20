# 李慧 / Livia Portfolio Website

这是一个静态个人作品集网站，用于展示个人简介、教育经历、研究方向、精选作品、获奖经历、软件技能与联系方式。

## 文件说明

- `index.html`：网站的页面结构和主要文字内容。
- `style.css`：网站的视觉样式、版式、颜色、网格背景和手机适配。
- `script.js`：网站的简单交互，目前用于手机端导航菜单展开与收起。
- `assets/images/`：放置个人照片和作品图片。
- `README.md`：项目说明和后续修改指引。

## 如何预览

直接双击 `index.html`，或在浏览器中打开这个文件即可预览网站。

## 图片路径

个人照片请命名为 `profile.jpg`，放入：

```text
assets/images/profile.jpg
```

首页作品封面图按以下路径读取：

```text
assets/images/work-01-cover.jpg
assets/images/work-02-cover.jpg
assets/images/work-03-cover.jpg
assets/images/work-04-cover.jpg
assets/images/work-06-cover.jpg
assets/images/work-07-cover.jpg
```

作品详情页图片按以下规则读取：

```text
assets/images/work-01-01.jpg
assets/images/work-01-02.jpg
assets/images/work-01-03.jpg
assets/images/work-01-04.jpg
assets/images/work-01-05.jpg
assets/images/work-02-01.jpg
assets/images/work-02-02.jpg
assets/images/work-02-03.jpg
assets/images/work-02-04.jpg
assets/images/work-03-01.jpg
assets/images/work-03-02.jpg
assets/images/work-03-03.jpg
assets/images/work-04-01.jpg
assets/images/work-04-02.jpg
assets/images/work-04-03.jpg
assets/images/work-04-04.jpg
assets/images/work-06-01.jpg
assets/images/work-07-01.jpg
```

如果作品图片暂时不存在，网页会显示 `IMAGE PENDING` 占位框。

## 如何替换图片

如果只是替换图片内容，通常不需要改 HTML，只要把新图片按上面的文件名放入 `assets/images/` 文件夹即可。

如果要改封面图片文件名，请在 `index.html` 中搜索：

```html
assets/images/work-01-cover.jpg
```

如果要改详情页图片文件名，请在对应的 `work-01.html` 到 `work-07.html` 中修改图片路径。

并把路径改成新的图片路径。

个人照片对应：

```html
assets/images/profile.jpg
```

## 后续如何修改文字

主要修改 `index.html`。

常见修改位置：

- 首页姓名、身份、关键词：查找 `id="home"`。
- 关于我：查找 `id="about"`。
- 教育经历：查找 `id="education"`。
- 研究方向：查找 `id="research"`。
- 精选作品：查找 `id="works"`。
- 获奖经历：查找 `id="awards"`。
- 软件技能：查找 `id="skills"`。
- 联系方式：查找 `id="contact"`。

## 后续如何修改样式

主要修改 `style.css`。

建议先从文件顶部的 `:root` 开始：

- `--color-bg`：页面背景色。
- `--color-paper`：纸张感底色。
- `--color-text`：主要文字色。
- `--color-muted`：辅助文字色。
- `--color-line`：细线和边框颜色。
- `--max-width`：页面最大宽度。

如果要调整首页版式，可以查找 `.hero`。
如果要调整精选作品列表，可以查找 `.work-card` 和 `.work-image-frame`。
如果要调整手机适配，可以查找 `@media`。
