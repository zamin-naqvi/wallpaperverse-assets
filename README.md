# WallpaperVerse Assets

This repository contains wallpapers for the WallpaperVerse app.

## Structure

```
wallpaperverse-assets/
├── wallpapers/          # Put all wallpaper images here
│   ├── example_1.jpg
│   ├── example_2.jpg
│   └── ...
├── wallpapers.json      # Wallpaper metadata
└── README.md           # This file
```

## Adding New Wallpapers

1. Upload your wallpaper image to the `wallpapers/` folder
2. Edit `wallpapers.json` and add a new entry:

```json
{
  "id": 102,
  "name": "Your Wallpaper Name",
  "fileName": "your_image.jpg",
  "category": "ANIME",
  "tags": ["tag1", "tag2", "tag3"],
  "isPremium": false,
  "isOnline": true
}
```

### Valid Categories
- `ANIME`
- `CARS`
- `NATURE`
- `SUPERHEROES`
- `CARTOON`

### ID Ranges
- **1-58**: Reserved for app's bundled wallpapers
- **59-99**: Reserved for future bundled wallpapers
- **100+**: Use for online wallpapers

### File Naming
- Use lowercase with underscores: `my_wallpaper.jpg`
- No spaces or special characters
- Supported formats: `.jpg`, `.jpeg`, `.png`

## Testing

After uploading:
1. Wait 1-2 minutes for GitHub CDN to update
2. Open the app and pull down to refresh
3. Your new wallpapers should appear

## Image URLs

Images are served via GitHub's raw content CDN:
```
https://raw.githubusercontent.com/aeroloomstudio/wallpaperverse-assets/main/wallpapers/your_image.jpg
```

You can test URLs in your browser before adding to the app.
