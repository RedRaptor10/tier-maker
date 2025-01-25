# Tier Maker

A web app that allows users to create their own tier lists. The Tier Maker can be repurposed for any topic. Inspired by [https://tiermaker.com](https://tiermaker.com).

**[See Demo](https://redraptor10.github.io/tier-maker/)**

![](/screenshot.jpg)

## Features
- Set tier list title, description, author, date, and background image/color
- Add/edit/remove tiers
- Drag tiers up/down
- Options to save progress, import, and export tier list
- Generate tier list image for download

## Configuration
1. Add item images to `/images/items` and background images to `/images/backgrounds` folders.
   - *Note: Item image sizes should be consistent. Backgrounds should have a regular and `-thumb` version.*
2. Modify *tier-maker.css* `--initial-item-height` and `--initial-item-width` with the item images' height and width (px).
3. Modify *tier-maker.js* defaults: (most are self-explanatory)

| Setting | Description |
| --- | --- |
| `title` | The title of the tier list. |
| `description` |The description of the tier list. |
| `background` | The background of the tier list. |
| `poolItems` | A list of item images in `/images/items`. |
| `backgrounds` | A list of background images in `/images/backgrounds`. |
| `tierItemExt` | The file extension of item images. |
| `animation` | The animation speed when dragging items. |
| `defaultTierCount` | The number of tiers to display. |
| `tierColors` | The colors of tiers to display. |
| `tierLetters` | The letters of tiers to display. |
| `fallbackBackgroundColor` | The background color if a background image fails to load. |
| `darkenBackground` | Set background to be slightly darker. |
| `showHeaderOnGenerate` | Display the tier list header on the generated image. |
| `showDate` | Display the current date. |
| `storageKey` | The key used for getting/setting the tier list in localStorage. |

## Why Should I Use This?
- Fully customizable
- No watermark
- No account required

## Tech
- JavaScript / CSS / HTML
- [SortableJS](https://sortablejs.github.io/Sortable/)
- [html2canvas](https://html2canvas.hertzen.com/)

[See here for a refactored version that allows item attachments.](https://github.com/RedRaptor10/Tier-Maker-MK1)
