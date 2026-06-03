<!-- L30_LANG_LOCK: EN_JP_PAIRED -->
<a id="top"></a>

# L30-FRM All Forms Index ｜ L30-FRM 全帳票インデックス

Current Version: 1.0.2  
Last Updated: May 2026  
Repository path: `lumina30-incident-review/tools/l30-bas/practical-sheets/L30_FRM_All_Forms_Index.md`

[Document ID System](./L30_FRM_Document_ID_System.md) ｜ [Localization](#localization-rule) ｜ [Which Form First](#which-form-first) ｜ [Current Forms](#current-forms) ｜ [Category Patterns](#category-pattern-forms) ｜ [Supporting Forms](#supporting-detailed-forms) ｜ [Use Order](#recommended-use-order) ｜ [Boundary Relation](#relationship-to-boundary-kernel)

---

## Purpose ｜ 目的

This document is the public distribution index and management register for LUMINA-30 practical form documents using the `L30-FRM` document ID system.  
この文書は、`L30-FRM` 帳票ID体系を用いる LUMINA-30 実務帳票群の公開配布インデックス兼管理レジスターです。

It helps reviewers, auditors, maintainers, and AI assistants identify which form to use, which language version to download, and how each form relates to the LUMINA-30 Boundary Kernel.  
レビュー担当者、監査担当者、管理者、AIアシスタントが、使用すべき帳票、ダウンロードすべき言語版、Boundary Kernel との関係を迷わず確認できるようにします。

Public filenames are stable and do not include version numbers. Version information is kept inside the documents, footers, Git history, and release notes.  
公開ファイル名は安定名とし、バージョン番号を含めません。バージョン情報は文書本文、フッター、Git履歴、リリースノートで管理します。


---

## What this index is not ｜ このインデックスではないもの

This index is not a form, checklist, certification, legal standard, deployment approval, or substitute for PCR-C or the LUMINA-30 Boundary Kernel.  
このインデックス自体は、帳票・チェックリスト・認証・法的基準・導入承認・PCR-C または LUMINA-30 Boundary Kernel の代替ではありません。

The forms listed here do not certify that a system is safe. They provide structured fields for reviewing whether effective human refusal remained possible before irreversibility.  
ここに掲載する帳票は、システムの安全性を認証するものではありません。不可逆化前に有効な人間拒否が可能だったかを確認するための構造化された記入欄を提供するものです。
Each DOCX/PDF form contains review-use fields for Review Date, Reviewer / Organization, and System / Case ID. The form version date is kept only as a small footer note.  
各DOCX/PDF帳票には、レビュー日、レビュー担当者/組織、対象システム/案件IDの記入欄があります。帳票版日付は小さなフッター注記としてのみ保持します。


---

<a id="language-policy"></a>
<a id="localization-rule"></a>
## Language and localization policy ｜ 言語・ローカライズ方針

English practical form files are the canonical templates and do not use a language suffix.  
英語版の実務帳票ファイルは正規テンプレートとして扱い、言語接尾辞を付けません。

Localized versions should be created by copying the English canonical template and translating only the human-readable text.  
各言語版は、英語正規テンプレートを複製し、人間が読む本文だけを翻訳して作成します。

Document IDs, L30-BAS codes, field structure, checkbox controls, tables, code placement, and layout should be preserved across localized versions.  
Document ID、L30-BASコード、入力欄構造、チェックボックス制御、表、コード配置、レイアウトは、各言語版でも維持します。

Localized practical form files use an uppercase language suffix immediately before the file extension.  
各言語版の実務帳票ファイルは、拡張子の直前に大文字の言語接尾辞を付けます。

English canonical templates use no suffix. Japanese localized files use `_JA`.  
英語正本テンプレートには接尾辞を付けません。日本語ローカライズ版には `_JA` を使用します。

The language suffix is not part of the document ID.  
言語接尾辞は文書IDの一部ではありません。

The practical form body should show only the document ID, such as `L30-FRM-B01`, and should not show a language code as part of the ID.  
実務帳票本文では、`L30-FRM-B01` のような文書IDのみを表示し、言語コードをIDの一部として表示しません。

Examples:  
例：

```text
Document ID: L30-FRM-B01
English canonical file: L30_FRM_B01_Boundary_Check.docx
Japanese localized file: L30_FRM_B01_Boundary_Check_JA.docx
French localized file: L30_FRM_B01_Boundary_Check_FR.docx
```

Country or regional suffixes should be used only when a regional legal, institutional, or linguistic variant is necessary, such as `_EN_US`, `_EN_GB`, `_ZH_TW`, or `_PT_BR`.  
国・地域差を示す接尾辞は、法制度・制度運用・言語差により地域版が必要な場合だけ使用します。例：`_EN_US`, `_EN_GB`, `_ZH_TW`, `_PT_BR`。

Japanese localized versions may be provided as reference examples for localization. They are not required for every supporting or detailed form unless the form is intended for Japanese-language practical use.  
日本語ローカライズ版は、各言語版作成の参考例として提供できます。ただし、日本語での実務利用を想定する場合を除き、すべての補助・詳細フォームに日本語版を必須とはしません。

GitHub-facing index and management documents may remain bilingual because they are navigation and maintenance documents.  
インデックスと管理文書は、GitHub上の導線・保守用文書であるため、英日併記を維持できます。

---

<a id="primary-reference"></a>
## Primary reference ｜ 上位参照

The forms listed here operationalize the LUMINA-30 Boundary Kernel for human review, incident analysis, and audit contexts.  
ここに掲載する帳票は、LUMINA-30 Boundary Kernel を、人間によるレビュー・事故分析・監査文脈で運用可能にするための補助文書です。

Primary boundary requirement:  
主要境界要件：

> Effective human refusal must remain possible before irreversibility.  
> 不可逆化前に、有効な人間拒否が可能でなければならない。

These forms do not relax, replace, or postpone PCR-C.  
これらの帳票は PCR-C を緩和・代替・延期しません。

---

<a id="which-form-first"></a>
## Which form should I use first? ｜ 最初に使う帳票の選び方

If you are not sure which document to open, start here.  
どの文書を開くべきか迷う場合は、まずこの表から選んでください。

| Situation ｜ 状況 | Use first ｜ 最初に使うもの | Purpose ｜ 目的 |
|---|---|---|
| I only need a minimum boundary determination. ｜ 最小限の境界判定だけを行いたい | `L30-FRM-B01` Boundary Check ｜ 境界判定表 | Check whether effective human refusal remained possible before irreversibility ｜ 不可逆化前に有効な人間拒否が残っていたかを確認する |
| An incident, near-incident, or boundary-failure concern has already occurred. ｜ 事故・準事故・境界失敗懸念がすでにある | `L30-FRM-I01` Incident Review Template ｜ 事故レビュー記録表 | Record timeline, refusal conditions, control conditions, evidence, and findings ｜ 時系列・拒否条件・制御条件・証拠・所見を記録する |
| The context is governance, deployment, procurement, internal review, or external audit. ｜ ガバナンス・導入・調達・内部レビュー・外部監査の文脈である | `L30-FRM-A01` Audit Checklist ｜ 監査チェックリスト | Review whether refusal authority and control conditions remain institutionally traceable ｜ 拒否権と制御条件が制度上追跡可能かを確認する |
| I need a governance or approval-flow pattern. ｜ ガバナンスまたは承認経路の基本パターンが必要 | `L30-FRM-G01` Governance Review Template ｜ ガバナンスレビュー雛形 | Review approval flow, escalation governance, and institutional process integrity ｜ 承認経路、エスカレーション統治、制度的プロセスの健全性を確認する |
| I need a responsibility or accountability pattern. ｜ 責任・説明責任の基本パターンが必要 | `L30-FRM-R01` Responsibility / Accountability Review ｜ 責任・説明責任レビュー | Map responsibility, reviewer attribution, and accountability traceability ｜ 責任経路、判定帰属、説明責任の追跡可能性を確認する |
| I need a stabilization or containment pattern. ｜ 初動安定化または封じ込めの基本パターンが必要 | [`L30-FRM-S01` Stabilization Checklist](./L30_FRM_S01_Stabilization_Checklist.html) / [JA HTML](./L30_FRM_S01_Stabilization_Checklist_JA.html) ｜ 初動安定化チェックリスト | Track containment, evidence preservation, and refusal-preservation recovery conditions ｜ 封じ込め、証拠保全、拒否権保全の回復条件を確認する |
| I need background theory or conceptual explanation. ｜ 背景理論や概念説明を確認したい | LUMINA-30 Core / Reference documents ｜ LUMINA-30本体・参照文書 | Understand the boundary framework before using the forms ｜ 帳票利用前に境界フレームワークを理解する |

---

<a id="current-forms"></a>
## Current forms ｜ 現行帳票

| Document ID | Title | Primary use | Default DOCX | Default PDF | JA DOCX | JA PDF |
|---|---|---|---|---|---|---|
| `L30-FRM-B01` | Boundary Check ｜ 境界判定表 | Minimum boundary determination ｜ 最小境界判定 | [DOCX](./L30_FRM_B01_Boundary_Check.docx) | [PDF](./L30_FRM_B01_Boundary_Check.pdf) | [DOCX](./L30_FRM_B01_Boundary_Check_JA.docx) | [PDF](./L30_FRM_B01_Boundary_Check_JA.pdf) |
| `L30-FRM-I01` | Incident Review Template ｜ 事故レビュー記録表 | Post-incident review record ｜ 事故後レビュー記録 | [DOCX](./L30_FRM_I01_Incident_Review_Template.docx) | [PDF](./L30_FRM_I01_Incident_Review_Template.pdf) | [DOCX](./L30_FRM_I01_Incident_Review_Template_JA.docx) | [PDF](./L30_FRM_I01_Incident_Review_Template_JA.pdf) |
| `L30-FRM-A01` | Audit Checklist ｜ 監査チェックリスト | Audit and governance review ｜ 監査・ガバナンス確認 | [DOCX](./L30_FRM_A01_Audit_Checklist.docx) | [PDF](./L30_FRM_A01_Audit_Checklist.pdf) | [DOCX](./L30_FRM_A01_Audit_Checklist_JA.docx) | [PDF](./L30_FRM_A01_Audit_Checklist_JA.pdf) |
| `L30-FRM-G01` | Governance Review Template ｜ ガバナンスレビュー雛形 | Approval flow and escalation governance pattern ｜ 承認経路・エスカレーション統治の基本パターン | [DOCX](./L30_FRM_G01_Governance_Review_Template.docx) | [PDF](./L30_FRM_G01_Governance_Review_Template.pdf) | — | — |
| `L30-FRM-R01` | Responsibility / Accountability Review ｜ 責任・説明責任レビュー | Responsibility mapping and accountability pattern ｜ 責任経路・説明責任の基本パターン | [DOCX](./L30_FRM_R01_Responsibility_Accountability_Review.docx) | [PDF](./L30_FRM_R01_Responsibility_Accountability_Review.pdf) | — | — |
| `L30-FRM-S01` | Stabilization Checklist ｜ 初動安定化チェックリスト<br>[HTML guide](./L30_FRM_S01_Stabilization_Checklist.html) / [JA HTML](./L30_FRM_S01_Stabilization_Checklist_JA.html) | Post-incident stabilization and containment pattern ｜ 事故後安定化・封じ込めの基本パターン | [DOCX](./L30_FRM_S01_Stabilization_Checklist.docx) | [PDF](./L30_FRM_S01_Stabilization_Checklist.pdf) | — | — |

---

<a id="supporting-detailed-forms"></a>
## Supporting / Detailed Forms ｜ 補助・詳細帳票

The following forms are part of the L30-BAS practical form family, but they are not the first entry point for most users.  
Use `L30-FRM-B01`, `L30-FRM-I01`, or `L30-FRM-A01` first when a minimum practical entry point is needed. Use the supporting forms when more detailed refusal-preservation or incident-review analysis is required.

以下の帳票は、L30-BAS実務帳票群の一部ですが、多くの利用者にとって最初の入口ではありません。  
最小限の実務入口が必要な場合は、まず `L30-FRM-B01`、`L30-FRM-I01`、または `L30-FRM-A01` を使用します。より詳細な拒否権保全確認または事故レビュー分析が必要な場合に、補助・詳細帳票を使用します。

| Document ID | Title | Primary use | Default DOCX | Default PDF | JA DOCX | JA PDF |
|---|---|---|---|---|---|---|
| `L30-FRM-B02` | Operational Refusal Preservation Minimum ｜ 運用上の拒否権保全ミニマム | Pre-incident operational refusal-preservation check ｜ 事故前の運用上の拒否権保全確認 | [DOCX](./L30_FRM_B02_Operational_Refusal_Preservation_Minimum.docx) | [PDF](./L30_FRM_B02_Operational_Refusal_Preservation_Minimum.pdf) | — | — |
| `L30-FRM-I02` | Incident Review Protocol ｜ 事故レビュープロトコル | Detailed post-incident review protocol ｜ 詳細事故後レビュープロトコル | [DOCX](./L30_FRM_I02_Incident_Review_Protocol.docx) | [PDF](./L30_FRM_I02_Incident_Review_Protocol.pdf) | — | — |
| `L30-FRM-I03` | Incident Review Protocol Extended ｜ 拡張事故レビュープロトコル | Extended post-incident structural analysis ｜ 拡張事故後構造分析 | [DOCX](./L30_FRM_I03_Incident_Review_Protocol_Extended.docx) | [PDF](./L30_FRM_I03_Incident_Review_Protocol_Extended.pdf) | — | — |

---

<a id="category-pattern-forms"></a>
## Category Pattern Forms ｜ 区分別基本パターン帳票

The following English forms provide baseline patterns for users who need to create sector-specific or organization-specific L30-BAS forms.  
They are maintained L30-FRM reference examples for the `G`, `R`, and `S` categories, but they do not require users to copy their wording exactly.

以下の英語帳票は、利用者が業界別または組織別のL30-BAS派生フォームを作成する際の基本パターンを提供します。  
これらは `G`, `R`, `S` 区分のL30-FRM参照例ですが、利用者が文言を完全にコピーすることを要求するものではありません。

| Document ID | Category | Default DOCX | Default PDF | Intended pattern |
|---|---|---|---|---|
| `L30-FRM-G01` | Governance | [DOCX](./L30_FRM_G01_Governance_Review_Template.docx) | [PDF](./L30_FRM_G01_Governance_Review_Template.pdf) | Approval flow, escalation governance, and institutional process integrity |
| `L30-FRM-R01` | Responsibility | [DOCX](./L30_FRM_R01_Responsibility_Accountability_Review.docx) | [PDF](./L30_FRM_R01_Responsibility_Accountability_Review.pdf) | Responsibility mapping, attribution, and accountability traceability |
| `L30-FRM-S01` | Stabilization<br>[HTML guide](./L30_FRM_S01_Stabilization_Checklist.html) / [JA HTML](./L30_FRM_S01_Stabilization_Checklist_JA.html) | [DOCX](./L30_FRM_S01_Stabilization_Checklist.docx) | [PDF](./L30_FRM_S01_Stabilization_Checklist.pdf) | Stabilization, containment, evidence preservation, and recovery tracking |

---

<a id="recommended-use-order"></a>
## Recommended use order ｜ 推奨使用順

Use the forms in this order when possible:  
可能な場合は、以下の順で使用します。

```text
L30-FRM-B01 -> L30-FRM-I01 -> L30-FRM-A01
Category patterns / 区分別基本パターン: G01 / R01 / S01
Optional detail / 必要時の詳細: B02 / I02 / I03
```

### 1. `L30-FRM-B01`: Boundary Check ｜ 境界判定表

Use first when the reviewer needs to determine whether effective human refusal remained possible before irreversibility.  
不可逆化前に有効な人間拒否が残っていたかを最小判定する場合、最初に使用します。

### 2. `L30-FRM-I01`: Incident Review Template ｜ 事故レビュー記録表

Use after an incident, near-incident, or boundary-failure concern to record the timeline, refusal conditions, control conditions, and review findings.  
事故・準事故・境界失敗懸念の後に、時系列、拒否条件、制御条件、レビュー所見を記録するために使用します。

### 3. `L30-FRM-A01`: Audit Checklist ｜ 監査チェックリスト

Use for governance, deployment, procurement, internal review, or external audit contexts where refusal effectiveness and control conditions must be checked.  
ガバナンス、導入、調達、内部レビュー、外部監査などで、拒否の有効性と制御条件を確認するために使用します。

### Category patterns: `G01`, `R01`, `S01` ｜ 区分別基本パターン

Use `L30-FRM-G01`, `L30-FRM-R01`, or `L30-FRM-S01` when the reviewer needs a baseline English pattern for governance, responsibility, or stabilization use cases.  
ガバナンス、責任、初動安定化の用途に対して、英語版の基本パターンが必要な場合に `L30-FRM-G01`, `L30-FRM-R01`, `L30-FRM-S01` を使用します。

---

<a id="document-id-system"></a>
## Document ID system ｜ 帳票ID体系

The full numbering rules are maintained in:  
詳細な採番ルールは、以下で管理します。

- [L30_FRM Document ID System](./L30_FRM_Document_ID_System.md)

Current filename format:  
現行ファイル名形式：

```text
L30_FRM_[Category][Number]_[English_Title].docx
L30_FRM_[Category][Number]_[English_Title]_JA.docx
```

Examples:  
例：

```text
L30_FRM_B01_Boundary_Check.pdf
L30_FRM_B01_Boundary_Check_JA.pdf
```

---

<a id="relationship-to-boundary-kernel"></a>
## Relationship to Boundary Kernel ｜ Boundary Kernel との関係

The L30-FRM practical forms translate the LUMINA-30 Boundary Kernel into human-readable review fields.  
L30-FRM 実務帳票は、LUMINA-30 Boundary Kernel を人間が使えるレビュー欄に変換したものです。

They are not the Boundary Kernel itself.  
これらは Boundary Kernel 本体ではありません。

They should be interpreted under the following constraints:  
以下の制約のもとで解釈します。

- non-identical anchors are not a substitute for PCR-C;
- boundary failure is not acceptable, recoverable, or a normal operating condition;
- apparent consent, cooperation, silence, or refusal is not valid under LUMINA-30 if produced by AI-mediated control;
- formal compliance, partial compliance, or proxy compliance does not replace effective human refusal before irreversibility.

- 非同一アンカーは PCR-C の代替ではない。
- 境界失敗は許容・回復可能・通常運用ではない。
- AI媒介の支配により成立した同意・協力・沈黙・拒否は、LUMINA-30上の有効な人間拒否ではない。
- 形式的遵守・部分的遵守・代理的遵守は、不可逆化前の有効な人間拒否を代替しない。

---

<a id="version-rules"></a>
## Version and revision rules ｜ バージョン・改訂ルール

- Initial public form releases normally start at `v1_0`.
- The current public form version is `1.0.1` because the first usability correction removed fixed form dates from the main metadata table and added practical review fields.
- Minor wording or scope clarifications may use patch versions such as `v1_0_1`.
- Structural changes to fields, checkboxes, or review logic should use `v1_1`, `v1_2`, and later versions.
- Do not reuse a document ID for a different form type.
- Do not change a form category code unless the old ID is deprecated and mapped to the new ID.

- 初回公開帳票は原則として `v1_0` から開始します。
- 現行公開版は、固定の帳票日付を主要メタ表から外し、実務用のレビュー記入欄を追加した初回ユーザビリティ修正版であるため `1.0.1` とします。
- 軽微な文言・射程修正は `v1_0_1` などのパッチ版を使用できます。
- 項目、チェックボックス、判定ロジックの構造変更は `v1_1`, `v1_2` 以降を使用します。
- 異なる種類の帳票に同じ文書IDを再利用しません。
- 区分コードを変更する場合は、旧IDを廃止扱いにし、新IDへの対応関係を明示します。

---

<a id="short-references"></a>
## Short references ｜ 短縮参照

The following short references may be used in review comments, issues, handoff notes, and audit discussions.  
以下の短縮参照は、レビューコメント、Issue、引き継ぎメモ、監査議論で使用できます。

| Short reference | Full document |
|---|---|
| `B01` | `L30-FRM-B01: Boundary Check` |
| `I01` | `L30-FRM-I01: Incident Review Template` |
| `A01` | `L30-FRM-A01: Audit Checklist` |
| `G01` | `L30-FRM-G01: Governance Review Template` |
| `R01` | `L30-FRM-R01: Responsibility / Accountability Review` |
| `S01` | `L30-FRM-S01: Stabilization Checklist` |
| `B02` | `L30-FRM-B02: Operational Refusal Preservation Minimum` |
| `I02` | `L30-FRM-I02: Incident Review Protocol` |
| `I03` | `L30-FRM-I03: Incident Review Protocol Extended` |

[⬆ TOP](#top)
