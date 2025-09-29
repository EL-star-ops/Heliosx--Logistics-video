# HeliosX Warehouse Video — Step-by-Step (Browser)

## What you need
- Scene images: exterior (HeliosX branding), interior depot with wall branding (Dermatica white/green, MedExpress blue + ZipHealth alongside), storage areas, 3 packaging lines, Royal Mail elevated ramp, loading bays
- Voiceover MP3 (generate from `voiceover_script.txt` or SSML file)
- Optional background music MP3

## Steps
1) Open `index.html` in Chrome.
2) Click **Images** → select your frames (PNG/JPG) in order.
3) Click **Voiceover** → select your narration MP3.
4) (Optional) Click **Music** → select a bed track (plays ~25% volume).
5) Captions are preloaded. Edit if needed or click **Download SRT** to save.
6) Set **Per-image seconds** and **FPS** (defaults: 5s, 30fps).
7) Click **Render & Export WebM** → downloads `heliosx_warehouse.webm`.
8) Convert to MP4 (optional):
   ffmpeg -i heliosx_warehouse.webm -c:v libx264 -c:a aac -b:a 192k heliosx_warehouse.mp4

Tips:
- Align total image duration ≈ voiceover length.
- Include a clear frame showing the Royal Mail elevated ramp.
- Brand walls: Dermatica (white/green), MedExpress (blue), ZipHealth (with MedExpress), HeliosX (blue/orange).
