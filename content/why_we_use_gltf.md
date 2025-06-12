---
layout: page
title: Why We Use GLTF
published: true
---

# Why We Use GLTF

## We use GLTF (GL Transmission Format) for several reasons:

* **Industry Standard**: GLTF is widely adopted in the industry as a standard format for 3D models, making it easier to share and collaborate on assets across different platforms and tools.
* **Efficiency**: GLTF is designed for efficient loading and rendering, which is crucial for real-time applications like games. It supports binary data, reducing file size and improving performance.
* **Version Control**: GLTF files are text-based JSON files, which makes them easier to version control. This is particularly important for collaborative projects where multiple contributors may be working on the same assets.
* **Human-Readable**: The text-based nature of GLTF files __allows for easier debugging and manual editing__. This is beneficial for developers who need to make quick adjustments or troubleshoot issues without relying on specialized tools.
* **Compatibility**: GLTF is compatible with a wide range of 3D software and game engines, including Godot, Unreal Engine, and others. This allows for seamless integration of assets created in different tools.
* **Material and Animation Support**: GLTF supports advanced features like PBR (Physically Based Rendering) materials, animations, and skinning, which are essential for creating high-quality 3D content. __This puts more control in the hands of artists and designers, allowing them to create visually appealing assets without needing extensive programming knowledge.__

## Why NOT FBX?

* **Proprietary Format**: FBX is a proprietary format owned by Autodesk, which can lead to compatibility issues and limitations in terms of accessibility and openness.
* **version control challenges**: FBX files are binary, making them difficult to version control effectively. This can lead to issues when multiple contributors are working on the same assets.
* **Conversion Overhead**: Converting FBX files to other formats can introduce additional overhead and potential loss of data, especially when dealing with complex animations or materials.
* **Material Limitations**: FBX has limitations in terms of material support and may not translate well across different engines or software, leading to inconsistencies in appearance.
* **Lack of Transparency**: FBX files can be opaque, making it difficult to understand the structure and content of the file without specialized tools.

## What about .GLB?

* **Duplicate files when imported**: When importing GLB files into Godot, they are converted to GLTF format, which means that the original GLB file is not used directly in the project. __This causes texture files to be duplicated__. Textures are a significant amount of the storage space in builds. Keeping build size down is important for game load times and being able to upload a web build to Itch. [See this conversation, for example](https://godotforums.org/d/29060-workflow-for-importing-glb-and-editing-materials)
* **Single File**: GLB is the binary version of GLTF, which combines the JSON data and binary data into a single file. It is useful for reducing the number of files needed for a 3D asset, making it easier to manage and distribute.
* **Redability**: GLB files __are not human-readable like GLTF files__, which can make debugging and manual editing more challenging.
* **Performance**: GLB files are optimized for performance, as they can _individually_ be loaded more quickly than multiple separate files. This is particularly beneficial for real-time applications like games.
* **Version Control**: While GLB files are binary, they can still be version controlled effectively if the project uses a system that supports binary files. __However, it is generally easier to work with GLTF for version control due to its text-based nature.__


## Resources

* [GLTF Overview](https://www.khronos.org/gltf/)
* 

* [glTF Support in Unreal Engine](https://dev.epicgames.com/documentation/en-us/unreal-engine/gltf-file-format-support-in-unreal-engine)

---

Written by [Jonathan Lewis](https://www.linkedin.com/in/jonathan-david-lewis/)

Please reach out if you have any questions or suggestions for improvements.