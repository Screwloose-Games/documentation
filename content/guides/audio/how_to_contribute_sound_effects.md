---
layout: page  
published: true  
title: How to Contribute Sound Effects  
---

# How to Contribute Sound Effects

This document covers the specifications for contributing sound effects to our Games. If you are interested in contributing sound effects, please review the following guidelines carefully to ensure consistent integration into our projects.

## See also

- [How to contribute music](./how_to_contribute_music.md)
- [How to contribute voice-over](./how_to_contribute_voice_over.md)
- [How to contribute ambient sounds](./how_to_contribute_ambient_sounds.md)

## Overview

This document outlines the standards for submitting sound effects to our games. To maintain consistency and performance across all our projects, contributors must adhere to the following sound effect specifications.

## Sound Effect Specifications

### File Format

`.wav` (Waveform Audio File Format)

### Reasoning

WAV files are uncompressed, providing high-quality sound and quick loading times, which are critical for short and frequent sound effects in games.

### Naming conventions

- Sound effects should follow this naming format: `sound_description.wav`.
- Be descriptive and specific (e.g., `footstep_grass.wav`, `door_open_creak.wav`).

### Sound Quality

- **Sample Rate**: 44.1 kHz (standard for game audio)
- **Bit Depth**: 16-bit (ensures high-quality sound while keeping file sizes manageable)

### Normalization

- Ensure all sound effects are normalized to a **-1 dB ceiling** to prevent clipping.
- Apply **consistent volume levels** across sound effects to avoid sudden loud spikes during gameplay.

### Length and Timing

- Ensure that sound effects are trimmed correctly, with no extra silence at the beginning or end of the file.
- If the sound is meant to loop, ensure it loops seamlessly without any clicks or pops.

## Metadata Requirements

Include the following metadata where possible:

- Sound effect name
- Sound designer’s name
- Description of use (e.g., "used for player jump," "used for enemy death")

## Submission Guidelines

1. **Review and Submission Process**
   - All sound effects must be submitted via the project’s shared drive or designated repository.
   - Organize files into the folder relevant for this asset. Eg. `/project/characters/character_name/audio/footsteps`
   - If there is no central location for the context for the asset, organize files into an `sfx` folder within the project `audio` directory. `/project/assets/audio/sfx`. They can be re-organized later.

2. **File Naming**
   - Use descriptive names for sound effects to ensure easy identification and integration.
   - Avoid generic names like `sound1.wav` or `effect2.wav`.
   - Use underscores to separate words in the file name (e.g., `bodyfall_concrete_v2.wav`).

3. **Versioning**
   - Clearly version each sound effect submission to track updates and iterations. `footstep_boot_grass_v1.wav`.

4. **Delivery Format**
   - Submit files using the project’s shared storage platform or GitHub repository.
   - Use `.wav` files for sound effects to ensure high-quality playback.

## Why Use .wav for Sound Effects?

WAV files are uncompressed and easier for the game engine to process. This format is ideal for short, frequent sound effects as it avoids the decoding overhead required by compressed formats like OGG, ensuring sound effects can play instantly without delay.
