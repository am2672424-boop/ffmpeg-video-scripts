# ffmpeg-video-scripts
# Automation & FFmpeg Video Utility Scripts

CLI snippets for automated batch processing, resizing, and aspect-ratio conversion.

## 9:16 Vertical Video Crop
```bash
ffmpeg -i input.mp4 -vf "crop=ih*(9/16):ih" -c:a copy output_shorts.mp4
