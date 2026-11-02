# Awesome Remotion [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**English** | [简体中文](readme.zh-CN.md)

> 用 React 和 Remotion 制作视频的精选资源列表。

Remotion 是一个用 React 以代码方式创作视频的框架：你编写组件、用 Hook 驱动动画，然后渲染成 MP4、WebM、GIF 或静帧图片——可以在本地、服务器或云端完成。本列表收录官方工具、社区包、模板、示例和学习资料，帮你更快交付。

欢迎参与贡献。提交 PR 前请先阅读[贡献指南](contributing.md)（英文），其中包含专门针对 AI 编程代理的规则说明。

## 目录

- [官方资源](#官方资源)
- [文档](#文档)
- [软件包](#软件包)
  - [核心](#核心)
  - [渲染](#渲染)
  - [媒体](#媒体)
  - [文本与字幕](#文本与字幕)
  - [动画与特效](#动画与特效)
  - [集成](#集成)
  - [开发工具](#开发工具)
- [模板](#模板)
- [组件](#组件)
- [示例](#示例)
- [完整项目](#完整项目)
- [工具](#工具)
- [教程](#教程)
- [文章](#文章)
- [案例研究](#案例研究)
- [社区](#社区)

## 官方资源

- [Remotion](https://www.remotion.dev) - 官方网站与文档。
- [Remotion on GitHub](https://github.com/remotion-dev/remotion) - 源码、Issue 与发布说明。
- [Remotion Blog](https://www.remotion.dev/blog) - 产品公告、版本说明与工程深度文章。
- [Showcase](https://www.remotion.dev/showcase) - 用 Remotion 制作的视频、广告与产品。
- [Success Stories](https://www.remotion.dev/success-stories) - 公司用 Remotion 落地视频功能的案例。
- [Experts](https://www.remotion.dev/experts) - 与 Remotion 相关的自由职业者与服务商名录。
- [Remotion Pro](https://www.remotion.pro) - 官方团队的付费组件、模板与 Starter 套件。
- [Brand](https://github.com/remotion-dev/brand) - 官方 Logo 与品牌资产仓库，其本身就用 Remotion 制作。

## 文档

- [Installation](https://www.remotion.dev/docs) - 新建项目，或把 Remotion 接入现有应用。
- [Your First Video](https://www.remotion.dev/docs/your-first-video) - 一步一步构建、预览并渲染你的第一个视频。
- [API Reference](https://www.remotion.dev/docs/api) - 核心 API 的全部组件、Hook 与函数。
- [Parameterized Rendering](https://www.remotion.dev/docs/parameterized-rendering) - 通过输入 props 制作可复用、数据驱动的视频。
- [Rendering](https://www.remotion.dev/docs/render) - 从 CLI、Node.js 或云端渲染视频。
- [Player](https://www.remotion.dev/docs/player) - 在 Web 应用中嵌入实时 Remotion 预览。
- [Lambda](https://www.remotion.dev/docs/lambda) - 用 AWS Lambda 弹性扩缩渲染。
- [Cloud Run](https://www.remotion.dev/docs/cloudrun) - 在 Google Cloud Run 上渲染。
- [Studio](https://www.remotion.dev/docs/studio) - 在浏览器中预览、拖动时间轴并检查合成。
- [Captions](https://www.remotion.dev/docs/captions) - 创建、导入字幕并设置样式。
- [Effects](https://www.remotion.dev/docs/effects) - 为视频与元素应用视觉效果。
- [Mediabunny](https://www.remotion.dev/docs/mediabunny) - 在浏览器中读写媒体文件。
- [Server-Side Rendering](https://www.remotion.dev/docs/ssr) - 从 Node.js 服务器渲染视频。
- [Client-Side Rendering](https://www.remotion.dev/docs/client-side-rendering) - 在浏览器中渲染或预览视频。
- [Import from Figma](https://www.remotion.dev/docs/figma) - 把 Figma 设计稿导入合成。
- [Import from After Effects](https://www.remotion.dev/docs/after-effects) - 把 After Effects 项目导入 Remotion。
- [Import from Spline](https://www.remotion.dev/docs/spline) - 把 Spline 3D 场景导入 Remotion。
- [Canvas Capture](https://www.remotion.dev/docs/canvas-capture) - 把画布中的 HTML 内容捕获为视频。
- [Timeline](https://www.remotion.dev/docs/timeline) - 用于编辑器界面的可定制多轨时间轴组件（付费）。
- [Editor Starter](https://www.remotion.dev/docs/editor-starter) - 构建自己的视频编辑器的起步模板（付费）。
- [AI](https://www.remotion.dev/docs/ai) - 在 Remotion 中使用编程代理与 AI 工具。
- [Troubleshooting](https://www.remotion.dev/docs/troubleshooting/debug-failed-render) - 排查渲染失败与常见错误。
- [License](https://www.remotion.dev/docs/license) - 了解公司授权与使用条款。
- [Resources](https://www.remotion.dev/docs/resources) - 官方维护的社区示例、模板与工具列表。

## 软件包

官方发布在 `@remotion` scope 下的 npm 包。

### 核心

- [remotion](https://www.npmjs.com/package/remotion) - 核心包，包含 `Composition`、`Sequence`、`useCurrentFrame` 等全部视频 API。
- [@remotion/cli](https://www.npmjs.com/package/@remotion/cli) - `npx remotion` 命令，用于预览与渲染合成。
- [@remotion/renderer](https://www.npmjs.com/package/@remotion/renderer) - 用 Node.js 或 Bun 渲染视频。
- [@remotion/bundler](https://www.npmjs.com/package/@remotion/bundler) - 用 Webpack 打包合成。
- [@remotion/player](https://www.npmjs.com/package/@remotion/player) - 在 React 应用中嵌入实时 Remotion 预览。
- [@remotion/studio](https://www.npmjs.com/package/@remotion/studio) - 与 Remotion Studio 交互的 API。
- [@remotion/web-renderer](https://www.npmjs.com/package/@remotion/web-renderer) - 完全在浏览器中渲染视频。

### 渲染

- [@remotion/lambda](https://www.npmjs.com/package/@remotion/lambda) - 在 AWS Lambda 上渲染视频。
- [@remotion/cloudrun](https://www.npmjs.com/package/@remotion/cloudrun) - 在 Google Cloud Run 上渲染视频。
- [@remotion/vercel](https://www.npmjs.com/package/@remotion/vercel) - 在 Vercel Sandbox 上渲染视频。
- [@remotion/serverless](https://www.npmjs.com/package/@remotion/serverless) - 分布式渲染运行时。
- [@remotion/licensing](https://www.npmjs.com/package/@remotion/licensing) - 管理 Remotion Pro 授权。

### 媒体

- [@remotion/media](https://www.npmjs.com/package/@remotion/media) - 基于 WebCodecs 的实验性媒体标签，播放更精准。
- [@remotion/media-utils](https://www.npmjs.com/package/@remotion/media-utils) - 处理音视频文件的工具函数。
- [@remotion/media-parser](https://www.npmjs.com/package/@remotion/media-parser) - 纯 JavaScript 的视频文件解析库。
- [@remotion/video](https://www.npmjs.com/package/@remotion/video) - 实验性视频嵌入标签，可靠且帧准确。
- [@remotion/gif](https://www.npmjs.com/package/@remotion/gif) - 在 Remotion 视频中嵌入 GIF。
- [@remotion/webcodecs](https://www.npmjs.com/package/@remotion/webcodecs) - 在浏览器中转换媒体。
- [@remotion/canvas-capture](https://www.npmjs.com/package/@remotion/canvas-capture) - 把画布中的 HTML 内容捕获为视频。
- [@remotion/video-matting](https://www.npmjs.com/package/@remotion/video-matting) - 在浏览器中把视频分离为背景层与透明前景层。

### 文本与字幕

- [@remotion/captions](https://www.npmjs.com/package/@remotion/captions) - 创建与排版字幕的基础组件。
- [@remotion/google-fonts](https://www.npmjs.com/package/@remotion/google-fonts) - 在合成中加载 Google Fonts。
- [@remotion/fonts](https://www.npmjs.com/package/@remotion/fonts) - 在 Remotion 中加载本地字体。
- [@remotion/animated-emoji](https://www.npmjs.com/package/@remotion/animated-emoji) - Google Fonts 动态 Emoji 组件。
- [@remotion/layout-utils](https://www.npmjs.com/package/@remotion/layout-utils) - 测量与适配文本及其他布局元素。
- [@remotion/rounded-text-box](https://www.npmjs.com/package/@remotion/rounded-text-box) - 创建 TikTok 风格的圆角多行文本框。
- [@remotion/sfx](https://www.npmjs.com/package/@remotion/sfx) - 视频用音效库。
- [@remotion/install-whisper-cpp](https://www.npmjs.com/package/@remotion/install-whisper-cpp) - 安装并使用 Whisper.cpp 进行语音转写。
- [@remotion/whisper-web](https://www.npmjs.com/package/@remotion/whisper-web) - 用 WASM 在浏览器中运行 Whisper.cpp。
- [@remotion/whisper-webgpu](https://www.npmjs.com/package/@remotion/whisper-webgpu) - 用 Whisper 与 WebGPU 在浏览器中转写音频。
- [@remotion/openai-whisper](https://www.npmjs.com/package/@remotion/openai-whisper) - 处理 OpenAI Whisper API 的输出。

### 动画与特效

- [@remotion/animation-utils](https://www.npmjs.com/package/@remotion/animation-utils) - CSS 属性动画辅助函数。
- [@remotion/transitions](https://www.npmjs.com/package/@remotion/transitions) - 在场景之间组合转场。
- [@remotion/motion-blur](https://www.npmjs.com/package/@remotion/motion-blur) - 为动画添加运动模糊。
- [@remotion/paths](https://www.npmjs.com/package/@remotion/paths) - 动画化并测量 SVG 路径。
- [@remotion/shapes](https://www.npmjs.com/package/@remotion/shapes) - 生成 SVG 形状。
- [@remotion/noise](https://www.npmjs.com/package/@remotion/noise) - 用于自然运动的噪声函数。
- [@remotion/light-leaks](https://www.npmjs.com/package/@remotion/light-leaks) - 用于转场与叠层的漏光特效。
- [@remotion/starburst](https://www.npmjs.com/package/@remotion/starburst) - 星芒放射特效。
- [@remotion/rough-notation](https://www.npmjs.com/package/@remotion/rough-notation) - 手绘风标注组件。
- [@remotion/svg-3d-engine](https://www.npmjs.com/package/@remotion/svg-3d-engine) - 3D SVG 挤出特效。
- [@remotion/gsap](https://www.npmjs.com/package/@remotion/gsap) - 用 GSAP 时间轴驱动 Remotion 帧。
- [@remotion/effects](https://www.npmjs.com/package/@remotion/effects) - 面向 canvas 组件的特效。
- [@remotion/mac-cursors](https://www.npmjs.com/package/@remotion/mac-cursors) - macOS 光标组件。

### 集成

- [@remotion/three](https://www.npmjs.com/package/@remotion/three) - 在视频中使用 React Three Fiber 组件。
- [@remotion/skia](https://www.npmjs.com/package/@remotion/skia) - 在视频中使用 React Native Skia 组件。
- [@remotion/lottie](https://www.npmjs.com/package/@remotion/lottie) - 嵌入 Lottie 动画。
- [@remotion/rive](https://www.npmjs.com/package/@remotion/rive) - 嵌入 Rive 动画。
- [@remotion/p5](https://www.npmjs.com/package/@remotion/p5) - 在合成中使用 p5.js 画作。
- [@remotion/maptiler](https://www.npmjs.com/package/@remotion/maptiler) - MapTiler 地图组件。
- [@remotion/elevenlabs](https://www.npmjs.com/package/@remotion/elevenlabs) - 处理 ElevenLabs API 生成的音频。

### 开发工具

- [@remotion/eslint-plugin](https://www.npmjs.com/package/@remotion/eslint-plugin) - 编写 Remotion 代码的 ESLint 规则。
- [@remotion/eslint-config-flat](https://www.npmjs.com/package/@remotion/eslint-config-flat) - Remotion 项目的默认 ESLint 扁平配置。
- [@remotion/zod-types](https://www.npmjs.com/package/@remotion/zod-types) - 用于合成 props 的 Zod 模式。
- [@remotion/tailwind-v4](https://www.npmjs.com/package/@remotion/tailwind-v4) - Tailwind CSS v4 支持。
- [@remotion/tailwind](https://www.npmjs.com/package/@remotion/tailwind) - Tailwind CSS v3 支持。
- [@remotion/enable-scss](https://www.npmjs.com/package/@remotion/enable-scss) - 在 Remotion 中启用 SCSS。
- [@remotion/codemods](https://www.npmjs.com/package/@remotion/codemods) - 升级 Remotion 项目的代码转换脚本。
- [@remotion/player-a11y](https://www.npmjs.com/package/@remotion/player-a11y) - Player 的无障碍封装，符合 WCAG 控制。
- [@remotion/drag-and-drop](https://www.npmjs.com/package/@remotion/drag-and-drop) - 构建与解析拖放载荷。

## 模板

来自[官方模板目录](https://www.remotion.dev/templates)的起步模板。

- [Hello World](https://www.remotion.dev/templates/hello-world) - 附带简单动画的示例场，适合第一个项目。
- [Blank](https://www.remotion.dev/templates/blank) - 空白画布，没有任何多余内容。
- [Next.js](https://www.remotion.dev/templates/next) - 视频生成应用的 SaaS 起步模板。
- [React Router 7](https://www.remotion.dev/templates/react-router) - 基于 React Router 7 的 SaaS 起步模板。
- [Vercel Sandbox](https://www.remotion.dev/templates/vercel) - 用 Vercel Sandbox 按需渲染视频。
- [Render Server](https://www.remotion.dev/templates/render-server) - 用于渲染视频的 Express 服务器。
- [Electron](https://www.remotion.dev/templates/electron) - 从桌面应用渲染视频。
- [Recorder](https://www.remotion.dev/templates/recorder) - 纯 JavaScript 打造的视频制作工具。
- [3D](https://www.remotion.dev/templates/three) - React Three Fiber 起步模板。
- [Skia](https://www.remotion.dev/templates/skia) - React Native Skia 起步模板。
- [Stills](https://www.remotion.dev/templates/still) - 内置服务器的动态 PNG/JPEG 图片模板。
- [Audiogram](https://www.remotion.dev/templates/audiogram) - 播客的文字与声波可视化。
- [Music Visualization](https://www.remotion.dev/templates/music-visualization) - 音乐反应式可视化。
- [Overlay](https://www.remotion.dev/templates/overlay) - 为视频剪辑软件设计的叠层合成。
- [Code Hike](https://www.remotion.dev/templates/code-hike) - 精美的代码动画。
- [TikTok](https://www.remotion.dev/templates/tiktok) - 逐词出现的动画字幕。
- [Stargazer](https://www.remotion.dev/templates/stargazer) - 用视频庆祝仓库获得星标。
- [Prompt to Video](https://www.remotion.dev/templates/prompt-to-video) - 把一段提示词变成带旁白的图像故事。
- [Prompt to Motion Graphics](https://www.remotion.dev/templates/prompt-to-motion-graphics) - AI 动画生成的 SaaS 起步模板。
- [Element Library](https://www.remotion.dev/templates/element-library) - 构建并发布你自己的 Remotion 元素库。
- [Editor Starter](https://www.remotion.dev/templates/editor-starter) - 打造自己视频编辑器的起步模板（付费）。

社区模板：

- [Remotion TTS Example](https://github.com/FelippeChemello/Remotion-TTS-Example) - 使用 Azure 的文字转语音。
- [Remotion gTTS Template](https://github.com/thecmdrunner/remotion-gtts-template) - 使用 Google 的文字转语音。
- [Docker Build and Render](https://github.com/scotthavird/remotion-docker-template) - 容器化的构建与渲染流水线。
- [Monorepo Template](https://github.com/Takamasa045/remotion-studio-monorepo) - 在 Monorepo 中共享多个组件。
- [DevContainer Template](https://github.com/openscript/remotion-devcontainer-template) - 可复现的开发容器。
- [Library Starter](https://github.com/remotion-dev/library-starter) - 发布 Remotion 库的最佳实践。
- [Remotion on Railway](https://railway.com/deploy/remotion-on-rails) - 一键部署模板。
- [Quote Shorts](https://github.com/developk/remotion-quote-shorts) - 从单个内容文件渲染的竖版引言视频。

## 组件

- [Remocn](https://remocn.dev) - 可复制粘贴的动画组件、转场、背景与场景。
- [Remotion UI](https://github.com/riaz37/remotion-ui) - 源码归你所有的成品动效组件与合成。
- [Remotion Bits](https://remotion-bits.dev) - 现成的动画组件、图表、转场与文字显现。
- [Onda](https://onda.video) - Remotion 的开源动效组件库。
- [Snapcn](https://snapcn.dev) - shadcn 风格的 Remotion 组件注册表，用 CLI 安装。
- [React Video Editor Templates](https://www.reactvideoeditor.com/remotion-templates) - 开源视频编辑器与时间轴组件。
- [TikTok Text Box](https://github.com/KyleTryon/TikTokTextBox) - TikTok 风格的多行文本框。
- [Remotion Animated](https://www.remotion-animated.dev) - Remotion 的声明式动画辅助库。
- [remotion-transition-series](https://github.com/marcusstenbeck/remotion-transition-series) - 基于 Remotion Transitions 的序列转场。
- [remotion-time](https://github.com/fwextensions/remotion-time) - Remotion 的时间辅助工具。
- [remotion-animate-text](https://github.com/pskd73/remotion-animate-text) - 文本动画辅助组件。
- [remotion-subtitles](https://github.com/ahgsql/remotion-subtitles) - Remotion 字幕组件。
- [Remotion Glitch Effect](https://github.com/storybynumbers/remotion-glitch-effect) - 故障风特效组件。
- [Clippkit](https://www.clippkit.com) - 免费 Remotion 组件。
- [SwiftClip](https://github.com/zz41354899/SwiftClip) - 30 个生产可用的 Remotion 模板。
- [RenderComp Free](https://github.com/RenderComp/free-remotion-templates) - 50 个 MIT 协议的 Remotion 模板。
- [cliphou.se](https://cliphou.se/remotion-templates) - 免费 MIT-0 模板，文字与颜色可编辑。
- [Lexington Motion](https://lexingtonthemes.com/remotion) - 适配社交媒体的无缝循环宣传模板（付费）。

## 示例

- [HTML in Canvas](https://github.com/remotion-dev/html-in-canvas) - 官方的画布 HTML 捕获为视频示例。
- [Typewriter Effect](https://github.com/remotion-dev/typewriter) - 经典打字机动画。
- [D3.js Charts](https://github.com/remotion-dev/d3-example) - 逐帧驱动 D3 可视化。
- [Tone.js Music](https://github.com/remotion-dev/tone-js-example) - 用 Tone.js 生成音乐。
- [Animated GLB Models](https://github.com/remotion-dev/glb-example) - 加载并动画化 glTF 模型。
- [3D Text](https://github.com/remotion-dev/3d-text) - 挤出效果的 3D 文字。
- [Text Morphing](https://github.com/remotion-dev/morph-text) - 在文字与形状之间变形。
- [Text Warping](https://github.com/remotion-dev/text-warping) - 让文字沿路径弯曲。
- [OpenGL Transitions](https://github.com/remotion-dev/remotion-gl-transitions) - 基于着色器的场景转场。
- [Light Leak Transition](https://github.com/remotion-dev/light-leak-example) - 漏光转场特效。
- [CSS Animations](https://github.com/remotion-dev/css-animation-play-state) - 用帧驱动 CSS 动画。
- [Jump Cuts](https://github.com/remotion-dev/video-with-jump-cuts) - 不重新挂载视频实现跳剪。
- [Measure a DOM Node](https://github.com/remotion-dev/measure-item) - 测量已渲染的元素。
- [Anime.js](https://github.com/remotion-dev/anime-example) - 使用 Anime.js 时间轴。
- [Mapbox](https://github.com/remotion-dev/mapbox-example) - Mapbox 地图动画。
- [MapLibre](https://github.com/remotion-dev/maplibre-example) - MapLibre 地图动画。
- [Three.js Particles](https://github.com/JonnyBurger/three-particles) - Three.js 粒子系统。
- [Apple Spring Animation](https://github.com/JonnyBurger/spring-loaded) - 复刻 Apple 的弹簧加载动画。
- [Wavy TikTok Effect](https://github.com/JonnyBurger/wavy-meme) - TikTok 风格的波浪特效。
- [Matter.js Pool Game](https://github.com/hylarucoder/remotion-physics) - Matter.js 物理模拟。
- [Bar Race Chart](https://github.com/hylarucoder/remotion-bar-race-chart) - 动画条形竞赛图。
- [Globe.gl](https://github.com/alexfernandez803/remotion-globegl) - 带弧线与标记点的 3D 地球。
- [Shader A-Roll](https://github.com/onion2k/a-roll) - 着色器驱动的视频特效。
- [12+ Examples](https://remotion-example.vercel.app) - 社区示例合集。

## 完整项目

- [GitHub Unwrapped](https://github.com/remotion-dev/github-unwrapped) - 为 GitHub 用户生成的年度代码回顾视频。
- [GitHub Unwrapped 2022](https://github.com/remotion-dev/github-unwrapped-2022) - GitHub Unwrapped 2022 版。
- [GitHub Unwrapped 2021](https://github.com/remotion-dev/github-unwrapped-2021) - GitHub Unwrapped 2021 版。
- [Remotion Trailer](https://github.com/remotion-dev/trailer) - Remotion 官方宣传片。
- [Remotion Wrapped](https://github.com/JonnyBurger/remotion-wrapped) - Remotion 创始人复刻的 Spotify Wrapped 动画。
- [Fireship-Style Videos](https://github.com/wcandillon/remotion-fireship) - 用 React 和 Remotion 复刻 Fireship 风格视频的完整源码。
- [Podcast Maker](https://github.com/FelippeChemello/podcast-maker) - 用动效与文字转语音把新闻简报变成每日 YouTube 视频。
- [Mockoops](https://github.com/Just-Moh-it/Mockoops) - 把无聊的屏幕录像变成精美的设备样机动画。
- [Product Hunt Today](https://github.com/Kamigami55/product-hunt-today) - 每日 Product Hunt 回顾视频。
- [Remotion Weather](https://github.com/florentpergoud/remotion-weather) - 法国天气预报视频生成器。
- [Rewind Table](https://github.com/gregonarash/rewind-table) - 以 Airtable 为数据源制作程序化视频。
- [Motionly](https://github.com/karelnagel/motionly) - 支持动态数据渲染的开源视频编辑器。
- [DataVids](https://github.com/apsquared/datavids_public) - 数据驱动的视频生成。
- [Social Video Generator](https://github.com/lyonjs/social-video-generator) - 会议讲者公布卡片视频。
- [Auto Reel Edit](https://github.com/sieve-community/auto-reel-edit) - 竖版短视频的加字幕与背景替换。
- [OpenMontage](https://github.com/calesthio/OpenMontage) - 开源的代理式视频制作系统。
- [OpenChatCut](https://github.com/0xsline/OpenChatCut) - 开源、本地优先的对话式 AI 视频编辑器，带多轨时间轴。
- [Kimu Video Editor](https://github.com/trykimu/videoeditor) - 基于 Remotion 的 CapCut 与 Canva 开源替代品。
- [clip-js](https://github.com/mohyware/clip-js) - 用 Next.js、Remotion 与 WASM 版 FFmpeg 构建的在线视频编辑器。
- [React Video Editor](https://github.com/openvideodev/react-video-editor) - CapCut 与 Canva 的开源克隆。
- [Short Video Maker](https://github.com/gyoridavid/short-video-maker) - 通过 MCP 与 REST API 为 TikTok、Reels 和 YouTube 制作短视频。
- [Cinetic](https://github.com/Leonxlnx/cinetic) - 由编程代理执导的电影感发布片与动效设计。
- [Vanta](https://github.com/itsjwill/vanta) - 开源 AI 视频引擎，支持声音克隆、数字人、字幕与 100+ 转场。

## 工具

- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=KarelNagel.remotion-vscode) - 在 VS Code 内预览与检查合成。
- [Agent Skills](https://www.remotion.dev/docs/ai/skills) - 教编程代理使用 Remotion 的官方技能。
- [Claude Code Plugin](https://github.com/remotion-dev/claude-code-plugin) - 官方 Remotion 技能打包的 Claude Code 插件。
- [Video Shotcraft](https://github.com/Vincentwei1021/video-shotcraft) - 制作电影感、可编辑产品宣传片的代理技能。
- [GitHub Actions Matrix Renderer](https://github.com/yuvraj108c/Remotion-Matrix-Renderer) - 把渲染拆分到 GitHub Actions 矩阵任务以提速。
- [Rustymotion](https://github.com/clearlysid/rustymotion) - 实验性的 Rust 版 Remotion 视频渲染器。
- [Remotion QA](https://github.com/GroMarketing/remotion-qa) - 检查成片的安全区、空气静默与字幕可读性。

## 教程

- [Fireship: Remotion Tutorial](https://www.youtube.com/watch?v=deg8bOoziaE) - 快节奏的 React 视频制作入门。
- [Spotify Wrapped 2020](https://www.youtube.com/watch?v=I-y_5H9-3gk) - 复刻 Spotify Wrapped 式的年度回顾。
- [Spotify Wrapped 2025](https://www.youtube.com/watch?v=WAjO-M_Q9C0) - 更新版 Spotify Wrapped 制作。
- [Programmatic Stories](https://www.youtube.com/watch?v=70UdF6DWY3M) - 制作 Instagram 风格的快拍视频。
- [Basketball Tracker](https://www.youtube.com/watch?v=A8miHLSf_BI) - 制作体育追踪图形。
- [Formula 1 Graphics](https://www.youtube.com/watch?v=sA-X0Bw_7Gg) - 制作 F1 风格的转播图形。
- [Football Graphics](https://www.youtube.com/watch?v=BI8IWwaDt8s) - 制作足球转播图形。
- [Remotion Skia Tutorial](https://www.youtube.com/watch?v=-7MOoWN2_nk) - 用 React Native Skia 实现高性能图形。
- [DVD Screensaver](https://www.youtube.com/watch?v=n69siyttEwM) - 制作弹跳的 DVD 待机画面。
- [Timing Animations](https://www.youtube.com/watch?v=WigIALCnEvw) - 理解帧、时序与插值。
- [Podcast Video with AI](https://www.youtube.com/watch?v=EGxBBL91nRM) - 用 Remotion 与 AI 制作播客视频。
- [Alfonso Graziano's Tutorial](https://www.youtube.com/watch?v=r4v1J7ozxIg) - 以项目为导向的 Remotion 讲解。
- [GSAP Timelines in Remotion](https://www.remotion.dev/docs/gsap) - 用 GSAP 时间轴驱动动画。

## 文章

- [Create Videos with Code](https://prismic.io/blog/create-videos-with-code-remotion-tutorial) - Prismic 的 Remotion 视频制作教程。
- [Remotion on Rails](https://medium.com/@viveknathani/remotion-on-rails-0852acc9595e) - 把 Remotion 部署到 Railway。

## 案例研究

来自官方 Success Stories 页面的公司实践。

- [Typeframes](https://www.remotion.dev/success-stories/typeframes) - 几分钟内生成产品宣传视频的 SaaS。
- [MakeStories](https://www.remotion.dev/success-stories/makestories) - 批量渲染 Web Stories 的平台。
- [shortvid.io](https://www.remotion.dev/success-stories/shortvid) - 自动生成会议宣传素材，且已开源源码。

## 社区

- [Discord](https://www.remotion.dev/discord) - 官方社区聊天：提问、展示与讨论。
- [X](https://x.com/remotion) - 产品动态与社区视频。
- [YouTube](https://www.youtube.com/@remotion_dev) - 官方教程、演讲与演示。
- [Instagram](https://www.instagram.com/remotion) - 用 Remotion 制作的短视频。
- [LinkedIn](https://www.linkedin.com/company/remotion) - 公司动态与招聘信息。
- [GitHub Organization](https://github.com/remotion-dev) - 全部官方仓库。
- [GitHub Topic](https://github.com/topics/remotion) - 打了 Remotion 标签的社区项目。
- [Reddit](https://www.reddit.com/r/remotion/) - 提问与展示作品的社区论坛。
- [Support](https://www.remotion.dev/docs/support) - 官方支持渠道与响应时效。

## 相关列表

- [Awesome React](https://github.com/enaqx/awesome-react) - React 资源精选列表。
- [Awesome Creative Coding](https://github.com/terkelg/awesome-creative-coding) - 生成艺术与创意编码资源。
- [Awesome FFmpeg](https://github.com/transitive-bullshit/awesome-ffmpeg) - FFmpeg 工具、脚本与资源。
- [Awesome Video](https://github.com/krzemienski/awesome-video) - 视频工程、流媒体与工具。

## 参与贡献

欢迎参与贡献。请先阅读[贡献指南](contributing.md)（英文），再提交 Issue 或 Pull Request，并在本地运行 `npx awesome-lint` 检查改动。参与即表示你同意遵守[行为准则](code-of-conduct.md)（英文）。
