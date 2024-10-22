---
layout: page
published: true
title: How to Contribute Music
---

# How to Contribute Music

This document covers the specifications for music in the game. If you are interested in contributing music, please read this document carefully.

## See also

- How to contribute sound effects
- How to contribute voice-overs
- How to contribute ambient sounds

## Overview

This document provides detailed guidelines for music composers contributing to projects. To ensure consistency and seamless integration with our Godot 4 games, please adhere to the following specifications for music submission.

## Music Specifications

### File Format

`.ogg` OGG (Ogg Vorbis)

### Bitrate

192 kbps Constant Bitrate (CBR)

### Reasoning

OGG provides an excellent balance between quality and file size, and 192 kbps ensures high-fidelity audio.

### Looping

- Music tracks should be designed to loop seamlessly.

### Naming conventions

- Music files should be named descriptively and follow the format `track_name.ogg`.

### Screwloose Games: Music Contribution Specifications



---


### **Audio Processing**

- **Normalization**: All music files must be normalized to ensure consistent playback volume across different tracks. Please apply a **-1 dB ceiling** to prevent clipping during playback.
  - **Target loudness**: -14 LUFS (for a balance between loudness and dynamics).
  - **Ensure no excessive dynamic range compression**, unless stylistically required.

### **Looping Music**

- For looping tracks, ensure the loop is seamless and doesn’t include any audible pops or clicks.
- Avoid fade-in or fade-out on loops unless specifically requested.
- If possible, provide two versions:
  1. **Looping Version**: For in-game looping (ensure seamless playback).
  2. **Full Version**: For promotional purposes or non-looped segments.

### **Sample Rate and Bit Depth**

- **Sample Rate**: 44.1 kHz (standard for game music)
- **Bit Depth**: 16-bit (sufficient for game audio quality while keeping file sizes manageable)

### **File Naming Conventions**

- Use this format to name files:
  - **[project_name]_bgm_[description]_[version].ogg**
  - Example: `puzzlegame_bgm_main_theme_v1.ogg`
- Be descriptive with the track’s purpose (e.g., "main_theme," "boss_fight," "ambient_loop").

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
   
2. **Versioning**
   - Clearly version each submission to track updates and iterations.

3. **Delivery Format**
   - Use the project’s shared file storage or GitHub repository for file delivery.
   - Ensure tracks are compressed efficiently to minimize file size without sacrificing quality (192 kbps OGG).

---

This document outlines the standards for contributing music to Screwloose Games. Adherence to these specifications will ensure that your music integrates smoothly into our projects.

## Deciding file types

### Performance and Memory Usage

Why use .ogg for music and ambient sounds and .wav for sound effects?

- **.ogg**: OGG files are compressed, which reduces file size and memory usage. They are ideal for longer music tracks and ambient sounds that play continuously in the background. These tracks are often streamed (rather than loaded into memory all at once)
- **.wav**: WAV files, being uncompressed, are easier for the game engine to load and play quickly. This is why they're often used for short, frequent sound effects. The game can play them without having to decode compressed data, which reduces processing overhead.

## Additional Resources
