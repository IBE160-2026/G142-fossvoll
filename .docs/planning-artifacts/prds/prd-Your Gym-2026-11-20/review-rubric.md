# PRD Quality Review — RepRoute (self-review at finalize, 2026-11-21)

Walked by the facilitating agent against the rubric, not by an independent subagent.

## Overall verdict
Strong journey-led PRD that is coherent around one thesis: a game feel that never slows logging. Main weaknesses were vague testable conditions and a few unmeasurable success metrics. These were fixed in the finalize pass.

## Findings and resolution
- **high** SM-1 to SM-4 were not measurable. *Fixed:* rewritten as tester-based checks.
- **high** NFR-1 "never slows" had no bound. *Fixed:* 100 ms response (assumption).
- **medium** FR-4, FR-6, FR-19 used subjective wording. *Fixed:* testable conditions.
- **medium** FR-8 mixed AI and offline behaviour. *Fixed:* rules-based templates always work, AI is optional.
- **medium** Glossary gaps (Equipment, Week). *Fixed.*
- **medium** Brief items dropped: original avatar design, machine choice per Exercise, session feedback, goal raising. *Fixed or listed as deferred.*
- **low** XP amounts, Level thresholds, launch targets undefined. *Logged as open questions 8 and 9.*

## Mechanical notes
FR-1 to FR-22 contiguous. UJ-1 and UJ-2 have a named protagonist. Every inline `[ASSUMPTION]` is in the index in §9.
