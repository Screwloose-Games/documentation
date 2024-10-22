---
title: How to Normalize Audio to LUFS
layout: page
published: true
---
# How to Normalize Audio to LUFS

## What is LUFS?

LUFS stands for Loudness Units Full Scale. It is a standard measurement for loudness in audio. It helps maintain consistent volume levels across different tracks.

Example visual difference in loudness levels:

![alt text](image.png)

- For original music, aim for a target loudness of -14 LUFS. You want it loud in the original recording to keep the dynamics, but not too loud that it clips or distorts. You need some headroom for mastering.
- Music will be adjusted (likely brought down to about -24 LUFS) to match the target loudness in the game engine.

### Example LUFS meters

Example tool: [Youlean Loudness Meter](https://youlean.co/youlean-loudness-meter/)

Too quiet:

![alt text](image-5.png)

A little too loud:

![alt text](2024-10-22_14-32-48.gif)

### Apply LUFS normalization

![alt text](image-6.png)

After normalization:

![alt text](2024-10-22_14-38-29.gif)
