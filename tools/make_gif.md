# Make GIFs and WebM from MP4

Quick ffmpeg recipes for producing small preview assets.

## MP4 to GIF

```bash
ffmpeg -i input.mp4 -vf "fps=12,scale=720:-1:flags=lanczos" -loop 0 output.gif
```

## MP4 to WebM (VP9)

```bash
ffmpeg -i input.mp4 -c:v libvpx-vp9 -b:v 0 -crf 35 -an output.webm
```

## Size tips

- Trim the clip first (`-ss 00:00:02 -t 5`) and crop to the region of interest.
- Lower frame rate for GIFs (10–15 fps) and cap width around 720 px for presentations.
- Use two-pass VP9 for tough cases and keep WebM + MP4 + GIF stems aligned.
