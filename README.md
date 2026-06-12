# 🎮 Brendo de Araujo - Game QA Portfolio

Welcome to my Game QA Portfolio.

This repository contains practical examples of game testing documentation, including bug reports, test plans, test cases, exploratory testing sessions, and design observations.

The objective of this portfolio is to demonstrate QA methodologies applied to video games while building experience within the Game QA field.

---

## About Me

I am a Quality Assurance Analyst with professional experience in software testing, exploratory testing, regression testing, bug reporting, and test documentation.

My current goal is to transition into the game industry by applying QA best practices to gameplay systems, user experience, progression mechanics, and overall game quality.

This portfolio documents my learning journey and practical experience in Game QA through real testing projects and structured quality analysis.

---

## Contact

- **Email:** brendoarodrigues2012@gmail.com
- **LinkedIn:** [linkedin.com/in/brendo-araujo](https://www.linkedin.com/in/brendo-araujo/)

---

## Skills

### Game QA

* Exploratory Testing
* Gameplay Testing
* Test Planning
* Test Case Design
* Bug Reporting
* Defect Tracking

### Software QA Background

* User Acceptance Testing (UAT)
* Automated Testing (Cypress — web applications)

### Tools

* Jira
* Azure DevOps
* GitHub
* OBS Studio
* ShareX
* Notion

---

## Game Under Test

### Metal Garden

| Field          | Details             |
| -------------- | ------------------- |
| Genre          | Action / Platformer |
| Platform       | PC                  |
| Testing Period | June 2026           |

> Metal Garden is an indie action game featuring multi-phase level design, aquatic zones, and enemy AI with dynamic behaviors including dodge reactions. Players navigate environmental hazards, manage limited resources — health items, ammunition, and grenades — and progress through a checkpoint-gated structure.

---

## Portfolio Projects

### Bug Reports

| ID                                              | Title                                                              | Game         | Severity | Status       |
| ----------------------------------------------- | ------------------------------------------------------------------ | ------------ | -------- | ------------ |
| [BUG-001](bug-reports/metal-garden/BUG-001.md) | Aquatic enemy stops attacking when player positions underneath it  | Metal Garden | Medium   | Confirmed    |
| [BUG-002](bug-reports/metal-garden/BUG-002.md) | Player can stand on or clip into aquatic enemy model               | Metal Garden | Low      | Confirmed    |
| [BUG-003](bug-reports/metal-garden/BUG-003.md) | Enemy clips into wall during dodge animation                       | Metal Garden | Medium   | Needs Retest |
| [BUG-004](bug-reports/metal-garden/BUG-004.md) | Player clips inside giant gear structure at end of Phase 3         | Metal Garden | Medium   | Confirmed    |

---

### Observations

| ID                                                | Title                                                                        | Game         | Status             |
| ------------------------------------------------- | ---------------------------------------------------------------------------- | ------------ | ------------------ |
| [OBS-001](observations/metal-garden/OBS-001.md)  | Enemies and resources respawn indefinitely after returning to a cleared area | Metal Garden | Pending Validation |

---

### Exploratory Sessions

| Session                                                                                   | Game         | Status    |
| ----------------------------------------------------------------------------------------- | ------------ | --------- |
| [Session 001 — Aquatic Zone & Phase 3](exploratory-sessions/metal-garden/session-001.md) | Metal Garden | Completed |

---

### Test Plans

| Project                                                                              | Game         | Status    |
| ------------------------------------------------------------------------------------ | ------------ | --------- |
| [Metal Garden — Full Test Plan](test-plans/metal-garden/test-plan-metal-garden.md)  | Metal Garden | Completed |

---

### Test Cases

| Document                                                                                      | Game         | Cases | Status       |
| --------------------------------------------------------------------------------------------- | ------------ | ----- | ------------ |
| [Combat and Collision](test-cases/metal-garden/combat-and-collision-test-cases.md)            | Metal Garden | 15    | Not Executed |

---

## Portfolio Statistics

| Metric              | Value |
| ------------------- | ----- |
| Games Tested        | 1     |
| Bug Reports Created | 4     |
| Test Plans Created  | 1     |
| Test Cases Designed | 15    |

*Statistics will be updated as new projects are completed.*

---

## Repository Structure

```text
game-qa-portfolio
├── bug-reports
│   └── metal-garden
├── test-plans
│   └── metal-garden
├── test-cases
│   └── metal-garden
├── exploratory-sessions
│   └── metal-garden
├── observations
│   └── metal-garden
├── assets
│   └── metal-garden
│       ├── screenshots
│       ├── gifs
│       └── videos
└── README.md
```

---

## Current Goal

Build a professional Game QA portfolio by testing real games, documenting defects, creating structured test plans, and conducting exploratory testing sessions following industry-standard QA practices.
