---
layout: page  
published: true  
title: How to Contribute Ambient Sounds  
---

# How to Contribute Ambient Sounds

This document covers the specifications for contributing ambient sounds to Screwloose Games. If you need to contribute ambient sounds, please follow these guidelines carefully to ensure smooth integration into our projects.

## See also

- [How to contribute music](./how_to_contribute_music.md)
- [How to contribute sound effects](./how_to_contribute_sound_effects.md)
- [How to contribute voice-over](./how_to_contribute_voice_over.md)

## Overview

This document outlines the requirements for submitting ambient sounds to our games. Ambient sounds contribute to the atmosphere and immersion of the game environment. To maintain consistency across our projects, please adhere to the following specifications.

## Ambient Sound Specifications

### File Format

`.ogg` (Ogg Vorbis)

### Reasoning

OGG is a compressed format that provides a great balance between quality and file size, making it ideal for ambient sounds that need to loop continuously in the background without consuming too much memory.

### Sound Quality

- **Sample Rate**: 44.1 kHz (standard for game audio)
- **Bit Depth**: 16-bit (sufficient for high-quality sound while keeping file sizes manageable)

### Looping

- Ambient sounds must loop seamlessly. Ensure there are no audible pops, clicks, or abrupt transitions at the loop points.
- Avoid fade-ins or fade-outs unless explicitly requested for specific scenarios.

### Naming Conventions

- Files should follow this naming format: `amb_description.ogg`.
- Be descriptive (e.g., `amb_forest_wind.ogg`, `amb_city_traffic.ogg`).

### Normalization

- Ensure all ambient sounds are normalized to a **-1 dB ceiling** to prevent clipping.
- Keep volume levels consistent across different ambient sounds to ensure smooth transitions.

## Metadata Requirements

Include the following metadata where applicable:

- Sound name
- Designer’s name
- Intended use or description (e.g., "used for forest ambience," "looping background sound for cityscape")

## Submission Guidelines

1. **Review and Submission Process**
   - Submit ambient sounds via the project’s shared drive or designated repository.
   - Organize files into an `ambient` audio folder within the project `audio` directory. `/project/assets/audio/ambient`. They can be re-organized later.

2. **Versioning**
   - Use clear version numbers to track updates (e.g., `amb_rain_loop_v2.ogg`).

3. **Delivery Format**
   - Submit files through the shared file storage platform or GitHub repository in the `.ogg` format.
