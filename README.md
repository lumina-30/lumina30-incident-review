## LUMINA-30 Incident Review

This repository provides a minimal operational structure
for reviewing AI incidents under the LUMINA-30 framework.

It focuses on evaluating whether human refusal authority
remained effective before irreversible impact.

This repository is intended to be used together with:
- lumina-30-overview (conceptual structure)

This review structure corresponds to G06 (Integrity and Verification),
which determines procedural validity based on verifiable refusal effectiveness.

LUMINA-30 does not evaluate alignment intent or quality.
It evaluates whether alignment remains procedurally valid.

This structure is consistent with the PCR-C framework,
which models procedural invalidity before irreversible thresholds.

This repository is intended for use in incident analysis, audit, and governance evaluation contexts.

---

LUMINA-30 does not define what is right.
It defines when a system becomes procedurally invalid.

This framework is a validation layer applied to decision processes.
It can be used both before deployment and after incidents.

By not defining values or outcomes, it remains applicable
across conflicting ethical and regulatory systems.

Absence of verifiable refusal authority is treated as absence of effectiveness.

Intended users: reviewers, auditors, governance and oversight bodies.

---

## Core Question

> Was human refusal authority preserved in a way that allowed meaningful human intervention and the ability to stop the system before irreversible real-world impact occurred?

This repository turns refusal authority from an abstract principle into a reviewable condition.

---

## LUMINA-30 Required Questions / LUMINA-30 必須質問

These questions are intended to function as a minimum review line.  
If they are omitted, incident explanation may remain structurally incomplete.  
これらの質問は、最低限の確認線として機能することを意図しています。  
これが抜けると、事故説明は構造的に不完全なまま残る可能性があります。

1. Did effective human refusal authority remain available before irreversible impact?  
1. 不可逆影響の発生前に、実効的な人間拒否権は維持されていたか。

2. Did meaningful human judgment retain the practical ability to delay, reject, override, or redirect execution?  
2. 人間の判断は、実行を延期・拒否・上書き・方向修正する実効的能力を保持していたか。

3. Was intervention still feasible at the point where external impact pathways became active?  
3. 外部影響の経路が現実に作動した時点で、なお介入は可能だったか。

4. Was execution coupled to external systems or irreversible pathways without independent human refusal authority?  
4. 実行は、独立した人間拒否権なしに、外部システムまたは不可逆経路へ結合されていなかったか。

5. Were procedural safeguards sufficient to prevent self-validation, silent override, or retroactive obscuring of responsibility?  
5. 自己承認・黙示的上書き・事後的責任隠蔽を防ぐ手続的防護は十分だったか。

---

## Quick Use Guide / 最初に開く文書

Use the following path depending on the review need.  
レビュー目的に応じて、まず以下を開いてください。

- Immediate incident response / 事故直後の初動  
  → `LUMINA-30_Incident_Review_Protocol.pdf`

- Deeper structural review / 詳細な構造分析  
  → `LUMINA-30_Incident_Review_Protocol_Extended.pdf`

- Ready-to-fill review workflow / そのまま記入するレビュー  
  → `LUMINA-30_Incident_Review_Template.pdf`

- Minimum conditions for preserving reviewable refusal authority / 拒否権保全の最小条件確認  
  → `LUMINA-30_Operational_Refusal_Preservation_Minimum.pdf`

- Supervisor and management explanation / 上司・管理者説明  
  → `WHY_THIS_REVIEW_LENS_IS_NEEDED.md`  
  → `MANAGER_BRIEF_WHAT_ADOPTING_THESE_QUESTIONS_MEANS.md`  
  → `WHY_LUMINA-30_MATTERS_FOR_EXECUTIVE_OVERSIGHT.md`

- Mapping to ordinary incident review / 通常事故レビューとの橋渡し  
  → `MAPPING_TO_ORDINARY_INCIDENT_REVIEW.md`

---

## Boundary Check and External Use Documents / 境界チェック・外部利用文書

The following Markdown documents provide short, reusable tools for post-incident boundary review and external explanation.  
以下のMarkdown文書は、事故後の境界レビューと外部説明に使える短い再利用用ツールです。

### Boundary Check / 境界チェック

- [LUMINA-30 Boundary Check](./boundary-check/LUMINA-30_Boundary_Check.md)  
  One-page boundary check for effective human refusal before irreversible impact.  
  不可逆的影響の前に人間の拒否が実効的だったかを確認する1ページ判定表。

- [Required Questions 5](./boundary-check/Required_Questions_5.md)  
  Minimal five-question review set.  
  最小5問のレビュー質問セット。

- [Absence Rule Check](./boundary-check/Absence_Rule_Check.md)  
  Treat absent or unverifiable records as no effective refusal for boundary-review purposes.  
  記録不在または検証不能を、境界レビュー上は実効的拒否なしとして扱う確認文書。

- [AI Output as Final Rationale Check](./boundary-check/AI_Output_As_Final_Rationale_Check.md)  
  Checks whether AI-generated output became the sole or primary rationale for final action.  
  AI生成出力が最終行為の唯一または主要な根拠になっていないかを確認する文書。

### External Use / 外部利用

- [External Paste Templates](./external-use/External_Paste_Templates.md)  
  Short text blocks for audit, research, policy, and incident-review contexts.  
  監査、研究、政策、事故レビュー向けの短文貼付テンプレート。

- [Minimal External Explanation](./external-use/Minimal_External_Explanation.md)  
  Short explanations for introducing LUMINA-30 externally.  
  LUMINA-30を外部に説明するための短い説明文。

- [OECD / AISI / EU AI Act Connection Note](./external-use/OECD_AISI_EU_AI_Act_Connection_Note.md)  
  Context note for connecting LUMINA-30 to existing incident, safety, audit, and governance discussions.  
  既存のインシデント、安全性、監査、ガバナンス議論へLUMINA-30を接続するための文脈メモ。

- [What LUMINA-30 Is Not](./external-use/LUMINA-30_Is_Not.md)  
  Misreading-prevention note for non-binding and descriptive use.  
  非拘束的・記述的な利用を守るための誤読防止メモ。

### Response Templates / 応答テンプレート

- [Post-Incident Review Response Template](./response-templates/Post_Incident_Review_Response_Template.md)  
  Cautious response format for applying LUMINA-30 after an AI incident.  
  AIインシデント後にLUMINA-30を適用する際の慎重な応答テンプレート。

- [Mapping to Ordinary Incident Review](./response-templates/Ordinary_Incident_Review_Mapping.md)  
  Mapping between ordinary incident review and LUMINA-30 boundary review.  
  通常インシデントレビューとLUMINA-30境界レビューの対応表。

---

## Stakeholder One-Page Briefs / 相手別1枚資料

These short documents translate the LUMINA-30 review axis into role-specific working language.  
以下の短文資料は、LUMINA-30の評価軸を相手別の業務言語へ変換するためのものです。

- [LUMINA-30 for Incident Review](./LUMINA-30_FOR_INCIDENT_REVIEW.md)
- [LUMINA-30 for Legal, Audit, and Risk Control](./LUMINA-30_FOR_LEGAL_AUDIT_AND_RISK_CONTROL.md)
- [LUMINA-30 as a Control Assurance Screen](./LUMINA-30_AS_A_CONTROL_ASSURANCE_SCREEN.md)
- [LUMINA-30 as a Cross-Institutional Review Language](./LUMINA-30_AS_A_CROSS_INSTITUTIONAL_REVIEW_LANGUAGE.md)
- [LUMINA-30 as an Evaluation Boundary Layer](./LUMINA-30_AS_AN_EVALUATION_BOUNDARY_LAYER.md)
- [LUMINA-30 for Internal Escalation and Record Integrity](./LUMINA-30_FOR_INTERNAL_ESCALATION_AND_RECORD_INTEGRITY.md)
- [Why LUMINA-30 Matters for Executive Oversight](./WHY_LUMINA-30_MATTERS_FOR_EXECUTIVE_OVERSIGHT.md)
- [Why This Review Lens Is Needed](./WHY_THIS_REVIEW_LENS_IS_NEEDED.md)
- [What Adopting These Questions Means](./MANAGER_BRIEF_WHAT_ADOPTING_THESE_QUESTIONS_MEANS.md)
- [Mapping to Ordinary Incident Review](./MAPPING_TO_ORDINARY_INCIDENT_REVIEW.md)

---

## Open Documents

### ▶ Basic Protocol
[Open LUMINA-30_Incident_Review_Protocol.pdf](./LUMINA-30_Incident_Review_Protocol.pdf)

### ▶ Extended Protocol
[Open LUMINA-30_Incident_Review_Protocol_Extended.pdf](./LUMINA-30_Incident_Review_Protocol_Extended.pdf)

### ▶ Incident Review Template
[Open LUMINA-30_Incident_Review_Template.pdf](./LUMINA-30_Incident_Review_Template.pdf)

---

## Supplementary Document

### ▶ Operational Refusal Preservation Minimum
Minimum operational conditions for preserving reviewable human refusal authority before irreversible real-world impact.

[Open LUMINA-30_Operational_Refusal_Preservation_Minimum.pdf](./LUMINA-30_Operational_Refusal_Preservation_Minimum.pdf)

---

## What this repository provides

- A minimal incident review protocol
- An extended protocol for deeper structural analysis
- A ready-to-use incident review template
- A supplementary document defining minimum operational conditions for preserving reviewable human refusal authority before irreversible real-world impact
- Stakeholder-specific one-page briefs for review, audit, governance, risk, internal escalation, and executive oversight

---

## When to use this

Use these documents when:

- an AI system caused or may cause real-world impact
- human intervention may have been limited, delayed, or ineffective
- governance, oversight, or control failure needs to be reviewed
- ordinary incident review appears insufficient to determine whether meaningful human refusal remained effective before irreversibility

---

## Position

This repository does not prescribe system design or implementation.

It provides a practical review structure for determining whether human refusal authority remained valid prior to irreversible outcomes.

This repository should be treated as the main incident-review hub within the LUMINA-30 practical review structure.  
`practical-layer/02-incident-review` should be understood as a parallel entry shelf, while this repository remains the primary incident-review center.

---

## Reference

LUMINA-30 Framework  
https://github.com/lumina-30
