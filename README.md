# dnacademy
fix img 33%

1. create manifest.json
JSON
{
  "manifest_version": 3,
  "name": "DNAcademy img fix",
  "version": "1.0",
  "description": "Forces coourse images to 100% width on community.godaddy.com",
  "content_scripts": [
    {
      "matches": ["https://community.godaddy.com/*"],
      "css": ["styles.css"],
      "run_at": "document_start"
    }
  ]
}

.arte__image {
  width: 100% !important;
}

2. create styles.css
.arte__image {
  width: 100% !important;
}
