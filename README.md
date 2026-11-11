# 视频研读 · Video Study

一个把视频变成图文学习材料的 Codex Skill。给它课程回放、访谈、产品演示或本地录屏，Codex 会用 Computer Use 打开播放器、定位并截取关键画面，再把截图和对应的字幕或转写按时间戳配在一起。

## 安装

在终端运行以下命令，把仓库克隆到 Codex 的个人技能目录：

```sh
mkdir -p "$HOME/.agents/skills"
git clone https://github.com/fermionoid/video-study.git "$HOME/.agents/skills/video-study"
```

已有同名技能时，更新原来的安装即可。安装后在 Codex 对话中输入 `$video-study`。如果技能没有出现，重启 Codex 后再试。[Codex 官方技能文档](https://developers.openai.com/codex/skills/)

## 使用

把链接或本地视频路径交给 Codex，再说你想拿到什么：

- **图文笔记**：用 `$video-study` 研读这个回放，截下讲到关键概念时的画面，配上文字和时间戳。
- **图文逐字稿**：用 `$video-study` 整理整场访谈，保留完整对话，把 Slides 放在对应的段落旁边，导出 PDF。
- **截图教程**：用 `$video-study` 把这段录屏整理成操作步骤，每一步配一张图和对应时间。

在线回放需要能在你的浏览器里播放。技能优先用播放器字幕或你提供的字幕；没有字幕时，需要有可用的转写工具。Computer Use 不可用时，有本地视频的情况下可以用 FFmpeg 截帧。已有字幕和图片也可以直接交给技能排版。

## 仓库内容

- [SKILL.md](SKILL.md) 定义技能的适用场景和交付方式。
- [视频工作流程](references/video-workflow.md) 说明如何看回放、截图、对齐文字和核对时间戳。
- [HTML 模板](assets/transcript.html) 提供目录、发言段落和图注的排版，内含虚构示例。

本仓库使用 [MIT 许可证](LICENSE)。
