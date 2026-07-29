# DNAcademy Image Full Width

Minimal Chrome extension that forces `.arte__image` blocks on community.godaddy.com to 100% width.

## Installation

1. Download or clone this repository
2. Open `chrome://extensions`
3. Enable **Developer mode**
4. Click **Load unpacked**
5. Select this folder

## Project structure

```
dnacademy-image-fullwidth/
├── manifest.json
├── styles.css
└── README.md
```

## manifest.json

```json
{
  "manifest_version": 3,
  "name": "DNAcademy Image Full Width",
  "version": "1.0.0",
  "description": "Forces .arte__image blocks to 100% width on community.godaddy.com",
  "content_scripts": [
    {
      "matches": ["https://community.godaddy.com/*"],
      "css": ["styles.css"],
      "run_at": "document_start"
    }
  ]
}
```

## styles.css

```css
.arte__image {
  width: 100% !important;
}
```

## License

MIT
