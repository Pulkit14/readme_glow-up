# ✨ README Glow-Up

A Claude skill that rewrites any repo's README into one people actually read.

It reads your real code first, then writes the pitch, features, install steps, and usage example. It never invents facts, and it lists what it could not verify.

## Before and after

**Before**
```
# journey-card
React component for journeys.
Run npm install.
```

**After**
```
# 🧭 journey-card
A swipeable travel card for React. Drop it in, get a trip preview in 3 lines.

## Install
npm install journey-card

## Usage
<JourneyCard title="Spiti in 5 days" stops={5} />

## License
MIT
```

More in [`examples/`](examples/before-after.md).

## Install

**Claude Code**
```
mkdir -p ~/.claude/skills/readme-glow-up
cp SKILL.md ~/.claude/skills/readme-glow-up/SKILL.md
```

**Claude app**
Zip the `readme-glow-up` folder and upload it in Settings, under Skills.

## Use

Open a repo and say:

> Glow up this README

## What it does
1. Scans the repo: README, package files, entry points, folders
2. Extracts only facts that are really there
3. Writes the new README
4. Lists gaps: missing screenshot, missing license, unverified commands

## Rules it follows
- No invented features, commands, or badges
- No buzzwords in the pitch
- Copy-paste-ready commands

## License
MIT
