<div align="center">

# Developer Systems Studio

**Build foundational developer technologies: languages, compilers, operating systems, browsers, databases, and protocols.**

`1 Master Skill` · `10 Internal Modules` · `Claude Code` · `OpenCode`

</div>

---

## About

Engineer low-level systems through explicit specifications, staged implementations, conformance tests, fuzzing where appropriate, and measured performance.

This repository exposes one discoverable skill: `developer-systems-studio`. Specialist playbooks live inside that skill's `references/` directory and are loaded by the master workflow as needed. You do not select each module separately.

## Quick start

### Project-local use

Copy this repository's `.claude/skills/developer-systems-studio/` folder into the target project's `.claude/skills/` directory. Then invoke the master skill from your compatible coding agent.

### Claude Code

```text
/developer-systems-studio
```

### OpenCode

```text
@developer-systems-studio
```

Agent discovery behavior can vary by installed version and configuration. Confirm the skill appears in the agent's available skill list before relying on it.

## Internal specialist modules

| Module | Role |
|---|---|
| `programming-language-engineer` | Internal specialist reference |
| `compiler-engineer` | Internal specialist reference |
| `operating-system-engineer` | Internal specialist reference |
| `browser-engineer` | Internal specialist reference |
| `database-internals-engineer` | Internal specialist reference |
| `network-protocol-engineer` | Internal specialist reference |
| `blockchain-engineer` | Internal specialist reference |
| `human-centered-product-design` | Shared human-centered quality reference |
| `design-quality-critic` | Shared human-centered quality reference |
| `product-experience-engineer` | Shared human-centered quality reference |

## Repository layout

```text
developer-systems-studio/
├── .claude/skills/developer-systems-studio/
│   ├── SKILL.md
│   ├── references/
│   ├── scripts/
│   ├── templates/
│   └── assets/
├── scripts/
├── README.md
├── README_BN.md
└── AGENTS.md
```

## Validation

Run: `python scripts/validate_pack.py`

The validator checks the master skill, expected reference files, frontmatter, basic link integrity, and accidental secrets. It does not prove provider/API availability or guarantee production behavior.

## Safety and service requirements

This repository contains agent instructions, reference playbooks, templates, and helper scripts. It is not itself a model, API subscription, cloud runtime, media-generation engine, or deployment service. Actual capabilities depend on tools, credentials, permissions, provider terms, quotas, dependencies, and hardware configured in your environment. Never commit secrets.

## Contribution and updates

Keep the master skill as the sole discoverable entry point. Add new specialist knowledge as internal references unless there is a deliberate decision to expose a new independent skill. Update the manifest and validation checks whenever modules change.
