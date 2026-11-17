# Video-Vame-creation
Repo to create videogames made WITH AI

## AI game-dev skills

This repo includes 79 game-development [Agent Skills](https://code.claude.com/docs/en/skills) plus a
router, installed project-locally in `.claude/skills/`. Any Claude Code session opened in this repo
picks them up automatically. Just describe what you want ("make a 2D platformer in Godot", "add an
inventory to my Phaser RPG") and the router loads the right engine, genre and system skills.

Covered engines: Godot, Unity, Unreal, Ebitengine, Phaser, PixiJS, three.js, Bevy, pygame, LÖVE,
Defold and Roblox. Also included: cross-engine disciplines (game feel, AI, procedural generation,
saves, UI, audio, shaders, asset creation), genre templates (platformer, roguelike, RPG, FPS, tower
defense, card, visual novel, survival, puzzle) and shipping workflows (game jams, prototyping,
itch.io, Steam, design docs).

Source: [gamedev-skills/awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills)
at commit `c6ca6c4` (2026-11-12), Apache-2.0. License and notice are in
`.claude/skills-licenses/awesome-gamedev-agent-skills/`.

To update to a newer release, re-run the copy from a fresh clone of the source repo:

```bash
git clone --depth 1 https://github.com/gamedev-skills/awesome-gamedev-agent-skills /tmp/gds
rm -rf .claude/skills && mkdir -p .claude/skills
find /tmp/gds/skills -name SKILL.md -exec dirname {} \; | while read -r d; do cp -R "$d" .claude/skills/; done
cp -R /tmp/gds/router .claude/skills/router
```
