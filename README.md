# Swift Engineering — Agent Skill

An agent skill that guides AI coding assistants to act as senior Swift engineers — writing, reviewing, refactoring, and debugging idiomatic, production-quality Swift for Apple platforms.

**Skill name:** `swift-engineering`
**Trigger description:** Expert Swift programming, modern language features, concurrency, type safety, error handling, and maintainable Apple-platform code. Use when writing, reviewing, refactoring, or debugging Swift.

---

## What It Does

When loaded into an AI coding assistant (Manus, Claude Code, Cursor, Codex, OpenCode, and others that support the agent skill format), this skill enforces professional Swift engineering discipline:

- **Idiomatic Swift first** — value types over references, immutability by default, explicit state machines modeled with enums, and safe optional handling.
- **Modern concurrency** — structured concurrency (`async`/`await`, `TaskGroup`), actor isolation, `Sendable` conformance, `@MainActor` UI discipline, and avoiding unsafe escapes such as `Task.detached`.
- **Clean architecture** — separated business logic, dependency injection, small cohesive types, and protocol-oriented design over deep inheritance trees.
- **Debugging discipline** — root-cause analysis, concurrency diagnostics, honest verification reports, and never claiming code compiles or tests pass without running them.
- **Complete output** — deliver complete, compilable code rather than vague pseudocode, with brief explanations of important tradeoffs.

---

## Installation

### Manus

1. Open Manus → **Settings → Skills**.
2. Click **Import from GitHub** and enter:

   ```
   https://github.com/mshanghai570/swift-engineering-agent-skill-
   ```

3. Or import directly with one click:
   **[Import to Manus](https://manus.im/app#settings/skills/import?githubUrl=https://github.com/mshanghai570/swift-engineering-agent-skill-)**

### Claude Code / Codex / OpenCode (`npx skills`)

```bash
npx skills add mshanghai570/swift-engineering-agent-skill-
```

### Manual installation

Clone this repository into your agent's skills directory:

```bash
git clone https://github.com/mshanghai570/swift-engineering-agent-skill-.git swift-engineering
```

Common locations:

- **Manus (Cloud / Local):** `/home/ubuntu/skills/swift-engineering/` or `~/.manus/user-skills/swift-engineering/`
- **Claude Code:** `~/.claude/skills/swift-engineering/`

---

## Repository Structure

```
swift-engineering-agent-skill-/
├── SKILL.md        # The skill specification (frontmatter + instructions)
├── README.md       # This file
├── LICENSE         # MIT License
└── .gitignore
```

---

## License

[MIT](LICENSE) © mshanghai570
