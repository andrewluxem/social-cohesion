# social-cohesion

Builds a voluntary team cohesion plan with inclusion, access, boundaries, and review measures.

It produces:

- **Team Cohesion Plan:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Social Cohesion playbook](https://www.andrewluxem.com/playbooks/social-cohesion). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/social-cohesion.git
cp -r social-cohesion/skills/social-cohesion ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r social-cohesion/skills/social-cohesion ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/social-cohesion
/plugin install social-cohesion@social-cohesion
```

For clients that install from an archive, use the versioned [social-cohesion v1.0.0 ZIP](https://www.andrewluxem.com/downloads/social-cohesion-v1.0.0.zip).

## Invoke it

```text
Plan work-connected rituals that build team cohesion
Use the social-cohesion skill.
```

Naming the skill is always valid: `use the social-cohesion skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/social-cohesion/
  assets/team-cohesion-plan-template.md
  LICENSE.md
  meta.yaml
  references/cohesion-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/social-cohesion/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/social-cohesion/LICENSE.md](skills/social-cohesion/LICENSE.md).
