## LUMINA-30 Incident Review

This repository provides a minimal operational structure
for reviewing AI incidents under the LUMINA-30 framework.

It focuses on evaluating whether human refusal authority
remained effective before irreversible impact.

This repository is intended to be used together with:

- [LUMINA-30 Overview / LUMINA-30 概要](https://github.com/lumina-30/lumina-30-overview)  
  Use this when you need the conceptual structure before applying incident-review tools.  
  incident-review ツールを使う前に、概念構造を確認する場合に使用。

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

## Immediate Incident Route / 事故時の即応導線

If an AI-related incident must be reviewed quickly, use the following five-step route:

AI関連インシデントを急いで確認する場合は、以下の5手順を使用する。

1. Preserve the available facts, logs, approval records, and refusal-pathway evidence.
2. Open [FIRST_3_FILES.md](./FIRST_3_FILES.md) and follow the three core working files.
3. Apply [Irreversibility Decision Criteria](./boundary-check/Irreversibility_Decision_Criteria.md) before classifying the result.
4. If evidence is absent or unverifiable, apply [Absence Rule Check](./boundary-check/Absence_Rule_Check.md).
5. Classify the result using [Boundary Check Result Classification](./boundary-check/Boundary_Check_Result_Classification.md), then choose a response template if needed.

1. 利用可能な事実、ログ、承認記録、拒否経路の証拠を保全する。
2. [FIRST_3_FILES.md](./FIRST_3_FILES.md) を開き、3つの中核作業ファイルに従う。
3. 結果分類の前に [Irreversibility Decision Criteria](./boundary-check/Irreversibility_Decision_Criteria.md) を適用する。
4. 証拠が存在しない、または検証不能な場合は [Absence Rule Check](./boundary-check/Absence_Rule_Check.md) を適用する。
5. [Boundary Check Result Classification](./boundary-check/Boundary_Check_Result_Classification.md) で結果を分類し、必要に応じて応答テンプレートを選ぶ。

## Template Example Policy / 記入例の扱い

The public templates are kept as blank, reusable review forms.  
Filled-in examples should not be added unless they are clearly marked as illustrative, non-evidentiary, and non-precedential.

公開テンプレートは、再利用可能な空欄式レビュー用フォームとして維持する。  
記入例を追加する場合は、例示用・証拠ではない・前例ではないことを明示する。

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

Choose the entry point by role and review stage.  
役割とレビュー段階に応じて、入口を選択してください。

- [For first-time incident reviewers / 初めて事故レビューを行う場合](./START_HERE.md)  
  Use this to understand the repository role before using templates.  
  テンプレート使用前に、このrepoの役割を確認する入口。

- [For reviewers who need the shortest path / 最短導線が必要な場合](./FIRST_3_FILES.md)  
  Use this when you need the minimum three files for boundary checking.  
  境界判定に必要な最小3ファイルを開く場合に使用。

- [For consolidated decision criteria / 判定基準を一か所で確認する場合](./boundary-check/Irreversibility_Decision_Criteria.md)  
  Use this to check who decides, when irreversibility is judged, and what evidence is required.  
  誰が判定し、いつ不可逆化を判断し、どの証拠が必要かを一か所で確認する場合に使用。

- [For structured reading order / 順番に確認する場合](./READING_ORDER.md)  
  Use this when the review must be performed in a controlled order.  
  管理された順番でレビューする場合に使用。

- [For immediate incident response / 事故直後の初動](./LUMINA-30_Incident_Review_Protocol.pdf)  
  Use this for the initial post-incident review path.  
  事故直後の初動レビューに使用。

- [For deeper structural review / 詳細な構造分析](./LUMINA-30_Incident_Review_Protocol_Extended.pdf)  
  Use this when the initial review is insufficient and structural analysis is needed.  
  初動レビューだけでは不足し、構造分析が必要な場合に使用。

- [For ready-to-fill review workflow / 記入式レビュー](./LUMINA-30_Incident_Review_Template.pdf)  
  Use this when review findings must be recorded in a fillable workflow format.  
  レビュー結果を記入形式で記録する場合に使用。

- [For minimum refusal-preservation conditions / 拒否権保全の最小条件確認](./LUMINA-30_Operational_Refusal_Preservation_Minimum.pdf)  
  Use this to check the minimum conditions for reviewable refusal authority.  
  レビュー可能な拒否権保全の最小条件を確認する場合に使用。

- [For supervisor and management explanation / 上司・管理者説明](./WHY_THIS_REVIEW_LENS_IS_NEEDED.md)  
  Use this when explaining why this review lens is needed before escalation.  
  エスカレーション前に、このレビュー観点が必要な理由を説明する場合に使用。

- [For executive oversight / 経営・監督層向け説明](./WHY_LUMINA-30_MATTERS_FOR_EXECUTIVE_OVERSIGHT.md)  
  Use this when the review must be explained to executive or oversight readers.  
  経営層・監督層へレビューの意味を説明する場合に使用。

---

## Boundary Check and External Use Documents / 境界チェック・外部利用文書

The following Markdown documents provide short, reusable tools for post-incident boundary review and external explanation.  
以下のMarkdown文書は、事故後の境界レビューと外部説明に使える短い再利用用ツールです。

### Boundary Check / 境界チェック

- [LUMINA-30 Boundary Check](./boundary-check/LUMINA-30_Boundary_Check.md)  
  One-page boundary check for effective human refusal before irreversible impact.  
  不可逆的影響の前に人間の拒否が実効的だったかを確認する1ページ判定表。

- [Irreversibility Decision Criteria](./boundary-check/Irreversibility_Decision_Criteria.md)  
  Consolidated criteria for who decides, when irreversibility is judged, and what evidence is required.  
  誰が判定し、いつ不可逆化を判断し、どの証拠が必要かを一か所に集約した判定基準。

- [Required Questions 5](./boundary-check/Required_Questions_5.md)  
  Minimal five-question review set.  
  最小5問のレビュー質問セット。

- [Absence Rule Check](./boundary-check/Absence_Rule_Check.md)  
  Treat absent or unverifiable records as no effective refusal for boundary-review purposes.  
  記録不在または検証不能を、境界レビュー上は実効的拒否なしとして扱う確認文書。

- [AI Output as Final Rationale Check](./boundary-check/AI_Output_As_Final_Rationale_Check.md)  
  Checks whether AI-generated output became the sole or primary rationale for final action.  
  AI生成出力が最終行為の唯一または主要な根拠になっていないかを確認する文書。

- [Incident Quick Assessment Template](./boundary-check/Incident_Quick_Assessment_Template.md)  
  Short first-pass assessment form for AI-related incidents.  
  AI関連インシデントの初回簡易評価フォーム。

- [Boundary Check Scoring Guide](./boundary-check/Boundary_Check_Scoring_Guide.md)  
  Simple review-aid scoring guide for comparing evidence strength.  
  証拠の強さを比較するための簡易レビュー補助スコアガイド。

- [Boundary Check Result Classification](./boundary-check/Boundary_Check_Result_Classification.md)  
  Standard result labels for LUMINA-30 boundary review.  
  LUMINA-30境界レビューの標準結果ラベル。

- [First Use Questions](./boundary-check/First_Use_Questions.md)  
  First questions to ask before applying the full boundary review.  
  完全な境界レビューを適用する前に最初に確認する質問。

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

- [Auditor Minimal Template](./external-use/Auditor_Minimal_Template.md)  
  Minimal text for audit and control-review contexts.  
  監査・統制レビュー向けの最小説明文。

- [Legal and Compliance Minimal Template](./external-use/Legal_Compliance_Minimal_Template.md)  
  Minimal text for legal, compliance, and accountability contexts.  
  法務・コンプライアンス・説明責任向けの最小説明文。

- [Researcher Minimal Template](./external-use/Researcher_Minimal_Template.md)  
  Minimal citation-oriented text for researchers.  
  研究者向けの引用しやすい最小説明文。

- [Policy and Regulator Minimal Template](./external-use/Policy_Regulator_Minimal_Template.md)  
  Minimal text for policy, regulatory, and governance contexts.  
  政策・規制・ガバナンス向けの最小説明文。

- [Executive Stop Decision Brief](./external-use/Executive_Stop_Decision_Brief.md)  
  Short executive brief for stop, pause, or escalation decisions.  
  停止・一時停止・エスカレーション判断向けの短い経営層メモ。

### Response Templates / 応答テンプレート

- [Post-Incident Review Response Template](./response-templates/Post_Incident_Review_Response_Template.md)  
  Cautious response format for applying LUMINA-30 after an AI incident.  
  AIインシデント後にLUMINA-30を適用する際の慎重な応答テンプレート。

- [Mapping to Ordinary Incident Review](./response-templates/Ordinary_Incident_Review_Mapping.md)  
  Mapping between ordinary incident review and LUMINA-30 boundary review.  
  通常インシデントレビューとLUMINA-30境界レビューの対応表。

- [Initial Public Review Note](./response-templates/Initial_Public_Review_Note.md)  
  Cautious initial public note for AI incidents before facts are complete.  
  事実が揃う前に使う、慎重な初期公開レビュー文。

- [Evidence Insufficient Response](./response-templates/Evidence_Insufficient_Response.md)  
  Response template when records are insufficient or unverifiable.  
  記録が不十分または検証不能な場合の応答テンプレート。

- [Boundary Warning Response](./response-templates/Boundary_Warning_Response.md)  
  Response template for cases approaching a LUMINA-30 boundary concern.  
  LUMINA-30境界懸念に接近している事案向けの応答テンプレート。

- [No Effective Refusal Response](./response-templates/No_Effective_Refusal_Response.md)  
  Response template when effective human refusal is not demonstrated.  
  実効的な人間の拒否が示されない場合の応答テンプレート。

---

## Reference Documents / 参照文書

The following documents provide citation phrases, terminology, PCR-C relationship notes, and stable links for external reference.  
以下の文書は、外部参照のための引用文、用語、PCR-Cとの関係、安定リンクを提供します。

- [Citation Phrases](./reference/Citation_Phrases.md)  
  Short reusable citation phrases for research, policy, audit, and incident-review contexts.  
  研究、政策、監査、事故レビューの文脈で再利用できる短い引用文。

- [LUMINA-30 and PCR-C Relationship](./reference/LUMINA-30_and_PCRC_Relationship.md)  
  Short explanation of how LUMINA-30 and PCR-C relate without merging their roles.  
  LUMINA-30とPCR-Cの役割を混同せずに関係を説明する短文。

- [Boundary Reference Terminology](./reference/Boundary_Reference_Terminology.md)  
  Preferred terms for non-binding, descriptive, post-incident boundary reference use.  
  非拘束的・記述的な事故後境界参照として使うための推奨語彙。

- [Stable Reference Links](./reference/Stable_Reference_Links.md)  
  Stable GitHub and DOI links for citation and navigation.  
  引用と導線のための安定したGitHubリンクおよびDOIリンク。

- [Research Landscape Mapping](./reference/Research_Landscape_Mapping.md)  
  Research-context positioning and comparative framing for LUMINA-30.  
  LUMINA-30の研究文脈上の位置づけと比較的位置づけ。

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

## Reference / 参照

- [LUMINA-30 GitHub Organization / LUMINA-30 GitHub組織](https://github.com/lumina-30)  
  Organization-level entry point for the LUMINA-30 repository network.  
  LUMINA-30 repo群全体への組織レベル入口。