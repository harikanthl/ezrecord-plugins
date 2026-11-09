# ezRecord for Claude Code

Let Claude record, edit, caption, dub and post videos with [ezRecord](https://harikanth.site/ezrecord), the screen and camera recorder for Mac. Claude can film a product demo while it clicks through your app, edit a recording by its transcript, cut shorts, dub a video into another language and plan a shoot.

Everything runs in the ezRecord app on your Mac. The plugin connects Claude to it at 127.0.0.1, with a passcode only you have.

## Install

1. Install ezRecord from https://harikanth.site/ezrecord (14 days free, then a plan) and open it.
2. In Claude Code:

```
/plugin install ezrecord --marketplace harikanthl/ezrecord-plugins
```

or from your shell:

```
claude plugin marketplace add harikanthl/ezrecord-plugins
claude plugin install ezrecord@ezrecord
```

3. When it asks for the passcode, copy it from ezRecord › Settings › Agents (the copy button beside Passcode; on 1.1.0, copy the MCP address and use the part after `/mcp/`). Claude Code keeps it in your Keychain.

On ezRecord 1.1.1 or later, ezRecord › Settings › Agents › Connect Claude Code does all three steps for you.

Then try: "record a 60 second demo of my app's signup flow", "edit my last recording and add captions", "make three shorts from it", or "dub it into Hindi".

## What's inside

Skills: setup, record-a-demo, edit-a-recording, make-shorts, dub-a-video, plan-a-shoot. They teach Claude ezRecord's workflows; the tools themselves (over 200) come from the app.

## Privacy

ezRecord's tools answer only on your Mac and only with your passcode. Recordings stay on your Mac. Paid services (ElevenLabs, Sarvam) are used only with your own keys and only after you agree to the cost. See https://harikanth.site/ezrecord/privacy.
