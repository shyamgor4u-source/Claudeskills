# Claudeskills

The top 10 Claude Code / Codex skill repos by GitHub stars (from [this reel](https://www.instagram.com/reels/DeumR-AE7Xy/)), combined into one `.claude/skills/` folder.

## Use

In a project, Claude Code loads skills from `.claude/skills/`. Personal skills, loaded in every project, live in `~/.claude/skills/`.

Copy all of them into your personal skills:

```bash
git clone https://github.com/shyamgor4u-source/Claudeskills /tmp/claudeskills && mkdir -p ~/.claude/skills && cp -r /tmp/claudeskills/.claude/skills/* ~/.claude/skills/
```

Or copy only the ones you want, e.g. `cp -r .claude/skills/brainstorming ~/.claude/skills/`.

## Heads-up

- **Style skills conflict.** Caveman (`caveman*`, `*cave`) and Ponytail (`ponytail*`) both change how Claude writes every reply. Install one family, not both.
- **Graphify** needs its Python tool too: `pip install graphifyy` (see the upstream repo).
- **Anthropic's docx, pdf, pptx and xlsx skills are not included.** Their license doesn't allow redistribution, and they are already built into claude.ai.
- **Not a skill:** `extras/karpathy-CLAUDE.md` is a CLAUDE.md file. Put its contents in your project's or `~/.claude/CLAUDE.md`.
- `agent-skills-test-driven-development` is Addy Osmani's TDD skill, renamed so it doesn't clash with Superpowers' `test-driven-development`.
- Mirror copies bundled inside the upstream repos (plugin and CLI bundles) were left out.

## Sources

Each skill keeps its upstream license; the repo-level license files are in `licenses/`.

| # | Repo | Commit | Skills |
|---|---|---|---|
| 1 | [obra/superpowers](https://github.com/obra/superpowers) | `22f0b46` | `brainstorming`, `diagnosing-superpowers`, `dispatching-parallel-agents`, `executing-plans`, `finishing-a-development-branch`, `receiving-code-review`, `requesting-code-review`, `subagent-driven-development`, `systematic-debugging`, `test-driven-development`, `using-git-worktrees`, `using-superpowers`, `verification-before-completion`, `writing-plans`, `writing-skills` |
| 2 | [mattpocock/skills](https://github.com/mattpocock/skills) | `4ae2317` | `ask-matt`, `chief-of-staff`, `claude-handoff`, `code-review`, `codebase-design`, `diagnosing-bugs`, `domain-modeling`, `git-guardrails-claude-code`, `grill-me`, `grill-with-docs`, `grilling`, `handoff`, `implement`, `implement-spec`, `improve-codebase-architecture`, `loop-me`, `migrate-to-shoehorn`, `pr`, `prototype`, `research`, `retro`, `scaffold-exercises`, `setup-matt-pocock-skills`, `setup-pre-commit`, `setup-ts-deep-modules`, `software-factory`, `tdd`, `teach`, `to-questionnaire`, `to-spec`, `to-tickets`, `triage`, `wait-what`, `wayfinder`, `wizard`, `writing-beats`, `writing-for-agents`, `writing-fragments`, `writing-shape` |
| 3 | [multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills) | `2c60614` | `karpathy-guidelines` |
| 4 | [anthropics/skills](https://github.com/anthropics/skills) | `ca45fc4` | `academy-guide`, `algorithmic-art`, `brand-guidelines`, `canvas-design`, `claude-api`, `discernment-nudge`, `doc-coauthoring`, `frontend-design`, `internal-comms`, `mcp-builder`, `skill-creator`, `slack-gif-creator`, `theme-factory`, `web-artifacts-builder`, `webapp-testing` |
| 5 | [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) | `96608e0` | `ponytail`, `ponytail-audit`, `ponytail-debt`, `ponytail-gain`, `ponytail-help`, `ponytail-review` |
| 6 | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | `b7d5353` | `banner-design`, `brand`, `design`, `design-system`, `slides`, `ui-styling`, `ui-ux-pro-max` |
| 7 | [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | `16218bf` | `graphify` |
| 8 | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | `4bf8898` | `cavecrew`, `caveman`, `caveman-commit`, `caveman-compress`, `caveman-discover`, `caveman-evidence-review`, `caveman-explore`, `caveman-help`, `caveman-learn`, `caveman-manage`, `caveman-optimize`, `caveman-review`, `caveman-setup`, `caveman-stats`, `investigate-first`, `lean-build`, `megacave`, `migration`, `safe-refactor`, `surgical-patch`, `ultracave`, `verify-and-stop` |
| 9 | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | `301b02b` | `api-and-interface-design`, `browser-testing-with-devtools`, `ci-cd-and-automation`, `code-review-and-quality`, `code-simplification`, `constraint-driven-development`, `context-engineering`, `debugging-and-error-recovery`, `deprecation-and-migration`, `documentation-and-adrs`, `doubt-driven-development`, `frontend-ui-engineering`, `git-workflow-and-versioning`, `idea-refine`, `incremental-implementation`, `interview-me`, `observability-and-instrumentation`, `performance-optimization`, `planning-and-task-breakdown`, `security-and-hardening`, `shipping-and-launch`, `source-driven-development`, `spec-driven-development`, `agent-skills-test-driven-development`, `using-agent-skills` |
| 10 | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | `9b4bf93` | `taste-skill` |
