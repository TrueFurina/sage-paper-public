# SAGE — agent-facing working set

This repository is a **curated subset** of a SAGE manuscript workspace, published so that an
autonomous research agent can read and work on the project. It contains the paper-facing material
only: section drafts, source materials the drafts derive from, the simulation code, and the
reference-verification archive.

## What this paper is

**Title:** *When Does Guidance Still Help? Separating Scaffolding Effects from Answer-Leakage Effects
in Graduate Cryptography Instruction — A Simulation Study*

**Form:** a **fully simulated** methodology study. There are **no human participants, no classroom,
and no student data**. The graduate cryptography curriculum is the *application scenario*; it is not
a data-collection site. Nothing in this repository supports any claim about learners.

**Target journal:** *Frontiers of Education in China* (FEDC).

## Contents

| File | Role |
|---|---|
| `23_Abstract_en.md` | Abstract (target 100–120 words) + clause-by-clause mapping table (internal) |
| `07_Introduction动机链_原文证据锚定.md` | §1 Introduction draft (English) + **per-claim source-anchoring table** (internal) |
| `13_Section2_Literature_Review_en.md` | §2 Literature Review draft |
| `01_theoretical_framework_en.md` | §3 Theoretical Framework draft (information bottleneck; boundary vs gradient) |
| `21_Section4_System_Design_en.md` | §4 System Design draft (five agents; the scaffolding ladder) |
| `17_Section5_Method_en.md` | §5 Method draft (simulated cohort; four arms) |
| `15_Section6_Results_en.md` | §6 Results draft (simulation results only) |
| `22_Section7_Discussion_en.md` | §7 Discussion draft |
| `14_Section8_Limitations_en.md` | §8 Limitations draft |
| `24_Section9_Conclusion_en.md` | §9 Conclusion draft |
| `28_AppendixABC_en.md` | Appendices A–C (bottleneck derivation; ladder + prompt templates; item bank + coding manual) |
| `25_AppendixE_Bilingual_References.md` | **Reference verification archive** — per-entry verification status, cross-library checks, and the bilingual-annotation examples FEDC requires |
| `05_论文大纲.md` | Outline / section targets |
| `02_系统架构与交互协议.md` | Chinese design specification that §4 and Appendix B derive from |
| `19_密码学知识图谱骨架.md` | Cryptography knowledge graph (46 nodes, ≈45 prerequisite edges) — **v0.1, not yet specialist-verified** |
| `20_密码学题库与测量.md` | Item bank framework and *Telling@N* coding manual |
| `m2_lambda_sweep.py` | The simulation that produces every number in §6 |
| `data/README.md` | Where each reported number comes from |
| `README.md` | Index of the full (private) workspace |
| `30_ClawsGO科研提示词包.md` | Our internal prompt pack for driving an agent on this project — includes the project's wording red lines and verification/acceptance clauses. **Agents should read this before acting.** |

## Ground rules an agent must follow here

1. **No fabricated metadata.** Reference fields that have not been verified are marked `[待核]`.
   Never fill them in from memory. If a field cannot be verified, leave it marked.
2. **A digit is a single source of truth.** Reported quantities are in *threshold* form
   (λ\* = 0.30, interval [0.20, 0.45]; earned-solve peak 0.5659; attributable share 86%, sensitivity
   76–88%; control arm +0.0594; full intervention +0.4380; instructive-leak mutant ≈43%).
   Superseded *continuous*-form values (0.35 / 0.5204 / 85%) must not appear anywhere.
3. **Cite only to the strength of what is held.** If a source's full text has not been obtained,
   any sentence about it carries a qualifier ("as described in the published abstract").
4. **No primacy claims.** Do not write "the first", "no existing work", or "no one has".
5. **No classroom implication.** Never write as though data came from students.
6. Numbers in §6 are **properties of the apparatus under a stipulated learner model**, computed by
   `m2_lambda_sweep.py`; they are not measurements of learning.

## What is deliberately not here

Internal decision records, project memory, audit trails and private notes are held in the private
workspace and are not published. Several drafts reference those files by number (e.g. "see `09`");
those references are internal and can be ignored for the purpose of working on the manuscript text.
