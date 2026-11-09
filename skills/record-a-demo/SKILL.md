---
name: record-a-demo
description: Record a product demo or walkthrough of an app on this Mac with ezRecord, with Claude driving the app and ezRecord filming each shot, then edit it into a finished video. Use when the person asks to record, film or make a demo, walkthrough, tutorial or launch video of an app or website.
---

# Record a product demo

ezRecord films; you drive the app with your own computer-use or browser tools. Without a way to click and type on this Mac, record with the person driving instead: `recorder_start`, tell them when it's rolling, `recorder_stop` when they say done.

1. `memory_get` first: the person's brand, usual captions and export preset.
2. `read_skill` with `{"name": "walkthrough-shots"}` and follow it exactly. It is the loop: `plan_shots` → `next_shot` → prepare the app → `recorder_start` on its window → act at a person's pace → `recorder_stop` → `shot_done`, until every shot is done.
3. Show the plan before recording: the shots, what each shows, and roughly how long the video will be.
4. Never record passwords, keys, real customer data or private windows. Use harmless sample data unless the person says otherwise.
5. When the shots are in, assemble and polish as the walkthrough skill says, then `export_project` and give the person the file path. Read its `check` and fix what it flags (silence, black frames, loudness) before handing over.
