# video-skills

Kiro skills for making videos entirely in code, copied from
[tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) (see `.kiro/skills/OPUS-VIDEO-SKILLS-LICENSE`).

| Skill | Style |
|---|---|
| `.kiro/skills/painted-animation/` | Hand-painted watercolour and ink cartoons, music videos, karaoke lyric videos |
| `.kiro/skills/kinetic-reel/` | Kinetic typography reels: showreels, portfolio, product and intro films |

## Changes from upstream

- `SKILL.md` scaffold commands use `<skill-dir>` instead of `~/.claude/skills/...`.
- `scripts/new_project.sh` falls back to `cp -a` when `rsync` is not installed.

## Requirements

Node.js, ffmpeg, Chrome/Chromium (set `CHROME_PATH` if it is not in a standard location), and Python 3 with numpy
(only for painted-animation's `beat_grid.py`).

On a machine without a GPU, pass `--soft-gl` to `render.mjs` so WebGL runs on SwiftShader. Expect roughly
20 s per 1080p frame on CPU.
