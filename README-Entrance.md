[创作工具下载链接 Download link for the creation tool (GitHub)](https://github.com/STRAYLIGHT66/Minecraft/tree/main/Entrance-%E5%85%A5%E5%9C%BA%E5%8A%A8%E7%94%BB)

===== English Description - EN =====
# Entrance

Entering a world shouldn't look like a progress bar.

Press "play world" and the loading screen is replaced by a short film: a beat of black, your video, a white flash, *hold E to enter*, then letterbox bars — while the world quietly finishes loading behind it.

## What you get

- Your own video as the intro, replaceable any time
- Hold-to-enter prompt; double-tap Esc to skip at any point
- Cinematic letterbox showing the world name (and the seed in singleplayer)
- Survival worlds play every entry; creative worlds only the first

## Requirements

Minecraft **26.2** + **Fabric Loader**. Fabric API is not required, and there are no other dependencies.

> This is a Fabric mod — it will not load on vanilla.

## Replacing the video

[Download link for the creation tool (GitHub)](https://github.com/STRAYLIGHT66/Minecraft/tree/main/Entrance-%E5%85%A5%E5%9C%BA%E5%8A%A8%E7%94%BB)

`EntranceTool.exe`: pick your video, pick your instance folder, pick a quality, done. It needs ffmpeg (the tool links you to it). The previous scene is backed up automatically.

Power users can use `make-scene.ps1`, or drop in a pre-exported frame sequence by hand.

## Heads up

A fresh install plays nothing — there is no video yet. Add one first.

## Config

Everything — copy, phase timings, playback rules — lives in `config/entrance/entrance.json`.



# 中文介绍：入场动画 Entrance

进世界的时候，不再是一闪而过的加载条。

## 它做什么

点下「进入世界」的瞬间，加载界面被替换成一段过场：

预黑 0.5 秒 → 播放你的视频 → 白屏过曝 → 「长按 E 进入世界」→ 电影黑边 → 淡出，交还控制。

世界在动画背后悄悄加载，所以你不会看到读条。

## 播放规则

- 生存存档：每次进入都播
- 创造存档：只有第一次进入该存档时播

## 换视频

[创作工具下载链接（GitHub）](https://github.com/STRAYLIGHT66/Minecraft/tree/main/Entrance-%E5%85%A5%E5%9C%BA%E5%8A%A8%E7%94%BB)

自带图形化转换工具 `EntranceTool.exe`：选视频 → 选游戏实例 → 选画质 → 完成。

需要自备 ffmpeg（工具里有下载地址，把 ffmpeg.exe 放在工具旁边即可）。

## 需要知道的

- **需要 Fabric Loader**（这是 Fabric 模组，原版装不了）
- 但**不需要 Fabric API**，也不需要任何其他模组
- 转换工具提供 720p / 1080p / 1440p 三档；65 秒的 1080p 约 90 MB 磁盘
- 任意阶段连按两次 Esc 跳过
- **刚装好时没有视频，所以什么都不会播** —— 先按上面的方法放一个进去
- 目前只支持 26.2

## 配置

`config/entrance/entrance.json`：文案、各阶段时长、播放规则都能改，改完重进世界生效。
