# High-Level-Design — Claude Guide

System design concepts, hands-on Python/Docker labs, and HLD interview questions.

## Structure

```
BasicConcepts/      # Theory + runnable demos per concept
  <Concept>/
    README.md
    implementations/   # Individual demos
    demos/             # Comparison tools
    examples/          # Real-world snippets
    quick_start.py     # Interactive entry point (Python 3)
Projects/           # Docker-based practical labs
  <LabName>/
    docker-compose.yml
    README.md
Questions/          # Design interview questions
  <QuestionName>/
    README.md
    (diagrams, code, notes)
```

## Conventions

- **Python 3** for all demos. Most concept folders have a `quick_start.py` that acts as the menu / interactive launcher.
- **Docker Compose** for the `Projects/` labs. Each lab is self-contained and runnable with `docker-compose up -d`.
- **READMEs use emoji section headers** (🛠️ 🎮 🚀 ⚡ 📁) — this is the established style here, keep it when adding concepts. (Contrast with the other two repos which stay emoji-free.)

## Status markers

In `README.md` question tables:
- Completed: `:white_check_mark:`
- In progress: `:construction:`
- Not started: `&#9744;`

Questions are bucketed as **Easy / Medium / Hard**.

## When adding a new BasicConcept

1. Create `BasicConcepts/<Concept>/` with the sub-folders above.
2. Include a `quick_start.py` — the entry point the root README will link to.
3. Add an entry in the root `README.md` under "Basic Concepts" with the 📁 + 🚀 blocks matching the existing style.
4. If it needs a Docker lab, add `Projects/<Concept>Lab/` and link it from the concept's README.

## When adding a new Question

1. Create `Questions/<Name>/README.md` with: problem statement, requirements, capacity estimation, API design, data model, HLD diagram, deep dives, bottlenecks.
2. Add a row to the appropriate difficulty table in the root `README.md`.

## Helpers

- Run `/status-report` to audit progress across Easy/Medium/Hard questions.

## Cross-repo links

- LLD equivalents → `../Low-Level-Design-Questions/`
- Java fundamentals → `../Basics_Java_With_OOP_Concepts/`
