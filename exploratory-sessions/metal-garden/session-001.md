# Exploratory Session 001 — Metal Garden

| Field         | Details                          |
| ------------- | -------------------------------- |
| Session ID    | SESSION-001                      |
| Game          | Metal Garden                     |
| Date          | 2026-06-11                       |
| Tester        | Brendo de Araujo                 |
| Duration      | [Insert duration]                |
| Area Tested   | Aquatic Zone — Enemy Encounters  |
| Session Type  | Unstructured Exploratory Testing |

---

## Charter

Explore the aquatic zone and its enemy interactions to identify behavioral anomalies, collision inconsistencies, and design concerns that affect gameplay quality and player experience.

---

## Summary

This session covered the aquatic zone of Metal Garden with focus on enemy behavior, player-enemy collision, and resource management. Two reproducible bugs and one design observation were identified. All findings are contained to the aquatic area and the broader traversal loop.

---

## Findings

| ID                                                              | Type        | Title                                                                           | Severity |
| --------------------------------------------------------------- | ----------- | ------------------------------------------------------------------------------- | -------- |
| [BUG-001](../../bug-reports/metal-garden/BUG-001.md)           | Bug         | Aquatic enemy stops attacking when player positions underneath it               | Medium   |
| [BUG-002](../../bug-reports/metal-garden/BUG-002.md)           | Bug         | Player can stand on or clip into aquatic enemy model                            | Low      |
| [OBS-001](../../observations/metal-garden/OBS-001.md)          | Observation | Enemies and resources respawn indefinitely after returning to a cleared area    | N/A      |

---

## Session Notes

- The player cannot attack while underwater, which limits offensive interaction testing in this area.
- No XP system, loot, or economy mechanics are present in the tested zone. The exploit potential of BUG-001 is contained to trivializing the encounter without further consequence.
- OBS-001 requires design intent clarification before it can be classified as a defect. The behavior may be an intentional safeguard against resource lockout.

---

## Coverage

- [x] Aquatic enemy attack behavior
- [x] Player-enemy collision and hitbox accuracy
- [x] Resource and enemy respawn behavior after checkpoint
- [ ] Full aquatic area traversal
- [ ] All enemy types in the zone
- [ ] Edge cases involving multiple enemies simultaneously
