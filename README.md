# Design skills for Claude Code

A set of 6 skills for [Claude Code](https://claude.ai/code) that encode a structured design process. Five cover the core stages of design work; one runs across all of them, focused on communicating with stakeholders. They save time without sacrificing quality.

---

## The problem they solve

AI tools are fast, but they don't have a point of view. Left to their defaults, they produce generic outputs that skip the parts of design that matter most: framing the right problem, explaining tradeoffs, knowing when to push back.

These skills fix that. Each one encodes not only what to do, but how to think about the work — what tradeoffs to consider, what signals to look for, and what good looks like in context. The result is a thinking partner that works the way a rigorous designer works, not a generic content generator.

---

## The 6 skills

The five core skills are designed to be used in sequence, but each works independently for focused tasks.

| # | Skill | What it does |
|---|-------|-------------|
| 01 | `research-and-landscape` | Gathering evidence, analyzing the competitive landscape, and building a grounded understanding of users before any design work begins |
| 02 | `problem-framing-and-planning` | Establishing clarity on the problem, its significance, the criteria for success, and a deliberate plan for the approach |
| 03 | `design-and-systems-thinking` | Divergent exploration, deliberate convergence, and design decisions that account for user needs, business constraints, and technical feasibility simultaneously |
| 04 | `prototyping` | Building interactive prototypes where design principles carry into the artifact, not get abandoned the moment code is written |
| 05 | `validation-and-iteration` | Evaluating design work against its stated goals and guiding what comes next: ship, iterate, rethink, or reframe |
| ✦ | `impact-and-communication` | Communicating design work to different audiences at every stage. Not a step — a practice that runs throughout the whole process |

---

## How to use them

**Option 1 — Global install (recommended)**
Copy the skill folders into your global Claude Code commands directory so they're available in any project:

```bash
cp -r design-skills-claude-code/* ~/.claude/commands/
```

Then call any skill from Claude Code with:

```
/research-and-landscape
/problem-framing-and-planning
/design-and-systems-thinking
/prototyping
/validation-and-iteration
/impact-and-communication
```

**Option 2 — Project-level install**
Copy the folders into your project's `.claude/commands/` directory to use them only within that project.

---

## About

These skills were built by [Florencia Ravitti](https://florenciaravitti.com), a product designer with a background in design systems, growth, and AI tools.

The process behind them is documented in the [full case study](https://florenciaravitti.com/case-studies/claude-skills.html).

---

## License

Licensed under the [MIT License](LICENSE). Free to use, adapt, and share — a credit or link back is appreciated.
