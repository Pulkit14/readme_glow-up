---
name: readme-glow-up
description: Rewrites a repository's README into a clear, inviting one. Use when the user asks to improve, rewrite, fix, or "glow up" a README, or shares a repo with a weak or missing README. Reads the real code first, then writes pitch, features, install, usage, and license, using only facts found in the repo.
---

# README Glow-Up

Turn a weak or missing README into one people want to read. Every claim must come from the repo itself.

## When to use
- User says: "improve my README", "glow up this README", "write a README for this repo"
- User shares a repo or folder with a thin README

## When NOT to use
- Writing API docs or full documentation sites
- Editing code
- Writing a README for a repo you have not read

## Process

### 1. Scan the repo
Read, in this order, whatever exists:
1. Existing README
2. `package.json`, `pyproject.toml`, `requirements.txt`, `Cargo.toml`, `pubspec.yaml`
3. Entry files (`index.*`, `main.*`, `App.*`, `bin/*`)
4. Folder structure (top two levels)
5. `LICENSE`, `.env.example`, scripts or Makefile
6. Any `examples/`, `demo/`, `screenshots/` folder

### 2. Extract the facts
Write down, privately:
- **What it does**, in one sentence a stranger understands
- **Who it is for**
- **Stack and requirements** (language, runtime version, dependencies)
- **How to install** (exact commands from the repo)
- **How to run or use it** (exact commands or a real code snippet)
- **License** (from the LICENSE file only)

If a fact is not in the repo, do not invent it. Mark it as a gap (step 5).

### 3. Write the README
Use this structure. Drop any section that has no real content.

```
# <emoji> <name>
<one-line pitch: what it does + why it matters>

<screenshot or GIF placeholder if no image exists>

## Features
- 3 to 6 bullets, each a concrete capability found in the code

## Install
<exact commands, in a code block>

## Usage
<smallest working example, taken from the code or examples folder>

## How it works   (optional, only if non-obvious)
<3 to 5 sentences>

## Contributing   (optional)
<2 lines>

## License
<license name from the LICENSE file>
```

### 4. Style rules
- Pitch is one line, plain words, no buzzwords ("revolutionary", "powerful", "seamless")
- Lead with what the reader gets, not how it was built
- Commands go in code blocks and must be copy-paste ready
- Short sentences. No walls of text
- One emoji in the title is fine. No emoji spam
- Keep the original author's voice if the old README had a clear one

### 5. Report the gaps
After the README, add a short "Gaps" list for the user:
- Missing screenshot or GIF
- Missing LICENSE file
- Install command could not be verified
- No usage example found in the repo
- Anything you had to leave out because the repo did not say

### 6. Deliver
- Save as `README.md` (do not overwrite the old one; save the old one as `README.old.md` if the user wants a backup)
- Show the user a short before/after summary: what changed and why

## Hard rules
- Never invent features, commands, badges, or numbers
- Never add fake badges (build passing, coverage, downloads)
- Never claim a license that is not in the repo
- If the repo is too small to read confidently, ask one question instead of guessing
