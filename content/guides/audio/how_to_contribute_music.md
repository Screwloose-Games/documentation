---
layout: page
published: true
title: How to Contribute Music
---

# How to Contribute Music

This document covers the specifications for music in the game. If you are interested in contributing music, please read this document carefully.

## Overview

This document provides detailed guidelines for music composers contributing to projects. To ensure consistency and seamless integration with our Godot 4 games, please adhere to the following specifications for music submission.

## Music Specifications

### Technical Specs

**File Format:** `.ogg` OGG (Ogg Vorbis)
**Bitrate:** 192 kbps Constant Bitrate (CBR)
**Bit Depth:** 16-bit
**Sample Rate:** 44.1 kHz

---

### **Audio Processing**

- **Normalization**: All music files must be normalized to ensure consistent playback volume across different tracks. Please apply a **-1 dB ceiling** to prevent clipping during playback.
  - **Target loudness**: -14 LUFS (for a balance between loudness and dynamics).
  - **Ensure no excessive dynamic range compression**, unless stylistically required.

- [How to Normalize LUFS](./how_to_normalize_lufs.md)

### **Looping Music**

- Create a loop point in the metadata
- End the file name with `_loop` if the file loops
- Ensure the loop is seamless and doesn’t include any audible pops or clicks.
- Avoid fade-in or fade-out on loops unless specifically requested.

- See: [How to Make Looping Audio Tracks](./how_to_make_looping_audio_tracks.md)

### **File Naming Conventions**

- Use this format to name files:
  - **[project_name]_bgm_[description]_[version].ogg**
  - Example: `puzzlegame_bgm_main_theme_v1.ogg`
- Be descriptive with the track’s purpose (e.g., "main_theme," "boss_fight," "ambient_loop").
- Use underscores to separate words (e.g., `main_theme.ogg`, `boss_fight.ogg`).
- Use lowercase letters
- Avoid special characters or spaces in file names.
- Use version numbers for different iterations (e.g., `main_theme_v1.ogg`, `main_theme_v2.ogg`).
- If the file loops, put `_loop` at the end of the file name (e.g., `main_theme_loop_v4.ogg`).

### **Metadata Requirements**

Include the following metadata in the OGG files:

- Track title
- Composer name
- Track length
- Any specific instructions for use (e.g., specific in-game context, scene details)

### **Submission Guidelines**

1. **Review and Submission Process**
   - All tracks must be submitted for review via the project’s designated shared drive or repository.
   - Ensure files are properly named and organized in a "Music" folder under the project name.

2. **Delivery Format**
   - Use the project’s shared file storage or GitHub repository for file delivery.
   - Ensure tracks are compressed efficiently to minimize file size without sacrificing quality (192 kbps OGG).
   - Organize files into a "Music" folder within the project’s audio directory. `/project/assets/audio/music`.

## See also

- [How to contribute sound effects](./how_to_contribute_sound_effects.md)
- [How to contribute voice-over](./how_to_contribute_voice_over.md)
- [How to contribute ambient sounds](./how_to_contribute_ambient_sounds.md)
- [Explanation of WAV and ogg](./explanation_of_wav_and_ogg.md)
