# Test Plan — Metal Garden

| Field       | Details           |
| ----------- | ----------------- |
| Document ID | TP-001            |
| Game        | Metal Garden      |
| Author      | Brendo de Araujo  |
| Date        | June 2026         |
| Version     | 1.0               |

---

## 1. Objective

Define the testing scope, approach, and coverage areas for Metal Garden as part of a structured Game QA assessment. This plan focuses on validating enemy AI behavior, collision systems, and checkpoint mechanics based on findings from Exploratory Session 001.

---

## 2. Scope

| System | Description |
| --- | --- |
| Enemy AI — Aquatic | Attack patterns and positional response behavior |
| Enemy AI — Dodge | Trigger conditions and post-dodge landing validation |
| Player-Enemy Collision | Hitbox accuracy and player-enemy overlap prevention |
| Environmental Collision | Moving hazards — Phase 3 gear structures |
| Checkpoint System | Safe point activation and area state on return |
| Resource Respawn | Health items, ammunition, and grenades after checkpoint cycle |

---

## 3. Out of Scope

- Multiplayer and network functionality
- Formal audio testing
- Localization and text review
- Performance benchmarking
- Narrative, cutscene, and dialogue content
- Any system or area not listed in Section 2

---

## 4. Risks

| Risk | Impact | Mitigation |
| --- | --- | --- |
| Single tester — no cross-validation | Findings may reflect individual play patterns | Retest confirmed defects across multiple sessions |
| BUG-003 has low reproduction rate | Defect may be intermittent or environment-specific | Dedicated retest session scheduled |
| Design intent unknown for OBS-001 | Respawn behavior cannot be confirmed as bug or feature | Logged as pending design validation |
| Game version confirmed as 2.7.2 | Results are tied to this specific build | Retest required if version changes |

---

## 5. Test Approach

- **Session-Based Exploratory Testing (SBET)** for open-ended discovery in unexplored areas
- **Manual test case execution** for structured coverage of in-scope systems
- Defects documented using the internal bug report template (ID, Severity, Priority, Steps, Evidence)
- Design and balance concerns logged separately under `observations/`
- All confirmed defects require video or screenshot evidence before status closure

---

## 6. Test Environment

| Field | Details |
| --- | --- |
| Platform | PC |
| Operating System | Windows 10 |
| Input Method | Keyboard / Mouse |
| Game Version | 2.7.2                    |

---

## 7. Areas Under Test

| # | Area | System | Related Findings |
| --- | --- | --- | --- |
| 1 | Aquatic Zone | Enemy AI — attack behavior and positional reactions | BUG-001 |
| 2 | General | Enemy AI — dodge trigger and landing validation | BUG-003 |
| 3 | Aquatic Zone | Player-enemy collision and hitbox accuracy | BUG-002 |
| 4 | Phase 3 End Section | Environmental collision — moving gear structures | BUG-004 |
| 5 | World / Traversal | Checkpoint activation and area state on return | OBS-001 |
| 6 | World / Traversal | Resource respawn after checkpoint cycle | OBS-001 |

---

## 8. Exit Criteria

- All 15 test cases in `test-cases/metal-garden/combat-and-collision-test-cases.md` executed with results recorded
- BUG-003 retested and status updated to Confirmed or Cannot Reproduce
- All confirmed defects have video or screenshot evidence attached
- OBS-001 respawn behavior documented with evidence
- Session notes updated with final coverage summary and open items
