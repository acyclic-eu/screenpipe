<h1 align="center">OysterWorkflow 适配版 Screenpipe</h1>

这是 ShuxinYang111 维护的
[screenpipe](https://github.com/mediar-ai/screenpipe) fork，基于上游
Screenpipe `v0.3.304` 系列，面向
[OysterWorkflow Core](https://github.com/ShuxinYang111/oysterworkflow-core)
做了兼容适配。

推荐用户直接在 OysterWorkflow Core 仓库中执行：

```bash
npm run screenpipe:install
npm run screenpipe:start
```

手动源码构建方式：

```bash
git clone https://github.com/ShuxinYang111/screenpipe.git
cd screenpipe
git checkout oysterworkflow-compatible-v0.3.304
cargo build --release

./target/release/screenpipe \
  --port 3030 \
  --disable-audio \
  --fps 1 \
  --language chinese \
  --language english
```

主要适配内容包括：稳定的中英文 OCR 语言顺序、macOS Apple Vision
语言代码处理、`--disable-system-audio`、最终音频片段 flush、音频搜索和空转写
marker 修复，以及 OysterWorkflow ingest 所需的 UI events 兼容性；当前 recorder
配置会启用 UI event capture，不需要额外传旧版 UI 参数。

感谢原始 Screenpipe 项目作者
[louis030195](https://github.com/louis030195)、
[Mediar](https://github.com/mediar-ai) 和所有 Screenpipe 贡献者。根目录代码仍保留
上游 MIT License，`ee/` 目录仍保留 Screenpipe Enterprise Edition License。

---

<img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=c3628864-a0cb-47a1-a822-2f936cff50b2" />

<p align="center">
   <a href ="https://screenpi.pe">
      <img src="https://github.com/user-attachments/assets/d3b1de26-c3c0-4c84-b9c4-b03213b97a30" alt="logo" width="200">
   </a>
</p>

<p align="center">
   <a href="README.md">English</a> | <a href="README-zh_CN.md">简体中文</a> | <a href="README-ja.md">日本語</a>
</p>

<h1 align="center">[ screenpipe ]</h1>


<p align="center">桌面的 24/7 记忆</p>
<p align="center">开源版 rewind。100% 本地运行。数据完全属于你。</p>



<p align="center">
   <a href ="https://screenpi.pe">
      <img src="https://github.com/user-attachments/assets/c88d218e-40a7-405d-b419-eec1553ea287" alt="logo" width="800">
   </a>
</p>

<p align="center">
    <a href="https://screenpi.pe" target="_blank">
        <img src="https://img.shields.io/badge/下载-桌面应用-black?style=for-the-badge" alt="下载">
    </a>
    <a href="https://github.com/screenpipe/screenpipe/releases?q=mcp-v&expanded=true" target="_blank">
        <img src="https://img.shields.io/badge/安装-Claude%20扩展-D97706?style=for-the-badge&logo=anthropic&logoColor=white" alt="安装 claude 扩展">
    </a>
</p>

<p align="center">
    <a href="https://discord.gg/screenpipe">
        <img src="https://img.shields.io/discord/823813159592001537?color=5865F2&logo=discord&logoColor=white&style=flat-square" alt="discord">
    </a>
    <a href="https://twitter.com/screenpipe">
        <img alt="x" src="https://img.shields.io/twitter/url/https/twitter.com/diffuserslib.svg?style=social&label=关注%20%40screenpipe">
    </a>
</p>

<br>


![image](https://github.com/user-attachments/assets/dec2e07c-b3d5-46dd-9f36-c0c26a82c9fb)


---

## 这是什么？

screenpipe 全天候录制你的屏幕和音频，所有数据存储在本地，让你将数字历史与 AI 连接起来。

```
┌─────────────────────────────────────────┐
│  屏幕 + 音频 → 本地存储 → AI            │
└─────────────────────────────────────────┘
```

- **记住一切** - 永远不会忘记你看到、听到或做过的事情
- **AI 搜索** - 用自然语言查找任何内容
- **100% 本地** - 你的数据永远不会离开你的设备
- **开源** - 可检查、可修改、完全拥有

## 安装

[下载桌面应用](https://screenpi.pe) — 支持 macOS、Windows、Linux

## 配置要求

- 10% CPU 使用率
- 4GB 内存
- 约 15GB 存储/月
- 支持离线运行

---

<p align="center">
    <a href="https://docs.screenpi.pe">文档</a> ·
    <a href="https://discord.gg/screenpipe">discord</a> ·
    <a href="https://twitter.com/screenpipe">x</a>
</p>
