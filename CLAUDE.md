# CLAUDE.md — it-bookmarks

Personal IT bookmarks repo. The README is the product — a clean, scannable list of useful links grouped by topic.

---

## When the user posts a link

1. **Fetch the page** — get the real title and understand what the resource does.
2. **Grab the favicon** — `https://www.google.com/s2/favicons?domain=DOMAIN&sz=16`
3. **Pick a section** — find the best existing H2, or propose a new one if nothing fits.
4. **Draft the entry** and **show it to the user for confirmation** before writing anything.
5. **Write to README.md** after confirmation — append to the end of the section, update the TOC if a new section was created.

If the user includes their own note or opinion about the link, weave it into the description.

---

## README format

### Standard item

```
- ![icon](https://www.google.com/s2/favicons?domain=DOMAIN&sz=16) [Name](url) — One-line description.
```

- Description: one sentence max, value-focused — *why* this is useful, not just what it is
- Start with a capital letter, end with a period
- For starred items, add ⭐ at the start of the description (after the `—`)

### Sub-resource (rare)

Indented directly below the parent, prefixed with `↳`:

```
- ![icon](https://www.google.com/s2/favicons?domain=DOMAIN&sz=16) [Parent Site](url) — Main description.
  - ↳ [Specific Guide](url/subpath) — What this sub-page adds.
```

### Section headers (H2)

Emoji prefix + descriptive title. Established sections:

| Section | Header | What belongs here |
|---|---|---|
| AI & Agents | `## 🤖 AI & Agents` | AI models, assistants, agent frameworks, MCP servers |
| Tools & Productivity | `## 🛠️ Tools & Productivity` | Dev tools, editors, IDEs, terminals, project management |
| Backend & Cloud | `## ☁️ Backend & Cloud` | Hosting, databases, cloud platforms, infrastructure |
| Frontend | `## ⚛️ Frontend` | UI libraries, browser APIs, CSS tools |
| Design & UI | `## 🎨 Design & UI` | Design tools, inspiration, UI resources |
| Interview Prep | `## 🎓 Interview Prep` | Coding practice, interview guides |

When proposing a new section, suggest an emoji that fits the topic. Confirm with the user before creating it.

### Table of Contents

Lives at the top of the README under the intro line. Update it whenever a new section is added.

---

## Confirmation prompt

When presenting a drafted entry, use this format:

```
**Section:** ## 🤖 AI & Agents

**Entry:**
- ![icon](favicon-url) [Name](url) — Description.

Confirm, or let me know what to change.
```

If proposing a new section, show the full section header and ask the user to confirm the name and emoji before creating it.

---

## Sorting

Within each section, products come before repos. Append new items to the **end** of their group (products or repos). The user reorders manually beyond that.

---

## What NOT to do

- Don't create files other than README.md (no separate category files)
- Don't reorder existing entries without being asked
- There is no `## ⭐ Must-Read` section — starred items use ⭐ at the start of their description instead
