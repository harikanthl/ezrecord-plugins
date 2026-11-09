---
name: edit-a-recording
description: Edit an ezRecord recording by its transcript, remove ums and pauses, add captions and a look, and export it. Use when the person asks to edit, clean up, caption, trim, tighten or export a recording or video they made with ezRecord, or "my last recording".
---

# Edit a recording

1. `memory_get`: the person's usual cleanup, captions and export preset. Match them.
2. Find the project: "latest" works for the last recording; otherwise `list_projects`.
3. `get_transcript`, and read it. Know what the video says before cutting.
4. Prompter recordings: `keep_last_takes` first (keeps the last read of each line).
5. `review_cleanup`, then `clean_up`. Skip any cut that would take a word the meaning needs. Show the person what was cut in a sentence or two, not the whole list.
6. Cut anything else they asked for with `cut_words` (by the transcript's words).
7. Captions with `set_captions` (pill or bold for social, classic or minimal for tutorials; `words: 2` for Reels style). Other looks with `set_project_style`.
8. `export_project` with their usual preset (default universal1080). Read the `check` it returns and fix problems before giving them the file path.

If ezRecord's editor is open on this project, your edits show there live and the person can undo them.
