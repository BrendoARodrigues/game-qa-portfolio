# Exploratory Session 001 — Metal Garden

| Field         | Details                          |
| ------------- | -------------------------------- |
| Session ID    | SESSION-001                      |
| Game          | Metal Garden                     |
| Date          | 2026-06-11                       |
| Tester        | Brendo de Araujo                 |
| Duration      | [Insert duration]                |
| Area Tested   | Multiple Areas — Aquatic Zone, Enemy AI, Phase 3 End Section |
| Session Type  | Unstructured Exploratory Testing |

---

## Charter

Explore the aquatic zone and its enemy interactions to identify behavioral anomalies, collision inconsistencies, and design concerns that affect gameplay quality and player experience.

---

## Summary

This session covered multiple areas of Metal Garden including the aquatic zone, enemy AI interactions, and the end section of Phase 3. Four reproducible bugs and one design observation were identified, spanning enemy behavior, player-enemy collision, AI movement, and environmental collision.

---

## Findings

| ID                                                              | Type        | Title                                                                           | Severity |
| --------------------------------------------------------------- | ----------- | ------------------------------------------------------------------------------- | -------- |
| [BUG-001](../../bug-reports/metal-garden/BUG-001.md)           | Bug         | Aquatic enemy stops attacking when player positions underneath it               | Medium   |
| [BUG-002](../../bug-reports/metal-garden/BUG-002.md)           | Bug         | Player can stand on or clip into aquatic enemy model                            | Low      |
| [BUG-003](../../bug-reports/metal-garden/BUG-003.md)           | Bug         | Enemy clips into wall during dodge animation                                    | Medium   |
| [BUG-004](../../bug-reports/metal-garden/BUG-004.md)           | Bug         | Player clips inside giant gear structure at end of Phase 3                      | Medium   |
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
- [x] Enemy dodge behavior and landing validation
- [x] Environmental collision — moving structures (Phase 3)
- [x] Resource and enemy respawn behavior after checkpoint
- [ ] Full aquatic area traversal
- [ ] All enemy types and dodge variants
- [ ] Edge cases involving multiple enemies simultaneously
