# The 300-Year Bloom · 三百年的昙花

Our entry for **Tripothon S1** (theme: *build a world as a gift*).

A first-person walk up a planet one man spent three hundred years turning into a flowerpot — for the seed his sleeping lover smuggled aboard.

- **Play in the browser:** https://ricroad.github.io/the-300-year-bloom/ (add `?lang=zh` for Chinese) · page source: [ricroad/the-300-year-bloom](https://github.com/ricroad/the-300-year-bloom)
- **Walkthrough video (8 min 08 s):** see the [v1.0 release](https://github.com/ricroad/tripo-s1-archive/releases/tag/v1.0)

This repository keeps the story documents and the finished art behind the game.

## The story

Two lovers crash on a dead orange-haze planet with air for one. She sleeps. He stays awake — one year in every six, from thirty to eighty — and terraforms the whole planet so the night-blooming cereus seed she smuggled aboard can one day open outdoors.

You wake as her, three hundred years later, on that night. Walk up out of the haze along the lit path he left for you. His pods stand by the way, each one more hand-made than the last, each with a log he recorded for you. At the top: a hut with HOME taped on the door, the flower by the doorstep, and his last pod — one wake-up left.

Wake him, and it is his last night. Or let him sleep.

8–12 minutes · English (`?lang=zh` for Chinese) · WASD / mouse / E, or touch.

## What's here

```
story/                 story bible, world, the five logs and her notebook (Chinese)
art/
├─ painted_v3/         sky and valley plates, ground textures, plant and rock cut-outs
├─ characters/         Yue and Kai character sheets (*-v2.png)
├─ pods/               sleep-pod concepts (*-v2.png)
├─ keyframes/          first frames of the five logs and two endings
├─ video/              five video logs and two endings, English dialogue (*-en.mp4)
├─ tripo/refs/         single-object reference images and the four prologue panels (Tripo image-to-image)
├─ tripo/models/       Tripo 3D models (.glb) with previews
├─ poster/             cover posters, 16:9 and 9:16, with their HTML layouts
└─ board/              three 3840×2160 visual boards: the world, the people and pods, the Tripo pipeline
```

## How it was made

Everything he built by hand is a Tripo model: the hut, his five pods, the towers, the ship's hull and tail, the cereus by the door, and what fifty waking years leave behind — the sample rack, the workbench, the cart, the mask, the oxygen bottle, the bench for two, the potato bed, the bucket of empty tape cores, his cane.

Pipeline: our own painted sheets and keyframes → a clean single-object reference with Tripo image-to-image → Tripo image-to-3D (v3.1 geometry, de-lit v3.5 texture) → in the browser under one toon ramp, moon rim, stepped fog and ink line. The four prologue panels are Tripo image-to-image too.

| Tool | Used for |
|---|---|
| Tripo (API v3) | all 3D models; reference images and prologue panels (image-to-image) |
| Seedance 2.5 | five video logs and two endings, English dialogue |
| GPT Image 2.5 | character and pod sheets, painted scenery and textures, log keyframes, poster bases |
| Three.js r160 | engine — the whole game is one HTML file |
| WebAudio | wind, reeds, footsteps, breath, hums and the theme, all synthesised live |
| Claude Code | page code, generation and capture pipelines |

All generations use only our own text and our own images as input. No third-party images, 3D models, sound effects, music or templates are used. Three.js (MIT) loads from a CDN; fonts are from Google Fonts (SIL OFL).

---

## 中文简介

Tripothon S1 参赛作品《三百年的昙花》，一个打开浏览器就能玩的第一人称叙事游戏。

一对恋人落在一颗被毒雾盖住的橙色星球上，干净的空气只够一个人用。于是月进了休眠舱，凯每六年醒一年，从三十岁到八十岁，用三百年把整颗星球改造成花盆，只为她带上船的那颗昙花种子能在室外开花。你扮演三百年后醒来的月，沿着他留下的灯路走上山顶，最后决定是叫醒他，还是让他睡着。

本仓库存放故事设定文档和美术成品：场景画、角色与休眠舱设定、日志首帧、日志和结局视频、Tripo 参考图和 3D 模型、封面海报、视觉素材板。可玩页面见 https://ricroad.github.io/the-300-year-bloom/ ，走查录屏在 [v1.0 Release](https://github.com/ricroad/tripo-s1-archive/releases/tag/v1.0)。
