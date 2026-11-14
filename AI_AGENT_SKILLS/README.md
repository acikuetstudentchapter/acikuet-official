# AI Agent Skills & Plugins Master Collection
**Curated for Shakil Ilhan**

This standalone folder contains the **6 leading open-source AI agent skills, harnesses, and coding rule repositories** downloaded directly from GitHub. You can copy, link, or reference them across any of your current or future software projects.

---

## The 6 Downloaded Repositories

### 1. `addyosmani-agent-skills`
- **Origin**: [github.com/addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)
- **Author**: Addy Osmani (Head of Chrome Engineering at Google)
- **Focus**: Structured AI agent lifecycle workflows:
  - `spec` — Transform requirements into clear technical specifications.
  - `plan` — Create architectural execution roadmaps before writing code.
  - `build` — Code generation with strict test-driven checkpoints.
  - `test` & `review` — Automated verification, linting, and quality review.
  - `simplify` & `ship` — Refactoring and deployment procedures.

### 2. `andrej-karpathy-skills`
- **Origin**: [github.com/multica-ai/andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills)
- **Author**: Andrej Karpathy (Former Director of AI at Tesla, OpenAI co-founder)
- **Focus**: "One file, fewer coding mistakes."
  - High-leverage rules that eliminate common hallucinations and subtle bugs.
  - Strict coding conventions, minimal dependencies, and readable architectures.

### 3. `everything-claude-code` (ECC)
- **Origin**: [github.com/affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code)
- **Author**: Affaan Mustafa
- **Focus**: Complete operating system for AI agent harnesses:
  - 260+ agent skills and prompt behaviors.
  - Persistent memory architectures and agent hooks.
  - Security scanning and sandbox permission constraints.

### 4. `mattpocock-skills`
- **Origin**: [github.com/mattpocock/skills](https://github.com/mattpocock/skills)
- **Author**: Matt Pocock (TypeScript creator / AI Hero)
- **Focus**: "AI Skills for Real Engineers."
  - Professional TypeScript patterns, strict type-safety, and API modeling.
  - `ask-matt` and interactive documentation interrogation routines.
  - Idea-to-ship workflows (`/to-spec`, `/to-tickets`, `/implement`, `/pr`).

### 5. `modern-web-guidance`
- **Origin**: [github.com/googlechrome/modern-web-guidance](https://github.com/googlechrome/modern-web-guidance)
- **Author**: Google Chrome Team
- **Focus**: "Authoritative guidance on modern web development."
  - Modern HTML/CSS, Web APIs, container queries, view transitions, and popovers.
  - Core Web Vitals (LCP, INP, CLS) optimization and accessibility best practices.
  - Multi-platform manifests for Gemini, Claude Code, Cursor, and Codex.

### 6. `ponytail`
- **Origin**: [github.com/DietrichGebert/Ponytail](https://github.com/DietrichGebert/Ponytail)
- **Author**: Dietrich Gebert
- **Focus**: "Writes less, smarter code."
  - Code reduction techniques (-50% boilerplate, +98% test pass rate).
  - Clean abstractions and prompt harnesses for reliable agents.

---

## How to Use These Skills in Any New Project

### Option A: In Antigravity / Gemini CLI
Copy any specific skill or rule into your project's root:
```bash
# Example: Copying Google Chrome's modern-web-guidance or Karpathy's guidelines
cp -r /Users/shakililhan/Downloads/AI_AGENT_SKILLS/modern-web-guidance/.agents /path/to/new-project/
```

### Option B: In Claude Code
Claude Code reads project-level skills or global skills. You can install them directly or point to them:
```bash
# In your project folder
npx skills@latest add /Users/shakililhan/Downloads/AI_AGENT_SKILLS/mattpocock-skills
```

### Option C: In Cursor / Windsurf / VS Code
Each folder already contains `.cursor`, `.windsurf`, or `.gemini` rule files. You can symlink or copy `.cursor/` into your active repository:
```bash
cd /path/to/any-project
cp -r /Users/shakililhan/Downloads/AI_AGENT_SKILLS/andrej-karpathy-skills/.cursor .
```

---

## How to Keep Them Updated
To pull the latest updates from all 6 GitHub repositories in the future, run this one command in your terminal:
```bash
for dir in /Users/shakililhan/Downloads/AI_AGENT_SKILLS/*/; do
  if [ -d "$dir/.git" ]; then
    echo "Updating $dir..."
    git -C "$dir" pull
  fi
done
```
