# Cinderella PW Extractor Bot

A Telegram bot to extract content from Physics Wallah (PW) and Classplus without purchase.

## Features

- **Physics Wallah (PW)**: Extract videos (with ClearKey DRM support), PDF notes, and DPPs
- **Classplus (CP)**: Extract videos and PDFs from Classplus courses
- Supports Today's Class extraction
- Full batch extraction with organized ZIP output

## What's New (Updated)

### Fixed Issues
1. **Video Extraction**: Added complete video URL extraction with ClearKey DRM support
2. **Video Mapping**: Now extracts from `videoMapping` (mux, alisg-cdn, cdn) fields
3. **DRM Keys**: Extracts and saves ClearKey decryption keys alongside video URLs
4. **ThreadPool Bug**: Fixed `'Client' object has no attribute 'request'` error
5. **Dead Code**: Removed unused `image` variable assignments

### Video Output Format
```
Video Name:https://sec-prod-mediacdn.pw.live/.../master.mpd | DRM: ClearKey | Key: KID:KEY
```

## Deploy to Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Environment Variables

| Variable | Description |
|----------|-------------|
| `API_ID` | Telegram API ID |
| `API_HASH` | Telegram API Hash |
| `BOT_TOKEN` | Bot Token from @BotFather |

## License

MPL-2.0
