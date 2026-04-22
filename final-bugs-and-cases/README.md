# Bug Cases — AI 100 Final Project
**Authors:** Jasraj "Jay" Raval & Jack Sweeney

Each file documents one intentional bug introduced into the ASL CNN system.
All 10 cases received a **❌ Bad** label from GenAI because every initial
self-reflection was too shallow — identifying symptoms without understanding
the root cause mechanism.

---

## Index

| File | Case | Student | Component | GenAI Label |
|---|---|---|---|---|
| [case_01_normalize_channels.md](case_01_normalize_channels.md) | 1 | Jasraj Raval | Preprocessing | ❌ Bad |
| [case_02_maxpool_kernel.md](case_02_maxpool_kernel.md) | 2 | Jack Sweeney | Architecture | ❌ Bad |
| [case_03_learning_rate.md](case_03_learning_rate.md) | 3 | Jasraj Raval | Training config | ❌ Bad |
| [case_04_dropout_p1.md](case_04_dropout_p1.md) | 4 | Jack Sweeney | Architecture | ❌ Bad |
| [case_05_crossentropy_args.md](case_05_crossentropy_args.md) | 5 | Jasraj Raval | Training loop | ❌ Bad |
| [case_06_fc_mismatch.md](case_06_fc_mismatch.md) | 6 | Jack Sweeney | Architecture | ❌ Bad |
| [case_07_epochs_zero.md](case_07_epochs_zero.md) | 7 | Jasraj Raval | Training config | ❌ Bad |
| [case_08_rotation_180.md](case_08_rotation_180.md) | 8 | Jack Sweeney | Preprocessing | ❌ Bad |
| [case_09_zero_grad.md](case_09_zero_grad.md) | 9 | Jasraj Raval | Training loop | ❌ Bad |
| [case_10_batch_size.md](case_10_batch_size.md) | 10 | Jack Sweeney | Training config | ❌ Bad |

---

## Failure Type Summary

| Failure Type | Cases | Danger |
|---|---|---|
| Runtime crash (explicit error) | 1, 2, 5, 6 | Low — forces immediate attention |
| Training instability (explosion / oscillation) | 3, 9 | Medium — visible but cause non-obvious |
| Silent failure (no error, wrong result) | 4, 7, 8, 10 | **High — outward appearance of success** |

---

## Each File Contains
- What was changed and why
- Original vs. buggy code side-by-side
- Exact error or observed behavior
- Initial self-reflection (shallow — all labeled Bad)
- GenAI Socratic guidance
- New self-reflection after guidance
- Root cause explanation
- Fix and lesson learned
