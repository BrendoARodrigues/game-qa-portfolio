# Combat and Collision Test Cases — Metal Garden

| Field            | Details                                                          |
| ---------------- | ---------------------------------------------------------------- |
| Document ID      | TC-METAL-GARDEN-001                                              |
| Game             | Metal Garden                                                     |
| Author           | Brendo de Araujo                                                 |
| Date             | June 2026                                                        |
| Area             | Enemy Combat, Enemy Collision, Environmental Collision, Checkpoints, Resources |
| Total Cases      | 15                                                               |
| Execution Status | Not Executed                                                     |

---

## Test Cases

| ID | Test Case | Preconditions | Steps | Expected Result | Status |
| --- | --- | --- | --- | --- | --- |
| TC-001 | Aquatic enemy initiates attack on player approach | Player in aquatic zone; enemy in idle/patrol state | 1. Enter aquatic zone.<br>2. Approach enemy until within attack range.<br>3. Observe enemy response. | Enemy detects player and initiates attack behavior. | Not Executed |
| TC-002 | Aquatic enemy attack behavior when player is directly below | Player engaged with aquatic enemy in attack state | 1. Trigger enemy attack.<br>2. Move player directly below the enemy.<br>3. Remain stationary.<br>4. Observe enemy behavior. | Enemy continues attack regardless of player's vertical position. | Not Executed |
| TC-003 | Aquatic enemy resumes attack after player exits position below | Player is below enemy and enemy is idle (BUG-001 condition) | 1. Position player below enemy until attack stops.<br>2. Move player to a lateral position.<br>3. Observe enemy response. | Enemy resumes attack when player is no longer in the blind spot. | Not Executed |
| TC-004 | Player blocked by aquatic enemy collision — all directions | Player in aquatic zone; aquatic enemy present | 1. Walk player into enemy from the front.<br>2. Repeat from left, right, and behind.<br>3. Observe collision response each time. | Player is blocked by the enemy collision volume; no model overlap occurs from any direction. | Not Executed |
| TC-005 | Player cannot stand on top of aquatic enemy model | Player in aquatic zone; aquatic enemy present | 1. Position player above enemy.<br>2. Move downward onto the top surface of the model.<br>3. Observe player-enemy interaction. | Collision blocks or displaces player; player cannot stand on enemy model. | Not Executed |
| TC-006 | Enemy dodge triggers on player approach | Dodge-capable enemy present in an open area | 1. Approach dodge-capable enemy slowly from the front.<br>2. Note the distance at which the dodge triggers.<br>3. Repeat approach from the left and right sides. | Dodge triggers consistently within a defined range from all approach directions. | Not Executed |
| TC-007 | Enemy dodge lands on a valid surface in open area | Dodge-capable enemy in open area with platforms nearby | 1. Trigger enemy dodge in an open space.<br>2. Observe dodge trajectory and landing point.<br>3. Confirm enemy is on solid ground.<br>4. Repeat 3 times. | Enemy lands on a valid, walkable surface after every dodge. | Not Executed |
| TC-008 | Enemy dodge near wall does not clip into geometry | Dodge-capable enemy positioned near a wall | 1. Position player to trigger enemy dodge toward the wall.<br>2. Observe dodge animation and landing position.<br>3. Confirm enemy position is outside wall geometry after landing. | Enemy is not embedded in wall geometry; enemy lands on the nearest valid surface. | Not Executed |
| TC-009 | Player collision with Phase 3 gear during normal traversal | Player in Phase 3; gear structures are active | 1. Navigate through Phase 3 near gear structures.<br>2. Move alongside gears without standing at the wall-contact point.<br>3. Observe collision behavior. | Gear pushes or stops player; no model overlap during normal traversal. | Not Executed |
| TC-010 | Player collision at gear-wall contact moment | Player in Phase 3 end section; gear in rotation cycle | 1. Identify the gear's wall-contact point.<br>2. Position player near that point.<br>3. Wait for gear to complete rotation and contact the wall.<br>4. Observe player behavior during contact. | Player is pushed away or blocked; player does not clip inside gear geometry. | Not Executed |
| TC-011 | Player can exit gear geometry if clipping occurs | BUG-004 condition triggered; player is inside gear | 1. Replicate BUG-004 conditions.<br>2. Attempt to move in all directions from inside the gear.<br>3. Observe whether player can exit or is expelled. | Collision resolves and expels player to the nearest valid surface. | Not Executed |
| TC-012 | Checkpoint activation stores area state | Player has not yet activated the checkpoint | 1. Navigate to checkpoint/safe point.<br>2. Activate checkpoint.<br>3. Note enemy and resource positions in the surrounding area.<br>4. Confirm activation feedback is displayed. | Checkpoint is activated; area state is recorded at this point. | Not Executed |
| TC-013 | Cleared enemies remain absent after returning through checkpoint | Checkpoint active; enemies in nearby area have been cleared | 1. Clear enemies in checkpoint area.<br>2. Activate checkpoint.<br>3. Progress forward to the next area.<br>4. Return through the checkpoint to the cleared area.<br>5. Observe enemy state. | Cleared enemies are not present; area state is preserved as of checkpoint activation. | Not Executed |
| TC-014 | Health items do not respawn after a single checkpoint cycle | Health items collected in an area; checkpoint active | 1. Collect all health items in an area.<br>2. Activate checkpoint.<br>3. Progress forward, then return to the area.<br>4. Observe health item state. | Health items do not respawn after one checkpoint cycle (see OBS-001). | Not Executed |
| TC-015 | Ammo and grenades do not respawn after a single checkpoint cycle | Ammo and grenades collected in an area; checkpoint active | 1. Collect all ammo and grenades in an area.<br>2. Activate checkpoint.<br>3. Progress forward, then return to the area.<br>4. Observe ammo and grenade state. | Ammo and grenades do not respawn after one checkpoint cycle (see OBS-001). | Not Executed |
