# Video-Vame-creation

Repo for making video games with AI.

## Game-dev skills

`.claude/skills/` holds 79 game-development skills and a `router` skill from
[awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills)
(Apache-2.0, see `.claude/skills-licenses/`).

- For any game-development request, load the `router` skill first. It detects the engine from
  project files (`project.godot`, `package.json` with `phaser`/`three`, `*.uproject`, etc.) and
  names the 2–3 engine, discipline, genre or workflow skills to read before writing code.
- If no engine is set up yet, ask which engine to use (or suggest one that fits the idea) before
  scaffolding a project.
- Router tables refer to paths like `skills/godot/...`; here every skill sits flat at
  `.claude/skills/<skill-name>/`.
