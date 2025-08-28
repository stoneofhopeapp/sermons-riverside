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

## Bible Book Ord Map

### 📖 English Version

| Book Name     | Ord | Book Name       | Ord | Book Name        | Ord |
|---------------|-----|-----------------|-----|------------------|-----|
| Genesis       | 1   | Isaiah          | 23  | Romans           | 45  |
| Exodus        | 2   | Jeremiah        | 24  | 1 Corinthians    | 46  |
| Leviticus     | 3   | Lamentations    | 25  | 2 Corinthians    | 47  |
| Numbers       | 4   | Ezekiel         | 26  | Galatians        | 48  |
| Deuteronomy   | 5   | Daniel          | 27  | Ephesians        | 49  |
| Joshua        | 6   | Hosea           | 28  | Philippians      | 50  |
| Judges        | 7   | Joel            | 29  | Colossians       | 51  |
| Ruth          | 8   | Amos            | 30  | 1 Thessalonians  | 52  |
| 1 Samuel      | 9   | Obadiah         | 31  | 2 Thessalonians  | 53  |
| 2 Samuel      | 10  | Jonah           | 32  | 1 Timothy        | 54  |
| 1 Kings       | 11  | Micah           | 33  | 2 Timothy        | 55  |
| 2 Kings       | 12  | Nahum           | 34  | Titus            | 56  |
| 1 Chronicles  | 13  | Habakkuk        | 35  | Philemon         | 57  |
| 2 Chronicles  | 14  | Zephaniah       | 36  | Hebrews          | 58  |
| Ezra          | 15  | Haggai          | 37  | James            | 59  |
| Nehemiah      | 16  | Zechariah       | 38  | 1 Peter          | 60  |
| Esther        | 17  | Malachi         | 39  | 2 Peter          | 61  |
| Job           | 18  | Matthew         | 40  | 1 John           | 62  |
| Psalms        | 19  | Mark            | 41  | 2 John           | 63  |
| Proverbs      | 20  | Luke            | 42  | 3 John           | 64  |
| Ecclesiastes  | 21  | John            | 43  | Jude             | 65  |
| Song of Songs | 22  | Acts            | 44  | Revelation       | 66  |

---

### 📖 中文（繁體）

| 書名       | Ord | 書名       | Ord | 書名         | Ord |
|------------|-----|------------|-----|--------------|-----|
| 創世記     | 1   | 以賽亞書   | 23  | 羅馬書       | 45  |
| 出埃及記   | 2   | 耶利米書   | 24  | 哥林多前書   | 46  |
| 利未記     | 3   | 耶利米哀歌 | 25  | 哥林多後書   | 47  |
| 民數記     | 4   | 以西結書   | 26  | 加拉太書     | 48  |
| 申命記     | 5   | 但以理書   | 27  | 以弗所書     | 49  |
| 約書亞記   | 6   | 何西阿書   | 28  | 腓立比書     | 50  |
| 士師記     | 7   | 約珥書     | 29  | 歌羅西書     | 51  |
| 路得記     | 8   | 阿摩司書   | 30  | 帖撒羅尼迦前書 | 52  |
| 撒母耳記上 | 9   | 俄巴底亞書 | 31  | 帖撒羅尼迦後書 | 53  |
| 撒母耳記下 | 10  | 約拿書     | 32  | 提摩太前書   | 54  |
| 列王紀上   | 11  | 彌迦書     | 33  | 提摩太後書   | 55  |
| 列王紀下   | 12  | 那鴻書     | 34  | 提多書       | 56  |
| 歷代志上   | 13  | 哈巴谷書   | 35  | 腓利門書     | 57  |
| 歷代志下   | 14  | 西番雅書   | 36  | 希伯來書     | 58  |
| 以斯拉記   | 15  | 哈該書     | 37  | 雅各書       | 59  |
| 尼希米記   | 16  | 撒迦利亞書 | 38  | 彼得前書     | 60  |
| 以斯帖記   | 17  | 瑪拉基書   | 39  | 彼得後書     | 61  |
| 約伯記     | 18  | 馬太福音   | 40  | 約翰一書     | 62  |
| 詩篇       | 19  | 馬可福音   | 41  | 約翰二書     | 63  |
| 箴言       | 20  | 路加福音   | 42  | 約翰三書     | 64  |
| 傳道書     | 21  | 約翰福音   | 43  | 猶大書       | 65  |
| 雅歌       | 22  | 使徒行傳   | 44  | 啟示錄       | 66  |
