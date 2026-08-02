# Deep Search Principles

[![skills.sh](https://skills.sh/b/zheminlin266/deep-search-principles)](https://skills.sh/zheminlin266/deep-search-principles)

A reusable agent skill for rigorous deep research, industry analysis, competitor research, and multi-source reports.

[中文说明](README.zh-CN.md)

## What it does

`deep-search-principles` gives an AI agent a repeatable research workflow that emphasizes:

- Traceable claims with Markdown citations
- Independent sources and cross-validation
- Clear separation of facts, estimates, guidance, consensus, and analysis
- Source freshness, provenance, and evidence quality
- Query expansion, retries, saturation checks, and coverage tracking
- Counterevidence, failure modes, and opposing views
- Evidence ledgers and coverage matrices for important claims
- Protection against prompt injection in external content

This skill defines research discipline. It does not provide a search engine, paid data, or a fixed list of sources.

## Install

After publishing this repository, install it with the open agent skills CLI:

```bash
# Replace with the public GitHub repository owner and name.
npx skills add <owner>/<repo> --skill deep-search-principles

# Install globally and skip prompts.
npx skills add <owner>/<repo> --skill deep-search-principles -g -y
```

You can also install it manually by placing `SKILL.md` in the skill directory supported by your agent.

## Use it when

Use this skill for requests such as:

- Deep research or literature-style reviews
- Industry, market, or competitor analysis
- Product, company, technology, or policy research
- Reports that require recent, multi-source, auditable evidence

It is usually unnecessary for a simple factual lookup, casual brainstorming, or a short summary that does not require an evidence trail.

## Repository layout

```text
.
├── SKILL.md             # The installable skill
├── README.md            # English documentation
├── README.zh-CN.md      # 中文文档
├── LICENSE              # MIT License
└── .gitignore
```

The repository keeps `SKILL.md` at the root so it can be discovered as a single-skill repository by the skills CLI and indexed by [skills.sh](https://skills.sh/).

## Compatibility

The skill follows the portable `SKILL.md` format and does not require runtime dependencies. It can be used with skills-compatible agents, including Codex, Claude Code, Cursor, OpenCode, and others supported by the skills CLI.

## Updating the skill

Edit `SKILL.md`, keep the YAML frontmatter valid, and push the change to the public GitHub repository. The repository is the source of truth; skills.sh can index the public repository without a separate generated package.

## Contributing

Improvements should make evidence more traceable, source selection more rigorous, or the workflow easier to execute. Do not add fabricated examples, URLs, statistics, or claims.

## License

[MIT](LICENSE)
