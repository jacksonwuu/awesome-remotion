# Awesome Remotion [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English](readme.md) | **简体中文**

> A curated list of awesome resources for building videos with React and Remotion.

Remotion is a framework for creating videos programmatically with React. You write components, animate them with hooks, and render them to MP4, WebM, GIF, or still images — locally, on a server, or in the cloud. This list collects the official tooling, community packages, templates, examples, and learning material that help you ship faster.

Contributions are welcome. See [Contributing](#contributing) before opening a pull request.

## Contents

- [Official](#official)
- [Documentation](#documentation)
- [Packages](#packages)
  - [Core](#core)
  - [Rendering](#rendering)
  - [Media](#media)
  - [Text and Captions](#text-and-captions)
  - [Animation and Effects](#animation-and-effects)
  - [Integrations](#integrations)
  - [Developer Tooling](#developer-tooling)
- [Templates](#templates)
- [Components](#components)
- [Examples](#examples)
- [Full Projects](#full-projects)
- [Tools](#tools)
- [Tutorials](#tutorials)
- [Articles](#articles)
- [Case Studies](#case-studies)
- [Community](#community)

## Official

- [Remotion](https://www.remotion.dev) - The official website and documentation.
- [Remotion on GitHub](https://github.com/remotion-dev/remotion) - Source code, issues, and release notes.
- [Remotion Blog](https://www.remotion.dev/blog) - Product announcements, release notes, and engineering deep dives.
- [Showcase](https://www.remotion.dev/showcase) - Videos, campaigns, and products made with Remotion.
- [Success Stories](https://www.remotion.dev/success-stories) - Case studies of companies shipping video features with Remotion.
- [Experts](https://www.remotion.dev/experts) - Directory of freelancers and agencies who work with Remotion.
- [Remotion Pro](https://www.remotion.pro) - Paid components, templates, and starter kits from the Remotion team.
- [Brand](https://github.com/remotion-dev/brand) - Official logo and brand assets, made with Remotion itself.

## Documentation

- [Installation](https://www.remotion.dev/docs) - Set up a new project or add Remotion to an existing app.
- [Your First Video](https://www.remotion.dev/docs/your-first-video) - Build, preview, and render a video step by step.
- [API Reference](https://www.remotion.dev/docs/api) - Every component, hook, and function in the core API.
- [Parameterized Rendering](https://www.remotion.dev/docs/parameterized-rendering) - Pass input props to create reusable, data-driven videos.
- [Rendering](https://www.remotion.dev/docs/render) - Render from the CLI, Node.js, or the cloud.
- [Player](https://www.remotion.dev/docs/player) - Embed a live Remotion preview in a web app.
- [Lambda](https://www.remotion.dev/docs/lambda) - Scale rendering across AWS Lambda.
- [Cloud Run](https://www.remotion.dev/docs/cloudrun) - Render on Google Cloud Run.
- [Studio](https://www.remotion.dev/docs/studio) - Preview, scrub, and inspect compositions in the browser.
- [Captions](https://www.remotion.dev/docs/captions) - Create, import, and style subtitles.
- [Effects](https://www.remotion.dev/docs/effects) - Apply visual effects to video and elements.
- [Mediabunny](https://www.remotion.dev/docs/mediabunny) - Read and write media files in the browser.
- [Server-Side Rendering](https://www.remotion.dev/docs/ssr) - Render videos from a Node.js server.
- [Client-Side Rendering](https://www.remotion.dev/docs/client-side-rendering) - Render or preview videos in the browser.
- [Import from Figma](https://www.remotion.dev/docs/figma) - Bring Figma designs into a composition.
- [Import from After Effects](https://www.remotion.dev/docs/after-effects) - Bring After Effects projects into Remotion.
- [Import from Spline](https://www.remotion.dev/docs/spline) - Bring Spline 3D scenes into Remotion.
- [Canvas Capture](https://www.remotion.dev/docs/canvas-capture) - Capture HTML-in-canvas content as a video.
- [Timeline](https://www.remotion.dev/docs/timeline) - A customizable, multi-track timeline component for editor UIs (paid).
- [Editor Starter](https://www.remotion.dev/docs/editor-starter) - A boilerplate for building your own video editor (paid).
- [AI](https://www.remotion.dev/docs/ai) - Use coding agents and AI tools with Remotion.
- [Troubleshooting](https://www.remotion.dev/docs/troubleshooting/debug-failed-render) - Debug failed renders and common errors.
- [License](https://www.remotion.dev/docs/license) - Understand the company license and terms.
- [Resources](https://www.remotion.dev/docs/resources) - The official list of community examples, templates, and tools.

## Packages

Official npm packages published under the `@remotion` scope.

### Core

- [remotion](https://www.npmjs.com/package/remotion) - The core package with `Composition`, `Sequence`, `useCurrentFrame`, and the rest of the video API.
- [@remotion/cli](https://www.npmjs.com/package/@remotion/cli) - The `npx remotion` command for previewing and rendering compositions.
- [@remotion/renderer](https://www.npmjs.com/package/@remotion/renderer) - Render videos with Node.js or Bun.
- [@remotion/bundler](https://www.npmjs.com/package/@remotion/bundler) - Bundle compositions with Webpack.
- [@remotion/player](https://www.npmjs.com/package/@remotion/player) - Embed a live Remotion preview in a React app.
- [@remotion/studio](https://www.npmjs.com/package/@remotion/studio) - APIs for interacting with Remotion Studio.
- [@remotion/studio-server](https://www.npmjs.com/package/@remotion/studio-server) - Run Remotion Studio with a server backend.
- [@remotion/browser-bundler](https://www.npmjs.com/package/@remotion/browser-bundler) - Compile virtual Remotion projects in the browser.
- [@remotion/web-renderer](https://www.npmjs.com/package/@remotion/web-renderer) - Render videos entirely in the browser.

### Rendering

- [@remotion/lambda](https://www.npmjs.com/package/@remotion/lambda) - Render videos on AWS Lambda.
- [@remotion/cloudrun](https://www.npmjs.com/package/@remotion/cloudrun) - Render videos on Google Cloud Run.
<!--lint ignore awesome-spell-check-->
- [Vercel Sandbox](https://www.npmjs.com/package/@remotion/vercel) - Render videos on Vercel Sandbox.
- [@remotion/serverless](https://www.npmjs.com/package/@remotion/serverless) - A runtime for distributed rendering.
- [@remotion/licensing](https://www.npmjs.com/package/@remotion/licensing) - Manage your Remotion Pro license.

### Media

- [@remotion/media](https://www.npmjs.com/package/@remotion/media) - Experimental WebCodecs-based media tags for accurate playback.
- [@remotion/media-utils](https://www.npmjs.com/package/@remotion/media-utils) - Utilities for working with audio and video files.
- [@remotion/media-parser](https://www.npmjs.com/package/@remotion/media-parser) - A pure JavaScript library for parsing video files.
- [@remotion/video](https://www.npmjs.com/package/@remotion/video) - Experimental tag for reliable video embedding.
- [@remotion/gif](https://www.npmjs.com/package/@remotion/gif) - Embed GIFs in a Remotion video.
- [@remotion/webcodecs](https://www.npmjs.com/package/@remotion/webcodecs) - Convert media in the browser.
- [@remotion/canvas-capture](https://www.npmjs.com/package/@remotion/canvas-capture) - Capture HTML-in-canvas content as a video.
- [@remotion/preload](https://www.npmjs.com/package/@remotion/preload) - Preload assets before rendering.
- [@remotion/video-matting](https://www.npmjs.com/package/@remotion/video-matting) - Separate a video into a base layer and a transparent foreground.

### Text and Captions

- [@remotion/captions](https://www.npmjs.com/package/@remotion/captions) - Primitives for creating and styling captions.
- [@remotion/google-fonts](https://www.npmjs.com/package/@remotion/google-fonts) - Load Google Fonts in compositions.
- [@remotion/fonts](https://www.npmjs.com/package/@remotion/fonts) - Load local fonts into Remotion.
- [@remotion/animated-emoji](https://www.npmjs.com/package/@remotion/animated-emoji) - Google Fonts animated emoji as components.
- [@remotion/layout-utils](https://www.npmjs.com/package/@remotion/layout-utils) - Measure and fit text and other layout elements.
- [@remotion/rounded-text-box](https://www.npmjs.com/package/@remotion/rounded-text-box) - Create TikTok-style multiline text boxes.
- [@remotion/sfx](https://www.npmjs.com/package/@remotion/sfx) - A sound effect library for your videos.
- [@remotion/install-whisper-cpp](https://www.npmjs.com/package/@remotion/install-whisper-cpp) - Install and use Whisper.cpp for transcription.
- [@remotion/whisper-web](https://www.npmjs.com/package/@remotion/whisper-web) - Run Whisper.cpp in the browser with WASM.
- [@remotion/whisper-webgpu](https://www.npmjs.com/package/@remotion/whisper-webgpu) - Transcribe audio in the browser with Whisper and WebGPU.
- [@remotion/openai-whisper](https://www.npmjs.com/package/@remotion/openai-whisper) - Work with output from the OpenAI Whisper API.

### Animation and Effects

- [@remotion/animation-utils](https://www.npmjs.com/package/@remotion/animation-utils) - Helpers for animating CSS properties.
- [@remotion/transitions](https://www.npmjs.com/package/@remotion/transitions) - Compose transitions between scenes.
- [@remotion/motion-blur](https://www.npmjs.com/package/@remotion/motion-blur) - Add motion blur to animations.
- [@remotion/paths](https://www.npmjs.com/package/@remotion/paths) - Animate and measure SVG paths.
- [@remotion/shapes](https://www.npmjs.com/package/@remotion/shapes) - Generate SVG shapes.
- [@remotion/noise](https://www.npmjs.com/package/@remotion/noise) - Noise functions for organic motion.
- [@remotion/light-leaks](https://www.npmjs.com/package/@remotion/light-leaks) - Light leak effects for transitions and overlays.
- [@remotion/starburst](https://www.npmjs.com/package/@remotion/starburst) - Starburst ray effects.
- [@remotion/rough-notation](https://www.npmjs.com/package/@remotion/rough-notation) - Rough-notation annotation primitives.
- [@remotion/svg-3d-engine](https://www.npmjs.com/package/@remotion/svg-3d-engine) - 3D SVG extrusion effects.
- [@remotion/gsap](https://www.npmjs.com/package/@remotion/gsap) - Drive Remotion frames with GSAP timelines.
- [@remotion/effects](https://www.npmjs.com/package/@remotion/effects) - Effects for canvas-based components.
- [@remotion/mac-cursors](https://www.npmjs.com/package/@remotion/mac-cursors) - macOS cursor components.

### Integrations

- [@remotion/three](https://www.npmjs.com/package/@remotion/three) - Use React Three Fiber components in a video.
- [@remotion/skia](https://www.npmjs.com/package/@remotion/skia) - Use React Native Skia components in a video.
- [@remotion/lottie](https://www.npmjs.com/package/@remotion/lottie) - Embed Lottie animations.
- [@remotion/rive](https://www.npmjs.com/package/@remotion/rive) - Embed Rive animations.
- [@remotion/p5](https://www.npmjs.com/package/@remotion/p5) - Use p5.js sketches in a composition.
- [@remotion/maptiler](https://www.npmjs.com/package/@remotion/maptiler) - MapTiler map components.
- [@remotion/elevenlabs](https://www.npmjs.com/package/@remotion/elevenlabs) - Work with audio from the ElevenLabs API.

### Developer Tooling

- [@remotion/eslint-plugin](https://www.npmjs.com/package/@remotion/eslint-plugin) - ESLint rules for writing Remotion code.
- [@remotion/eslint-config-flat](https://www.npmjs.com/package/@remotion/eslint-config-flat) - Default ESLint flat config for Remotion projects.
- [@remotion/zod-types](https://www.npmjs.com/package/@remotion/zod-types) - Zod schemas for composition props.
- [@remotion/tailwind-v4](https://www.npmjs.com/package/@remotion/tailwind-v4) - Tailwind CSS v4 support.
- [@remotion/tailwind](https://www.npmjs.com/package/@remotion/tailwind) - Tailwind CSS v3 support.
- [@remotion/enable-scss](https://www.npmjs.com/package/@remotion/enable-scss) - Enable SCSS in Remotion.
- [@remotion/codemods](https://www.npmjs.com/package/@remotion/codemods) - Codemods for upgrading Remotion projects.
- [@remotion/player-a11y](https://www.npmjs.com/package/@remotion/player-a11y) - Accessible wrapper around the Player with WCAG controls.
- [@remotion/drag-and-drop](https://www.npmjs.com/package/@remotion/drag-and-drop) - Build and parse drag-and-drop payloads.
- [@remotion/canvas](https://www.npmjs.com/package/@remotion/canvas) - Experimental primitives for building authoring interfaces.
- [@remotion/sdk](https://www.npmjs.com/package/@remotion/sdk) - Experimental primitives for building Remotion authoring tools.

## Templates

Official starters from the [template catalog](https://www.remotion.dev/templates).

- [Hello World](https://www.remotion.dev/templates/hello-world) - A playground with a simple animation, recommended for first projects.
- [Blank](https://www.remotion.dev/templates/blank) - An empty canvas with no extras.
- [Next.js](https://www.remotion.dev/templates/next) - A SaaS starter for video generation apps.
- [React Router 7](https://www.remotion.dev/templates/react-router) - A SaaS starter built on React Router 7.
- [Vercel Sandbox](https://www.remotion.dev/templates/vercel) - Render videos on demand using Vercel Sandbox.
- [Render Server](https://www.remotion.dev/templates/render-server) - An Express server for rendering videos.
- [Electron](https://www.remotion.dev/templates/electron) - Render videos from a desktop app.
- [Recorder](https://www.remotion.dev/templates/recorder) - A video production tool built entirely in JavaScript.
- [3D](https://www.remotion.dev/templates/three) - A React Three Fiber starter.
- [Skia](https://www.remotion.dev/templates/skia) - A React Native Skia starter.
- [Stills](https://www.remotion.dev/templates/still) - Dynamic PNG and JPEG images with a built-in server.
- [Audiogram](https://www.remotion.dev/templates/audiogram) - Text and waveform visuals for podcasts.
- [Music Visualization](https://www.remotion.dev/templates/music-visualization) - Audio-reactive visuals for music.
- [Overlay](https://www.remotion.dev/templates/overlay) - Compositions designed for video editing software.
- [Code Hike](https://www.remotion.dev/templates/code-hike) - Animated code walkthroughs.
- [TikTok](https://www.remotion.dev/templates/tiktok) - Animated word-by-word captions.
- [Stargazer](https://www.remotion.dev/templates/stargazer) - Celebrate repository stars with a video.
- [Prompt to Video](https://www.remotion.dev/templates/prompt-to-video) - Turn a prompt into a narrated image story.
- [Prompt to Motion Graphics](https://www.remotion.dev/templates/prompt-to-motion-graphics) - A SaaS starter for AI-powered animation generation.
- [Element Library](https://www.remotion.dev/templates/element-library) - Build and publish your own Remotion element library.
- [Editor Starter](https://www.remotion.dev/templates/editor-starter) - A boilerplate for starting your own video editor (paid).

Community templates:

- [Remotion TTS Example](https://github.com/FelippeChemello/Remotion-TTS-Example) - Text-to-speech with Azure.
- [Remotion gTTS Template](https://github.com/thecmdrunner/remotion-gtts-template) - Text-to-speech with Google.
- [Docker Build and Render](https://github.com/scotthavird/remotion-docker-template) - A containerized build and render pipeline.
- [Monorepo Template](https://github.com/Takamasa045/remotion-studio-monorepo) - Multiple shared components in a monorepo.
- [DevContainer Template](https://github.com/openscript/remotion-devcontainer-template) - A reproducible development container.
- [Library Starter](https://github.com/remotion-dev/library-starter) - Best practices for publishing a Remotion library.
- [Remotion on Railway](https://railway.com/deploy/remotion-on-rails) - A one-click deployment template.
- [Quote Shorts](https://github.com/developk/remotion-quote-shorts) - Vertical quote videos rendered from a single content file.

## Components

- [Remocn](https://remocn.dev) - Copy-paste animated components, transitions, backgrounds, and scenes.
- [Remotion UI](https://github.com/riaz37/remotion-ui) - Production-ready motion components and compositions whose source you own.
- [Remotion Bits](https://remotion-bits.dev) - Ready-made animated components, charts, transitions, and text reveals.
- [Onda](https://onda.video) - Open-source motion graphics components for Remotion.
- [Snapcn](https://snapcn.dev) - A shadcn-style registry of Remotion components you install with the CLI.
- [React Video Editor Templates](https://www.reactvideoeditor.com/remotion-templates) - Open-source video editor and timeline components.
- [TikTok Text Box](https://github.com/KyleTryon/TikTokTextBox) - A TikTok-style multiline text box.
- [Remotion Animated](https://www.remotion-animated.dev) - Declarative animation helpers for Remotion.
- [remotion-transition-series](https://github.com/marcusstenbeck/remotion-transition-series) - Sequence transitions built on Remotion Transitions.
- [remotion-time](https://github.com/fwextensions/remotion-time) - Time-based helpers for Remotion.
- [remotion-animate-text](https://github.com/pskd73/remotion-animate-text) - Text animation helpers.
- [remotion-subtitles](https://github.com/ahgsql/remotion-subtitles) - Subtitle components for Remotion.
- [Remotion Glitch Effect](https://github.com/storybynumbers/remotion-glitch-effect) - A glitch effect component.
- [Clippkit](https://www.clippkit.com) - Free Remotion components.
- [SwiftClip](https://github.com/zz41354899/SwiftClip) - 30 production-ready Remotion templates.
- [RenderComp Free](https://github.com/RenderComp/free-remotion-templates) - 50 MIT-licensed Remotion templates.
- [cliphou.se](https://cliphou.se/remotion-templates) - Free MIT-0 templates with editable text and colors.
- [Lexington Motion](https://lexingtonthemes.com/remotion) - Looping promo templates for social media.

## Examples

- [HTML in Canvas](https://github.com/remotion-dev/html-in-canvas) - The official example for capturing HTML-in-canvas content as a video.
- [Typewriter Effect](https://github.com/remotion-dev/typewriter) - A classic typewriter animation.
- [D3.js Charts](https://github.com/remotion-dev/d3-example) - Animate D3 visualizations frame by frame.
- [Tone.js Music](https://github.com/remotion-dev/tone-js-example) - Generate music with Tone.js.
- [Animated GLB Models](https://github.com/remotion-dev/glb-example) - Load and animate glTF models.
- [3D Text](https://github.com/remotion-dev/3d-text) - Extruded 3D text.
- [Text Morphing](https://github.com/remotion-dev/morph-text) - Morph between words and shapes.
- [Text Warping](https://github.com/remotion-dev/text-warping) - Warp text along a path.
- [OpenGL Transitions](https://github.com/remotion-dev/remotion-gl-transitions) - Shader-based scene transitions.
- [Light Leak Transition](https://github.com/remotion-dev/light-leak-example) - A light leak transition effect.
- [CSS Animations](https://github.com/remotion-dev/css-animation-play-state) - Drive CSS animations from the frame.
- [Jump Cuts](https://github.com/remotion-dev/video-with-jump-cuts) - Make jump cuts without remounting video.
- [Measure a DOM Node](https://github.com/remotion-dev/measure-item) - Measure rendered elements.
- [Anime.js](https://github.com/remotion-dev/anime-example) - Use Anime.js timelines.
- [Mapbox](https://github.com/remotion-dev/mapbox-example) - Animated Mapbox maps.
- [MapLibre](https://github.com/remotion-dev/maplibre-example) - Animated MapLibre maps.
- [Three.js Particles](https://github.com/JonnyBurger/three-particles) - A particle system in Three.js.
- [Apple Spring Animation](https://github.com/JonnyBurger/spring-loaded) - Recreate Apple's spring-loaded animation.
- [Wavy TikTok Effect](https://github.com/JonnyBurger/wavy-meme) - A wavy TikTok-style effect.
- [Matter.js Pool Game](https://github.com/hylarucoder/remotion-physics) - A physics simulation with Matter.js.
- [Bar Race Chart](https://github.com/hylarucoder/remotion-bar-race-chart) - An animated bar race chart.
- [Globe.gl](https://github.com/alexfernandez803/remotion-globegl) - A 3D globe with arcs and points.
- [Shader A-Roll](https://github.com/onion2k/a-roll) - Shader-driven video effects.
- [12+ Examples](https://remotion-example.vercel.app) - A gallery of community examples.

## Full Projects

- [GitHub Unwrapped](https://github.com/remotion-dev/github-unwrapped) - A personalized year-in-review video for GitHub users.
- [GitHub Unwrapped 2022](https://github.com/remotion-dev/github-unwrapped-2022) - The 2022 edition of GitHub Unwrapped.
- [GitHub Unwrapped 2021](https://github.com/remotion-dev/github-unwrapped-2021) - The 2021 edition of GitHub Unwrapped.
- [Remotion Trailer](https://github.com/remotion-dev/trailer) - The official promotional video for Remotion.
- [Remotion Wrapped](https://github.com/JonnyBurger/remotion-wrapped) - A Spotify Wrapped-style animation built by Remotion's founder.
- [Fireship-Style Videos](https://github.com/wcandillon/remotion-fireship) - Recreate Fireship-style videos with React and Remotion.
- [Recorder](https://github.com/remotion-dev/recorder) - A video production tool built entirely in JavaScript.
- [Podcast Maker](https://github.com/FelippeChemello/podcast-maker) - Turn newsletters into narrated videos with motion graphics and text-to-speech.
- [Stargazer](https://github.com/pomber/stargazer) - Celebrate a repository's star milestone with a video of its stargazers.
- [Mockoops](https://github.com/Just-Moh-it/Mockoops) - Create device mockup animations from screen recordings.
- [Product Hunt Today](https://github.com/Kamigami55/product-hunt-today) - A daily Product Hunt recap video.
- [Remotion Weather](https://github.com/florentpergoud/remotion-weather) - A weather forecast video creator.
- [Rewind Table](https://github.com/gregonarash/rewind-table) - Programmatic videos using Airtable as a data source.
- [Motionly](https://github.com/karelnagel/motionly) - An open-source video editor with dynamic data rendering.
- [DataVids](https://github.com/apsquared/datavids_public) - Data-driven video generation.
- [Social Video Generator](https://github.com/lyonjs/social-video-generator) - Conference speaker announcement cards.
- [Auto Reel Edit](https://github.com/sieve-community/auto-reel-edit) - Captioning and background removal for vertical reels.
- [OpenMontage](https://github.com/calesthio/OpenMontage) - An open-source, agentic video production system.
- [OpenChatCut](https://github.com/0xsline/OpenChatCut) - An open-source, local-first conversational AI video editor with a multi-track timeline.
- [Kimu Video Editor](https://github.com/trykimu/videoeditor) - An open-source CapCut and Canva alternative built on Remotion.
- [clip-js](https://github.com/mohyware/clip-js) - An online video editor built with Next.js, Remotion, and WebAssembly FFmpeg.
- [React Video Editor](https://github.com/openvideodev/react-video-editor) - An open-source CapCut and Canva clone.
- [Short Video Maker](https://github.com/gyoridavid/short-video-maker) - Create shorts for TikTok, Reels, and YouTube with MCP and a REST API.
- [Cinetic](https://github.com/Leonxlnx/cinetic) - Cinematic launch films and motion design directed by a coding agent.
- [Vanta](https://github.com/itsjwill/vanta) - An open-source AI video engine with voice cloning, avatars, captions, and 100+ transitions.

## Tools

- [Remotion CLI](https://www.remotion.dev/docs/cli) - The command-line interface for previewing, rendering, and managing projects.
- [VS Code Extension](https://marketplace.visualstudio.com/items?itemName=KarelNagel.remotion-vscode) - Preview and inspect compositions inside VS Code.
- [Agent Skills](https://www.remotion.dev/docs/ai/skills) - Official skills that teach coding agents how to use Remotion.
- [Claude Code Plugin](https://github.com/remotion-dev/claude-code-plugin) - The official Remotion skills packaged as a Claude Code plugin.
- [Video Shotcraft](https://github.com/Vincentwei1021/video-shotcraft) - An agent skill for cinematic, editable product promos.
- [GitHub Actions Matrix Renderer](https://github.com/yuvraj108c/Remotion-Matrix-Renderer) - Render videos faster by splitting work across GitHub Actions jobs.
- [Rustymotion](https://github.com/clearlysid/rustymotion) - An experimental Rust-based renderer for Remotion videos.
- [Remotion QA](https://github.com/GroMarketing/remotion-qa) - Check renders for safe zones, dead air, and unreadable captions.

## Tutorials

- [Fireship: Remotion Tutorial](https://www.youtube.com/watch?v=deg8bOoziaE) - A fast introduction to making videos with React.
- [Spotify Wrapped 2020](https://www.youtube.com/watch?v=I-y_5H9-3gk) - Recreate a Spotify Wrapped-style recap.
- [Spotify Wrapped 2025](https://www.youtube.com/watch?v=WAjO-M_Q9C0) - An updated Spotify Wrapped build.
- [Programmatic Stories](https://www.youtube.com/watch?v=70UdF6DWY3M) - Build Instagram-style story videos.
- [Basketball Tracker](https://www.youtube.com/watch?v=A8miHLSf_BI) - Animate sports tracking graphics.
- [Formula 1 Graphics](https://www.youtube.com/watch?v=sA-X0Bw_7Gg) - Build Formula 1-style broadcast graphics.
- [Football Graphics](https://www.youtube.com/watch?v=BI8IWwaDt8s) - Build football broadcast graphics.
- [Remotion Skia Tutorial](https://www.youtube.com/watch?v=-7MOoWN2_nk) - Use React Native Skia for high-performance graphics.
- [DVD Screensaver](https://www.youtube.com/watch?v=n69siyttEwM) - Animate a bouncing DVD logo.
- [Timing Animations](https://www.youtube.com/watch?v=WigIALCnEvw) - Understand frames, timing, and interpolation.
- [Podcast Video with AI](https://www.youtube.com/watch?v=EGxBBL91nRM) - Create a podcast video with Remotion and AI.
- [Alfonso Graziano's Tutorial](https://www.youtube.com/watch?v=r4v1J7ozxIg) - A project-based Remotion walkthrough.
- [GSAP Timelines in Remotion](https://www.remotion.dev/docs/gsap) - Drive animations with GSAP timelines.

## Articles

- [Create Videos with Code](https://prismic.io/blog/create-videos-with-code-remotion-tutorial) - A Prismic tutorial on building a video with Remotion.
- [Remotion on Rails](https://medium.com/@viveknathani/remotion-on-rails-0852acc9595e) - Deploy Remotion on Railway.

## Case Studies

Official write-ups of companies shipping video with Remotion.

- [Typeframes](https://www.remotion.dev/success-stories/typeframes) - A SaaS that generates product promo videos in minutes.
- [MakeStories](https://www.remotion.dev/success-stories/makestories) - A platform that renders web stories at scale.
- [shortvid.io](https://www.remotion.dev/success-stories/shortvid) - Automated conference promo material, with the source code open-sourced.

## Community

- [Discord](https://www.remotion.dev/discord) - The official community chat for help, showcases, and discussion.
- [X](https://x.com/remotion) - Product updates and community videos.
- [YouTube](https://www.youtube.com/@remotion_dev) - Official tutorials, talks, and demos.
- [Instagram](https://www.instagram.com/remotion) - Short videos made with Remotion.
- [LinkedIn](https://www.linkedin.com/company/remotion) - Company news and hiring updates.
- [GitHub Organization](https://github.com/remotion-dev) - All official repositories.
- [GitHub Topic](https://github.com/topics/remotion) - Community projects tagged with Remotion.
- [Reddit](https://www.reddit.com/r/remotion/) - A community forum for questions and showcases.
- [Support](https://www.remotion.dev/docs/support) - Official support options and response times.

## Related Lists

- [Awesome React](https://github.com/enaqx/awesome-react) - A curated list of React resources.
- [Awesome Creative Coding](https://github.com/terkelg/awesome-creative-coding) - Generative art and creative coding resources.
- [Awesome FFmpeg](https://github.com/transitive-bullshit/awesome-ffmpeg) - FFmpeg tools, scripts, and resources.
- [Awesome Video](https://github.com/krzemienski/awesome-video) - Video engineering, streaming, and tooling.

## Contributing

Contributions are welcome. Read the [contribution guidelines](contributing.md) before opening an issue or pull request, and run `npx awesome-lint` locally to check your changes. By participating, you agree to follow the [Code of Conduct](code-of-conduct.md).
