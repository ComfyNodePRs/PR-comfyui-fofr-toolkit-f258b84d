# 🪴 comfyui-fofr-toolkit

Simple building block nodes for ComfyUI

## Nodes

### Incrementer

A simple counter with a max value.

Inputs:
- `current_index` (required): An integer representing the current index. Default is 0.
- `max` (optional): The maximum value before the counter resets. Default is 10.

### Width and height from aspect ratio

Calculates width and height based on a given aspect ratio and ideal target size.

Inputs:
- `aspect_ratio` (required): Choose from predefined aspect ratios (eg "1:1", "16:9", "21:9").
- `target_size` (required): The target size
- `multiple_of` (optional): Ensure the output dimensions are multiples of this value (default 8, range 1-1024).

### Width and height for scaling image to ideal size

Calculates width and height for scaling an input image to a target size while maintaining its aspect ratio.

Inputs:
- `image` (required): The input image to be scaled.
- `target_size` (required): The target size for scaling. Default is 1024, range 64-8192.
- `multiple_of` (optional): Ensure the output dimensions are multiples of this value (default 8, range 1-1024).
