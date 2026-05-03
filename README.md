# 🚀 AGKit (Antigravity Kit)

> **A comprehensive AI Agent framework with modular Skills, Specialist Agents, and Slash-Command Workflows — designed to supercharge your AI-powered development experience.**

[![Based on Antigravity Kit](https://img.shields.io/badge/Based%20on-Antigravity%20Kit-blueviolet?style=flat-square)](https://github.com/vudovn/antigravity-kit)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

---

## 📖 About

**AGKit** is an extended fork of the excellent [Antigravity Kit](https://github.com/vudovn/antigravity-kit) by [@vudovn](https://github.com/vudovn). It builds upon the original foundation with additional agents, enhanced skills, and expanded workflows tailored for advanced agentic coding.

### What's Different?

This fork includes enhancements and additions on top of the original Antigravity Kit:

- **25 Specialist Agents** — including `oracle`, `librarian`, `plan-consultant`, `plan-reviewer`, and `multimodal-analyst` (ported from OmO patterns)
- **17 Skills** — curated workflow library with `conductor`, `subagent-driven-development`, `verification-before-completion`, `using-git-worktrees`, `finishing-a-development-branch`, `receiving-code-review`, and more
- **32 Workflows** — full Conductor methodology support for context-driven development across sessions

---

## ⚡ Quick Start

### Install into your project

```bash
# Copy the .agent folder into your project root
cp -r .agent /path/to/your-project/
```

### Or clone this repo

```bash
git clone https://github.com/NguyenSiTrung/AGKit.git
```

> **💡 Tip:** If you're using AI editors like **Cursor** or **Windsurf**, do NOT add `.agent/` to `.gitignore` — the IDE needs to index it for slash commands to appear. Instead, add it to `.git/info/exclude` to keep it local.

---

## 🧩 What's Included

| Component      | Count | Description                                                          |
| -------------- | ----- | -------------------------------------------------------------------- |
| **Agents**     | 25    | Specialist AI personas (frontend, backend, security, PM, QA, etc.)   |
| **Skills**     | 17    | Core development workflow and knowledge modules                      |
| **Workflows**  | 32    | Slash command procedures                                             |

---

## 🤖 Intelligent Agent Routing

**No need to memorize agent names!** The system automatically detects your intent and routes to the right specialist:

```
You: "Add JWT authentication"
AI: 🤖 Applying @security-auditor + @backend-specialist...

You: "Fix the dark mode button"
AI: 🤖 Using @frontend-specialist...

You: "Login returns 500 error"
AI: 🤖 Using @debugger for systematic analysis...
```

**How it works:**
- Silently analyzes your request
- Detects domain(s) — frontend, backend, security, devops, etc.
- Selects the best specialist(s)
- Informs you which expertise is being applied

---

## 🤖 Agents (25)

| Agent                    | Focus                      | Key Skills                                               |
| ------------------------ | -------------------------- | -------------------------------------------------------- |
| `orchestrator`           | Multi-agent coordination   | parallel-agents, behavioral-modes, delegation-patterns   |
| `project-planner`        | Discovery, task planning   | brainstorming, plan-writing, architecture                |
| `frontend-specialist`    | Web UI/UX                  | frontend-design, react-best-practices, tailwind-patterns |
| `backend-specialist`     | API, business logic        | api-patterns, nodejs-best-practices, database-design     |
| `database-architect`     | Schema, SQL                | database-design, prisma-expert                           |
| `mobile-developer`       | iOS, Android, RN           | mobile-design                                            |
| `game-developer`         | Game logic, mechanics      | game-development                                         |
| `devops-engineer`        | CI/CD, Docker              | deployment-procedures, docker-expert                     |
| `security-auditor`       | Security compliance        | vulnerability-scanner, red-team-tactics                  |
| `penetration-tester`     | Offensive security         | red-team-tactics                                         |
| `test-engineer`          | Testing strategies         | testing-patterns, tdd-workflow, webapp-testing           |
| `debugger`               | Root cause analysis        | systematic-debugging                                     |
| `performance-optimizer`  | Speed, Web Vitals          | performance-profiling                                    |
| `seo-specialist`         | Ranking, visibility        | seo-fundamentals, geo-fundamentals                       |
| `documentation-writer`   | Manuals, docs              | documentation-templates                                  |
| `product-manager`        | Requirements, user stories | plan-writing, brainstorming                              |
| `product-owner`          | Strategy, backlog, MVP     | plan-writing, brainstorming                              |
| `qa-automation-engineer` | E2E testing, CI pipelines  | webapp-testing, testing-patterns                         |
| `code-archaeologist`     | Legacy code, refactoring   | clean-code, code-review-checklist                        |
| `explorer-agent`         | Codebase analysis          | architecture, systematic-debugging                       |
| `oracle`                 | Strategic technical advisor | architecture, systematic-debugging                       |
| `librarian`              | OSS docs & research        | documentation-templates                                  |
| `plan-consultant`        | Pre-planning analysis      | brainstorming, architecture                              |
| `plan-reviewer`          | Plan validation            | plan-writing, code-review-checklist                      |
| `multimodal-analyst`     | Visual content analysis    | —                                                        |

---

## 🧠 Skills (17)

Skills are loaded automatically based on task context. Organized by domain:

<details>
<summary><strong>Agent Coordination & Workflow</strong> (10 skills)</summary>

| Skill                            | Description                                              |
| -------------------------------- | -------------------------------------------------------- |
| `subagent-driven-development`    | Dispatch subagent per task with two-stage review          |
| `dispatching-parallel-agents`    | Multi-task coordination and execution                    |
| `executing-plans`                | Systematically execute structured development plans      |
| `verification-before-completion` | Evidence-based verification before declaring done         |
| `finishing-a-development-branch` | Structured branch completion: verify, merge/PR, cleanup   |
| `receiving-code-review`          | How to respond to PR review feedback                      |
| `requesting-code-review`         | Process for opening PRs and requesting reviews            |
| `test-driven-development`        | Core methodology for implementing features/fixes          |
| `systematic-debugging`           | Rigorous debugging workflow                               |
| `using-git-worktrees`            | Isolated worktree workspaces for feature development      |

</details>

<details>
<summary><strong>Project Management & Context</strong> (2 skills)</summary>

| Skill                 | Description                                                    |
| --------------------- | -------------------------------------------------------------- |
| `conductor`           | Context-driven development, spec-first coding, TDD tracks      |
| `using-superpowers`   | Establishing how to find and use AI capabilities efficiently   |

</details>

<details>
<summary><strong>Planning & Advisory</strong> (4 skills)</summary>

| Skill                 | Description                              |
| --------------------- | ---------------------------------------- |
| `brainstorming`       | Socratic questioning & discovery         |
| `writing-plans`       | Task planning, breakdown, & structure    |
| `oracle`              | Strategic technical advisor              |
| `librarian`           | OSS docs & research                      |

</details>

<details>
<summary><strong>Agent Customization</strong> (1 skill)</summary>

| Skill                 | Description                              |
| --------------------- | ---------------------------------------- |
| `writing-skills`      | Creating, editing, and verifying skills  |

</details>
---

## 🔄 Workflows (32)

Invoke with slash commands in your AI editor:

### Core Workflows

| Command          | Description                           |
| ---------------- | ------------------------------------- |
| `/brainstorm`    | Socratic discovery & exploration      |
| `/create`        | Create new features or apps           |
| `/debug`         | Systematic debugging                  |
| `/deploy`        | Deploy application                    |
| `/enhance`       | Improve existing code                 |
| `/orchestrate`   | Multi-agent coordination              |
| `/plan`          | Create task breakdown                 |
| `/preview`       | Preview changes locally               |
| `/status`        | Check project status                  |
| `/test`          | Generate and run tests                |
| `/ui-ux-pro-max` | Design with 50 styles                 |
| `/init-deep`     | Deep context initialization           |
| `/ralph-loop`    | Continuous dev loop until completion  |
| `/start-work`    | Execute from planner-generated plan   |
| `/refactor`      | Intelligent refactoring with TDD      |
| `/handoff`       | Session context transfer              |

### Conductor Workflows (Context-Driven Development)

| Command                | Description                              |
| ---------------------- | ---------------------------------------- |
| `/conductor-setup`     | Initialize project with Conductor        |
| `/conductor-newtrack`  | Create new feature/bug track with spec   |
| `/conductor-implement` | Execute tasks from track plan            |
| `/conductor-status`    | Display project progress                 |
| `/conductor-revert`    | Git-aware revert of tracks/phases/tasks  |
| `/conductor-validate`  | Validate project integrity               |
| `/conductor-block`     | Mark task as blocked with reason         |
| `/conductor-skip`      | Skip current task with reason            |
| `/conductor-revise`    | Update spec/plan for implementation issues |
| `/conductor-archive`   | Archive completed tracks                 |
| `/conductor-export`    | Export project summary as markdown       |
| `/conductor-handoff`   | Create context handoff for next session  |
| `/conductor-refresh`   | Sync context docs with codebase state    |
| `/conductor-formula`   | Manage track workflow templates          |
| `/conductor-distill`   | Extract reusable template from track     |
| `/conductor-wisp`      | Quick ephemeral exploration track        |

---

## 📊 Statistics

| Metric              | Value                         |
| ------------------- | ----------------------------- |
| **Total Agents**    | 25                            |
| **Total Skills**    | 17                            |
| **Total Workflows** | 32                            |
| **Total Scripts**   | 2 (master) + 18 (skill-level) |
| **Coverage**        | ~95% web/mobile development   |

---

## 🙏 Credits & Acknowledgments

This project is based on the original **[Antigravity Kit](https://github.com/vudovn/antigravity-kit)** created by **[@vudovn](https://github.com/vudovn)**. Huge thanks for building the foundational framework that makes this possible.

---

## 📄 License

MIT © [NguyenSiTrung](https://github.com/NguyenSiTrung)

Based on [Antigravity Kit](https://github.com/vudovn/antigravity-kit) by [@vudovn](https://github.com/vudovn)
