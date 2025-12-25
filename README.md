# My Claude Skills

A collection of 22 Claude Code skills for extending Claude's capabilities with specialized knowledge and workflows.

## Installation

Clone this repo into your project or home directory:

```bash
git clone https://github.com/rohunvora/my-claude-skills.git
```

Skills are automatically discovered by Claude Code from `.claude/skills/`.

## Skills

### Context Engineering (9 skills)

| Skill | Purpose |
|-------|---------|
| `advanced-evaluation` | LLM-as-Judge techniques: direct scoring, pairwise comparison, bias mitigation |
| `context-compression` | Summarization strategies for long-running agent sessions |
| `context-degradation` | Recognize and mitigate failure patterns (lost-in-middle, poisoning, distraction) |
| `context-fundamentals` | Core concepts of context anatomy in agent systems |
| `context-optimization` | Compaction, masking, caching strategies to extend effective context |
| `evaluation` | Assessment frameworks for testing agent performance |
| `memory-systems` | Short-term, long-term, and graph-based memory architectures |
| `multi-agent-patterns` | Orchestrator, peer-to-peer, hierarchical agent architectures |
| `tool-design` | Design tools that agents can use effectively |

### UX/Design (6 skills)

| Skill | Purpose |
|-------|---------|
| `build-design-system` | Design Graph methodology: scales → components → variants → themes |
| `fix-hierarchy` | Apply Von Restorff, Serial Position, Prägnanz to fix visual hierarchy |
| `fix-spacing` | Apply Laws of Proximity, Common Region, Connectedness to fix spacing |
| `improve-flow` | Apply Peak-End Rule, Goal-Gradient, Zeigarnik Effect to improve user flow |
| `structure-app` | Object-Oriented UX for structuring app information architecture |
| `ui-density` | Matt Ström's 4-dimensional framework for analyzing UI density |

### Workflow (4 skills)

| Skill | Purpose |
|-------|---------|
| `changelog-generator` | Transform git commits into user-friendly release notes |
| `extract-insights` | Extract insights from Are.na channels and curated reference collections |
| `reframe` | Reframe stuck problems using WHO/WHERE/WHAT shifts and inversion |
| `spec-first` | Enforce spec → plan → execute → verify loop before writing code |

### Development (2 skills)

| Skill | Purpose |
|-------|---------|
| `html-tools` | Build single-file browser apps without React or build steps |
| `prompt-engineering` | Agent prompting patterns, persuasion principles, context management |

### Meta (1 skill)

| Skill | Purpose |
|-------|---------|
| `skill-creator` | Guide for creating new Claude Code skills |

## Usage

Skills activate automatically when relevant. To invoke manually:

```
/skill-name
```

Or reference in conversation: "Use the spec-first approach for this feature."

## Skill Highlights

### spec-first
Enforces a disciplined development workflow:
1. Frame the problem (conversation)
2. Write `spec.md` (freeze decisions)
3. Generate `todo.md` (plan with verification commands)
4. Execute (small diffs, frequent verification)
5. Verify (adversarial review)
6. Decide what lasts

### ui-density
Analyzes interfaces using Matt Ström's 4-dimensional framework:
- **Visual density** — what users perceive
- **Information density** — Tufte's data-ink ratio
- **Design density** — explicit vs implicit (Gestalt) decisions
- **Temporal density** — value delivered per unit time

### html-tools
Patterns for building single-file browser apps:
- URL state persistence for shareable links
- localStorage for secrets
- Copy-paste as universal data transfer
- Direct browser calls to CORS-enabled APIs
- Pyodide for Python in browser

### build-design-system
Implements Brent Jackson's Design Graph:
```
Scales → Components → Variants → Themes
```
Mathematical foundations: powers of 2, limited palettes, constrained choices.

## Sources

- Context engineering skills adapted from [Agent-Skills-for-Context-Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering)
- UX skills grounded in [Laws of UX](https://lawsofux.com)
- html-tools based on [Simon Willison's patterns](https://simonwillison.net/2025/Dec/10/html-tools/)
- build-design-system based on [Brent Jackson's Design Graph](https://jxnblk.com/blog/design-graph/)
- ui-density based on [Matt Ström's UI Density](https://matthewstrom.com/writing/ui-density/)

## License

MIT
