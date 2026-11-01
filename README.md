# dsh-fat-fish

English | [中文](README.zh.md)

A draggable fish-maid desk pet for the DeepSeek Harness Web UI. It reminds you to drink water and stand up, keeps a small daily log, and reacts to how often you actually do those things.

![Chubby Fish Buddy](assets/default-avatar.webp)

## Features

- A floating, draggable desk pet with idle bobbing, blinking, bubbles, and a forward-swim dash.
- Water and walk reminders with configurable intervals, pause/resume, snooze, and one-click logging.
- Daily water/walk counts plus a compact recent-history view.
- Custom avatar import: PNG, JPG, WebP, and GIF; resized locally to 1024px and stored only in this browser.
- Free pet scaling from 60% to 200%; default 165%.
- Frequency-aware inner monologue, meme-flavored thoughts, and rapid-click roasts.
- An original Manbo-style chime synthesized with Web Audio. No third-party recordings or samples are bundled.
- Settings, history, avatar, scale, and position survive reloads through `localStorage`.

## Requirements

- DSH Web with the `shell.overlay` slot (tested with DSH `0.2.1-rc.3`).
- No build step and no extra services.

## Install

The package is a ready-to-install DSH bundle. Once it is listed in the DSH Plugin Market, install it there. For local development, install the package directory through the DSH plugin manager.

## Sound and privacy

- The reminder chime is generated at runtime with the Web Audio API. It is an original Manbo-style composition, not a copy of any existing recording or melody.
- Reminder schedules, daily counts, settings, avatar, scale, and position stay in browser `localStorage`. The plugin makes no network requests for these features.

## Development

The repository is the package root. There is no build step: edit `client.js` and the locale files, then install the directory with the DSH plugin manager.

## License

Code is MIT-licensed. The bundled default character artwork and plugin icon are covered by the asset notice in [NOTICE.md](NOTICE.md).
