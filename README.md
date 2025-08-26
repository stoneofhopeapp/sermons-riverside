# Sermon Data (Weekly Upload)

This repository holds weekly sermon files. Each file is a JSON named by date.
You **do not** edit `manifest.json` — it is updated automatically.

---

## 📄 File naming
- Put one file per week at the repo **root**, e.g.:
  - `20250907.json` (format: `YYYYMMDD.json`)
- Example file is included: `20250821.json`. Duplicate it and edit.

> Tip: Keep the name exactly 8 digits (year + month + day). This keeps the list in date order.

---

## ✍️ What to put in the JSON
Each `YYYYMMDD.json` may contain **one sermon object** or an **array of multiple sermons**.  
Both are valid. Example with multiple sermons:

[
  {
      "title": "A Contrite Confession",
      "preacher": "Cole Smith",
      "date": "Aug 17/25",
      "intro": "Psalm 51 is a prayer of repentance...",
      "audio_url": "https://example.com/audio.mp3",
      "pdf_url": "https://example.com/notes.pdf",
      "video_url": "https://www.youtube.com/embed/IFWRQtpFKug",
      "youtube_id": "IFWRQtpFKug",
      "book_ord": 19,
      "chapter_range": "Psalm 51",
      "chapters": [51]
    }
]
