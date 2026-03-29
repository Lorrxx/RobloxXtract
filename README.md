<div align="center">

<img src="https://cdn.simpleicons.org/roblox/ffffff" width="48" height="48" alt="Roblox" />

# RobloxXtract

A single-file browser tool for fetching, previewing, and downloading Roblox assets by ID.

<br />

[![License](https://img.shields.io/github/license/Lorrxx/RobloxXtract?style=flat-square&color=7c83f5&labelColor=16162a)](LICENSE)
[![HTML](https://img.shields.io/badge/HTML-single%20file-7c83f5?style=flat-square&labelColor=16162a)](RobloxXtract.html)
[![No dependencies](https://img.shields.io/badge/dependencies-none-7c83f5?style=flat-square&labelColor=16162a)]()

</div>

---

## Overview

RobloxXtract is a standalone HTML file — no install, no server, no build step. Open it in any browser and paste a Roblox asset ID to fetch metadata, preview the asset, and download it with the correct file format.

---

## Features

<table>
<tr>
<td width="40" align="center"><img src="https://api.iconify.design/lucide/scan-search.svg?color=ffffff" width="18" /></td>
<td><strong>Automatic type detection</strong> — queries the Roblox Economy API to identify the exact asset type</td>
</tr>
<tr>
<td align="center"><img src="https://api.iconify.design/lucide/image.svg?color=ffffff" width="18" /></td>
<td><strong>Image preview</strong> — renders thumbnail for images, decals, shirts, pants, badges, and more</td>
</tr>
<tr>
<td align="center"><img src="https://api.iconify.design/lucide/music.svg?color=ffffff" width="18" /></td>
<td><strong>Audio playback</strong> — inline player for audio assets with correct extension detection (.mp3, .ogg, .wav, .flac)</td>
</tr>
<tr>
<td align="center"><img src="https://api.iconify.design/lucide/download.svg?color=ffffff" width="18" /></td>
<td><strong>Direct download</strong> — downloads assets as their actual file type, not as unnamed blobs</td>
</tr>
<tr>
<td align="center"><img src="https://api.iconify.design/lucide/layers.svg?color=ffffff" width="18" /></td>
<td><strong>60+ asset types</strong> — handles images, audio, meshes, models, animations, plugins, fonts, and more</td>
</tr>
<tr>
<td align="center"><img src="https://api.iconify.design/lucide/copy.svg?color=ffffff" width="18" /></td>
<td><strong>URL copying</strong> — one-click copy for asset delivery and thumbnail URLs</td>
</tr>
</table>

---

## Supported Asset Types

| Category | Types |
|---|---|
| Image | Image, Decal, T-Shirt, Shirt, Pants, Face, Badge, Game Pass, Texture Pack |
| Audio | Audio (mp3, ogg, wav, flac) |
| Model | Hat, Model, Gear, Head, Torso, Limbs, Package, Solid Model, MeshPart, Dynamic Head |
| Accessory | Hair, Face, Neck, Shoulder, Front, Back, Waist, Ear, Eye, Eyebrow, Eyelash |
| Animation | Climb, Death, Fall, Idle, Jump, Run, Swim, Walk, Pose, Emote, Mood |
| Script | Lua Script, Plugin, Code Snippet |
| Other | Place, Font Family, Video |

---

## Usage

**1. Download** — grab `RobloxXtract.html` from this repository.

**2. Open** — open the file directly in any modern browser (Chrome, Firefox, Edge, Safari).

**3. Paste** — enter an asset ID in any of these formats:

```
rbxassetid://15858587148
https://www.roblox.com/catalog/15858587148
15858587148
```

**4. Fetch** — click **Fetch** or press `Enter`. The tool will:
- Detect the asset type via the Roblox API
- Show a preview (image or audio player)
- Provide a download button with the correct file extension

---

## Notes

- Some assets are **private or moderated** — metadata and previews will be unavailable for these.
- Asset delivery uses a CORS proxy (`corsproxy.io`) to resolve content types from the browser.
- This tool does **not** bypass Roblox's access controls — private assets cannot be downloaded.
- Thumbnail images are fetched from Roblox's public thumbnail CDN at 512×512.

---

## Privacy

RobloxXtract runs entirely in your browser. No data is sent to any third-party server other than:
- `economy.roblox.com` — asset metadata
- `assetdelivery.roblox.com` — asset content
- `www.roblox.com` — thumbnails
- `corsproxy.io` — CORS proxy for browser-side requests

---

## License

[MIT](LICENSE)
