---
name: make-shorts
description: Turn a long ezRecord recording into vertical 9:16 shorts or reels with captions and the camera on the face, or condense a long stream into a shorter video. Use when the person asks for shorts, reels, TikToks, clips, highlights, or to cut a long video or livestream down.
---

# Make shorts

1. `memory_get` for their caption look and preset.
2. Pick the project ("latest" or from `list_projects`) and read `get_transcript`.
3. For a talk, tutorial or podcast: `make_shorts` with `count` (default 3), or pass `moments` you chose from the transcript (whole sentences, 15 to 60 seconds, each one makes sense alone and starts with a hook).
4. For a long stream or call the person wants shorter but still long-form: `condense`.
5. Return each file's path with one line on what that short is about, and a suggested title.
