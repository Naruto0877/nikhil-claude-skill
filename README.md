# Nikhil Claude Skill

Nikhil's personal coding workflow for Claude and Codex: understand the goal, implement the simplest solution, keep the diff focused, and verify the result.

The canonical skill is [skills/nikhil-claude-skill/SKILL.md](skills/nikhil-claude-skill/SKILL.md). It favors completing authorized work and making reasonable routine decisions, with questions reserved for consequential missing information.

## Local skill installation

From the repository root, copy the skill into each tool's personal skills folder. If a destination already exists, review it before replacing it.

```sh
mkdir -p ~/.codex/skills ~/.claude/skills
cp -R skills/nikhil-claude-skill ~/.codex/skills/
cp -R skills/nikhil-claude-skill ~/.claude/skills/
```

Explicit invocation: `$nikhil-claude-skill` in Codex, or `/nikhil-claude-skill` in Claude Code. The description also supports automatic selection for relevant coding tasks.

After editing the canonical skill, copy it to the installed locations again. The installed folders are independent copies.

## Optional Claude Code plugin

The repository also retains the upstream plugin packaging. To use that instead of the direct Claude skill copy:

```text
/plugin marketplace add /Users/nikhilvarma/Desktop/ai-coding-repos/nikhil-claude-skill
/plugin install nikhil-claude-skill@nikhil-skills
```

Choose one Claude installation method to avoid exposing the same skill twice. The direct skill copies are the installation used for this setup.

## Project instructions and maintenance

[CLAUDE.md](CLAUDE.md) contains the same instructions for project use. Merge them with existing project instructions instead of overwriting them. [CURSOR.md](CURSOR.md) covers the included Cursor rule. [EXAMPLES.md](EXAMPLES.md) links to fresh expense-app examples included in the installed skill. They illustrate the principles without imposing app-specific requirements on other projects.

When changing the workflow, keep the skill, CLAUDE.md, and Cursor rule consistent. Plugin metadata must continue pointing to `skills/nikhil-claude-skill`.

## Attribution

Adapted by Nikhil Varma from [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills), originally under `forrestchang/andrej-karpathy-skills`, inspired by Andrej Karpathy's observations. The upstream skill and plugin declare the MIT license. The rewritten workflow and examples are distributed under the included [MIT license](LICENSE). This is Nikhil's adaptation and is not an official Karpathy project.

This is a separate personal repository. The original upstream clone remains intact in the adjacent `andrej-karpathy-skills` folder.
