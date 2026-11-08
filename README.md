# ffmpeg-video-scripts
# Video Automation & FFmpeg Utility Scripts

Automated scripts for formatting, cropping, and extracting audio for AI video pipelines.

### 1. Vertical Video Conversion (9:16 for Shorts / Reels)
ffmpeg -i input.mp4 -vf "crop=ih*(9/16):ih" -c:a copy output_vertical.mp4

### 2. Extract Clean Audio Track
ffmpeg -i input_video.mp4 -vn -q:a 0 -map a output_audio.mp3

### 3. Compress Video for Web / Preview
ffmpeg -i input.mp4 -vcodec libx264 -crf 28 output_compressed.mp4
