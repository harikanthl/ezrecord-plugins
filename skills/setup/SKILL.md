---
name: setup
description: Connect Claude to ezRecord on this Mac and check it works. Use when ezRecord's tools fail to connect, return 401 or "needs its passcode", or the person asks to set up, connect or test ezRecord.
---

# Connect ezRecord

ezRecord's tools come from the ezRecord app on this Mac (127.0.0.1:7879). They only answer while the app is running, and only with its passcode.

1. Call `app_status`. If it answers, report the version and any missing permission (screen, camera, microphone) with where to turn it on (System Settings › Privacy & Security). You're done.
2. If the connection is refused: ezRecord isn't running, or its agent server is off. Ask the person to open ezRecord (it is at https://harikanth.site/ezrecord, with a 14 day free trial, if they do not have it) and check ezRecord › Settings › Agents › "Let agents use ezRecord" is on.
3. If it says the passcode is missing or wrong: the quickest fix is ezRecord › Settings › Agents › Connect Claude Code (ezRecord 1.1.1 or later). Otherwise ask them to copy it from ezRecord › Settings › Agents (the copy button beside Passcode; on 1.1.0, the part of the MCP address after /mcp/), run `/plugin configure ezrecord@ezrecord` and paste it there. Then `/mcp` reconnects the server.
4. Call `app_status` again to confirm.

Never ask the person to paste the passcode into the chat.
