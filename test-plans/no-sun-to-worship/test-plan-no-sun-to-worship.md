# Test Plan — No Sun To Worship

| Field       | Details              |
| ----------- | -------------------- |
| Document ID | TP-002               |
| Game        | No Sun To Worship    |
| Author      | Brendo de Araujo     |
| Date        | [Fill in date]       |
| Version     | 1.0                  |

---

## 1. Objective

[Define the testing scope, approach, and coverage areas for No Sun To Worship. Describe the main systems to be validated and the purpose of this test plan.]

---

## 2. Scope

| System | Description |
| --- | --- |
| [System 1] | [Description of what will be tested] |
| [System 2] | [Description of what will be tested] |
| [System 3] | [Description of what will be tested] |
| [System 4] | [Description of what will be tested] |
| [System 5] | [Description of what will be tested] |

---

## 3. Out of Scope

- [System or feature not covered in this test plan]
- [System or feature not covered in this test plan]
- [System or feature not covered in this test plan]
- Any system or area not listed in Section 2

---

## 4. Risks

| Risk | Impact | Mitigation |
| --- | --- | --- |
| Single tester — no cross-validation | Findings may reflect individual play patterns | Retest confirmed defects across multiple sessions |
| Game version not confirmed | Results may not reflect current patch state | Confirm version before each test execution |
| [Additional risk] | [Impact] | [Mitigation] |

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
| Platform | [Fill in platform] |
| Operating System | [Fill in OS] |
| Input Method | [Fill in input method] |
| Game Version | [Fill in game version] |

---

## 7. Areas Under Test

| # | Area | System | Related Findings |
| --- | --- | --- | --- |
| 1 | [Area name] | [System being tested] | — |
| 2 | [Area name] | [System being tested] | — |
| 3 | [Area name] | [System being tested] | — |
| 4 | [Area name] | [System being tested] | — |
| 5 | [Area name] | [System being tested] | — |

---

## 8. Exit Criteria

- All test cases in `test-cases/no-sun-to-worship/gameplay-and-systems-test-cases.md` executed with results recorded
- All confirmed defects have video or screenshot evidence attached
- All design observations documented and pending validation items noted
- Session notes updated with final coverage summary and open items
