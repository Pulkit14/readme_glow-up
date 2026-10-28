# Before and after examples

## 1. React component

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

## 2. Python script

**Before**
```
rename tool
python rename.py
```

**After**
```
# 🗂️ batch-rename
Rename hundreds of files by pattern from the command line.

## Install
pip install -r requirements.txt

## Usage
python rename.py ./photos --pattern "trip_{n}" --start 1

## License
MIT
```

## 3. Claude skill

**Before**
```
my skill
put in skills folder
```

**After**
```
# 🧪 my-skill
Reviews pull requests for mobile layout bugs.

## Install
mkdir -p ~/.claude/skills/my-skill
cp SKILL.md ~/.claude/skills/my-skill/

## Usage
Say: "Review this PR for mobile issues"

## License
MIT
```

## Gaps report example

After each rewrite the skill lists what it could not confirm:
- No screenshot found, add one under the pitch
- No LICENSE file found, license section left out
- Install command not verified against a lockfile
