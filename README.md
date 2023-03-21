# NoWater
 
## Remove Watermark from Image

This is a Python script to remove a watermark from an image using OpenCV.

### Usage

To use this script, run the following command:

```
python remove_watermark.py input_file output_file [--color COLOR_COLOR COLOR] [--method {telea,ns}] [--threshold THRESHOLD] [--brush BRUSH]

```

- `input_file`: The path to the input image file.
- `output_file`: The path to save the output image file.
- `-color COLOR_COLOR COLOR`: The watermark color in BGR format (default: 150 150 150).
- `-method {telea,ns}`: The inpainting method to use (default: telea).
- `-threshold THRESHOLD`: The color threshold for watermark detection (default: 10).
- `-brush BRUSH`: The size of the inpainting brush (default: 3).

### Example

```
python remove_watermark.py input.jpg output.jpg --color 255 255 255 --method ns --threshold 5 --brush 5

```

This will remove a white watermark from the `input.jpg` file using the `ns` inpainting method with a color threshold of 5 and a brush size of 5. The output will be saved to `output.jpg`.

### Dependencies

This script requires the following Python packages:

- `opencv-python`
- `numpy`
- `argparse`
