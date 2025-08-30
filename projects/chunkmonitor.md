---
title: "ChunkMonitor"
description: "A Paper plugin that helps online players spot who's causing lag by displaying most chunk generation."
logo: "cover/chunkmonitor-cover.jpg"
tags: ["minecraft", "plugin"]
dateCreated: "2025-04-30 12:00:00"
dateUpdated: "2025-04-30 12:00:00"
sitemap:
  loc: /projects/chunkmonitor
  lastmod: 2025-04-30
  changefreq: monthly
  priority: 0.8
---

<img src="chunkmonitor/ChunkMonitor.png" width="64">

# ChunkMonitor

**ChunkMonitor** is a Paper plugin that helps you spot players causing lag by monitoring chunk generation. Ever wonder why your TPS drops? This plugin shows you who’s generating the most chunks in real-time!

[Jump to Download](#download)

## Features
- Monitors chunk generation in real-time.
- Displays a boss bar showing the player generating the most chunks per minute.
- Boss bar changes color based on the rate of chunk generation:
    - **Green** for low generation.
    - **Yellow** for medium generation.
    - **Red** for high generation.
- Updates chunk generation statistics at a configurable interval.
- Supports player joining with the boss bar being displayed if necessary.

## In-game picture
- Low chunk generation
  ![low-gen.png](chunkmonitor/low-gen.png)
- Medium chunk generation
  ![mid-gen.png](chunkmonitor/mid-gen.png)
- High chunk generation
  ![high-gen.png](chunkmonitor/high-gen.png)

## Compatibility
This is a Paper plugin and will not work with Spigot servers, but Purpur is fine.

I don't know if any version other than `1.21.5` would work, because that's the only version I tested.

## Configuration

You can adjust the plugin’s behavior using the configuration file (`config.yml`), which is generated upon enabling the plugin.

### Available Configuration Options:

- **`update-interval-ticks`**:
    - The interval (in ticks) at which chunk statistics are updated.
    - Default: `20` (1 second)

- **`min-display-threshold`**:
    - The minimum chunk generation rate required to display the boss bar.
    - Default: `250.0` (chunks per minute)

- **`yellow-threshold`**:
    - The chunk generation rate at which the boss bar color changes to yellow.
    - Default: `500.0` (chunks per minute)

- **`red-threshold`**:
    - The chunk generation rate at which the boss bar color changes to red.
    - Default: `1000.0` (chunks per minute)

- **`maxAttributionDistance`**:
    - The maximum distance a player can be from a chunk to be counted as the "nearest" player generating the chunk.
    - Default: `50.0` (blocks)

## Download

Two official ways to download at
- Modrinth [ChunkMonitor](https://modrinth.com/plugin/chunkmonitor)
- GitHub Releases [ChunkMonitor](https://github.com/TechitWinner/ChunkMonitor/releases)

## Source Code

- GitHub [ChunkMonitor](https://github.com/TechitWinner/ChunkMonitor)

## Credits
Since this is my first Java plugin project.  
This plugin was created with the help of the  **Paper documentation**, **Spigot documentation** and **ChatGPT**. (I know it's stupid)

## License
This project is licensed under the **GPL-3.0 License**  
or **TL;DR**...
- **What you can do**: Use, modify, distribute, and share the software (even commercially), as long as you comply with the GPL’s terms (especially sharing the source code and keeping the license intact).
- **What you cannot do**: You cannot distribute proprietary versions of the software, impose restrictions like DRM, or mix it with software that is under an incompatible license.