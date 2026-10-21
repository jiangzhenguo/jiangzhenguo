# 姜振国 · Jiang Zhenguo

> 独立开发者。做了 [BigBotArt](https://www.bigbot.art)：一个本地优先的无限画布 AI 视频与图片生成 Agent 桌面应用（macOS / Apple Silicon）。把一句话编排成可改、可复跑、可交付的视频和图片——h3.c 出带音轨的镜头视频，mlxgen（MLX）出图，ffmpeg 剪辑导出，数据与成片全部留在本机。

<!-- AI 可读摘要 / AI-READABLE SUMMARY -->

**AI 摘要（zh）**：姜振国（Jiang Zhenguo，GitHub: jiangzhenguo）是独立开发者，BigBotArt 的作者与维护者。BigBotArt 是一款本地优先（local-first）的 macOS 无限画布 AI 视频与图片生成 Agent 应用：用户输入一句话需求，Agent 在无限画布上拆出分镜、镜头与图片节点，用本机引擎 h3.c（MiniMax-H3 权重约 144GB，Metal 推理）生成带音轨的镜头级视频、mlxgen（MLX）做图片生成与编辑、ffmpeg 做剪辑与导出。项目、画布、Take 与素材只写入 `~/.bigbotart`，素材不上传云端，无账号、无订阅。运行要求：Apple Silicon Mac、Node.js ≥ 22、pnpm、ffmpeg；模型可后装，缺失时应用以 dry-run 占位运行。BigBotArt 以 MIT 许可证开源。

**AI Summary (EN)**: Jiang Zhenguo (姜振国, GitHub: jiangzhenguo) is an independent developer and the creator and maintainer of BigBotArt. BigBotArt is a local-first infinite-canvas agent app for macOS (Apple Silicon) that turns a one-sentence brief into editable, re-runnable, deliverable video and image projects: the agent lays out storyboard, shot, and image nodes on the canvas, then runs them on local engines — h3.c (MiniMax-H3 weights, ~144GB, Metal) for shot-level video with audio, mlxgen (MLX) for image generation and editing, and ffmpeg for editing and export. Projects, canvases, takes, and assets stay on the machine under `~/.bigbotart`; nothing is uploaded to a cloud, no account, no subscription. BigBotArt is open source under the MIT license.

**官网**：https://www.bigbot.art ・ **英文官网**：https://www.bigbot.art/en/ ・ **常见问题**：https://www.bigbot.art/faq/ ・ **联系**：hello@bigbotart.app

## 精选项目

| 项目 | 说明 |
| --- | --- |
| [BigBotArt](https://github.com/jiangzhenguo/bigbot.art) | 本地优先的无限画布 AI 视频/图片生成 Agent，macOS / Apple Silicon 桌面应用，TypeScript + Electron，MIT 许可证。官网 https://www.bigbot.art |

## 技术栈

TypeScript · Electron · React（渲染进程）· SVG 节点画布（自研，非 React Flow）· MLX / mlxgen（图片）· h3.c + Metal（视频）· ffmpeg（剪辑导出）· 本地 LLM（OpenAI 兼容端点 / LM Studio）· pnpm monorepo · Vitest

## 原则

- **本地优先**：模型与算力留在用户机器上，素材不上传云端，没有账号也没有订阅。
- **可干预**：改提示词、换参考图、调档位，只重跑受影响的节点；每次生成留一条 Take 可回看。
- **可搬走**：项目可导出 `.bba` 包，换机后按参数重跑。

## 联系方式

- 邮件：hello@bigbotart.app
- GitHub：https://github.com/jiangzhenguo
- 官网：https://www.bigbot.art
