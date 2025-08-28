# Riverside Sermons Data

This repository stores weekly sermon metadata for **Riverside Calvary Chapel**.  
Each sermon is represented as a JSON file named by its date (e.g. `20250826.json`).  
A `manifest.json` file is automatically maintained by GitHub Actions to list all sermons and track the latest version.

---

## 📂 File structure
- `YYYYMMDD.json` — individual sermon data (title, preacher, bible reference, media links).  
- `manifest.json` — auto-generated file containing:
  - `latestVersion`: the most recent date string.  
  - `files`: list of all available sermon JSONs.  

Example:

`20250826.json`
[
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
]
