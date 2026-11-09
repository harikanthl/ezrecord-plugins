---
name: dub-a-video
description: Dub an ezRecord video into another language in the person's own cloned voice (ElevenLabs) or an Indian-language voice (Sarvam), and export it with every language as an audio track. Use when the person asks to dub, translate the voice, make a Hindi/Spanish/Telugu/any-language version, or add multi-language audio.
---

# Dub a video

Dubbing spends the person's own ElevenLabs or Sarvam credit and sends their audio or text to that service. Be explicit about both.

1. `dub_plan` with the `language`. It returns the cost and exactly what would leave the Mac. Show both to the person and wait for a yes before anything else. Cloning their voice needs their own consent in ezRecord; never pick `my_voice` for someone else's voice.
2. `dub_translate`. Show the lines whose `fit` is `too_long` and offer shorter wording; fix with `dub_update_line`.
3. `dub_generate` after they agree. Follow progress with `dub_status`.
4. `export_dub` (multitrack on by default: one MP4 with the original plus every dub as language-tagged tracks, for YouTube multi-language audio). Give them the paths.
