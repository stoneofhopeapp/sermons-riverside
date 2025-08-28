# Riverside Sermons Data

This repository stores weekly sermon metadata for **Riverside Calvary Chapel**.

---

## Quick Steps

1. After the sermon(s) are available each week, create a new JSON file.
2. **Filename format:** `yyyymmdd.json` &nbsp;*(e.g., `20250827.json`)*
3. Start from **TEMPLATE.json** (below) and fill in the fields.
4. Commit the file to the repository (main branch).
5. ✅ That’s it — `manifest.json` will update automatically.

---

## JSON Template

Copy this structure (also available as `TEMPLATE.json`) and fill in every field:

```json
{
  "title": "",
  "preacher": "",
  "date": "",
  "intro": "",
  "audio_url": "",
  "pdf_url": "",
  "video_url": "",
  "youtube_id": "",
  "book_ord": null,
  "chapter_range": "",
  "chapters": []
}
```

---

## Multiple Sermons in One Day

If there are multiple sermons on the same day, put them into a list:

```json
[
  {
    "title": "Sermon 1",
    "preacher": "",
    "date": "",
    "intro": "",
    "audio_url": "",
    "pdf_url": "",
    "video_url": "",
    "youtube_id": "",
    "book_ord": 19,
    "chapter_range": "Psalm 37",
    "chapters": [37]
  },
  {
    "title": "Sermon 2",
    "preacher": "",
    "date": "",
    "intro": "",
    "audio_url": "",
    "pdf_url": "",
    "video_url": "",
    "youtube_id": "",
    "book_ord": 43,
    "chapter_range": "John 3",
    "chapters": [3]
  }
]
```

---

## Guidelines

- Make sure the JSON is **valid** (commas, braces, quotes).
- Provide correct values for all properties.
- Commit the new file directly to the repository.

---

## ⚠️ Important

- `manifest.json` is **auto-generated** by GitHub Actions.
- **Do not edit** or delete `manifest.json` manually.
- Only add or update the dated `yyyymmdd.json` files.
