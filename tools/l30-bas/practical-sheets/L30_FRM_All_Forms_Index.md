<a id="top"></a>

# L30_FRM All Forms Index ｜ L30_FRM 全帳票インデックス

Current Version: 1.0.1  
Last Updated: May 2026  
Repository path: `lumina30-incident-review/tools/l30-bas/practical-sheets/L30_FRM_All_Forms_Index.md`

[Document ID System](./L30_FRM_Document_ID_System.md) ｜ [Which Form First](#which-form-first) ｜ [Current Forms](#current-forms) ｜ [Supporting Forms](#supporting-detailed-forms) ｜ [Use Order](#recommended-use-order) ｜ [Boundary Relation](#relationship-to-boundary-kernel)

---

## Purpose ｜ 目的

This document is the public distribution index and management register for LUMINA-30 practical form documents using the `L30_FRM` document ID system.  
この文書は、`L30_FRM` 帳票ID体系を用いる LUMINA-30 実務帳票群の公開配布インデックス兼管理レジスターです。

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
## Language policy for practical tools ｜ 実務ツールの言語方針

English practical form files are the default and do not use a language suffix.  
英語版の実務帳票ファイルは標準版として扱い、言語接尾辞を付けません。

Japanese practical form files use `_JP` immediately before the file extension.  
日本語版の実務帳票ファイルは、拡張子の直前に `_JP` を付けます。

The `_JP` suffix is not part of the document ID.  
`_JP` は文書IDの一部ではありません。

The practical form body should show only the document ID, such as `L30_FRM_B01`, and should not show a language code as part of the ID.  
実務帳票本文では、`L30_FRM_B01` のような文書IDのみを表示し、言語コードをIDの一部として表示しません。

Examples:  
例：

```text
Document ID: L30_FRM_B01
Default English file: L30_FRM_B01_Boundary_Check.docx
Japanese file: L30_FRM_B01_Boundary_Check_JP.docx
```

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
| I only need a minimum boundary determination. ｜ 最小限の境界判定だけを行いたい | `L30_FRM_B01` Boundary Check ｜ 境界判定表 | Check whether effective human refusal remained possible before irreversibility ｜ 不可逆化前に有効な人間拒否が残っていたかを確認する |
| An incident, near-incident, or boundary-failure concern has already occurred. ｜ 事故・準事故・境界失敗懸念がすでにある | `L30_FRM_I01` Incident Review Template ｜ 事故レビュー記録表 | Record timeline, refusal conditions, control conditions, evidence, and findings ｜ 時系列・拒否条件・制御条件・証拠・所見を記録する |
| The context is governance, deployment, procurement, internal review, or external audit. ｜ ガバナンス・導入・調達・内部レビュー・外部監査の文脈である | `L30_FRM_A01` Audit Checklist ｜ 監査チェックリスト | Review whether refusal authority and control conditions remain institutionally traceable ｜ 拒否権と制御条件が制度上追跡可能かを確認する |
| I need background theory or conceptual explanation. ｜ 背景理論や概念説明を確認したい | LUMINA-30 Core / Reference documents ｜ LUMINA-30本体・参照文書 | Understand the boundary framework before using the forms ｜ 帳票利用前に境界フレームワークを理解する |

---

<a id="current-forms"></a>
## Current forms ｜ 現行帳票

| Document ID | Title | Primary use | Default DOCX | Default PDF | JP DOCX | JP PDF |
|---|---|---|---|---|---|---|
| `L30_FRM_B01` | Boundary Check ｜ 境界判定表 | Minimum boundary determination ｜ 最小境界判定 | [DOCX](./L30_FRM_B01_Boundary_Check.docx) | [PDF](./L30_FRM_B01_Boundary_Check.pdf) | [DOCX](./L30_FRM_B01_Boundary_Check_JP.docx) | [PDF](./L30_FRM_B01_Boundary_Check_JP.pdf) |
| `L30_FRM_I01` | Incident Review Template ｜ 事故レビュー記録表 | Post-incident review record ｜ 事故後レビュー記録 | [DOCX](./L30_FRM_I01_Incident_Review_Template.docx) | [PDF](./L30_FRM_I01_Incident_Review_Template.pdf) | [DOCX](./L30_FRM_I01_Incident_Review_Template_JP.docx) | [PDF](./L30_FRM_I01_Incident_Review_Template_JP.pdf) |
| `L30_FRM_A01` | Audit Checklist ｜ 監査チェックリスト | Audit and governance review ｜ 監査・ガバナンス確認 | [DOCX](./L30_FRM_A01_Audit_Checklist.docx) | [PDF](./L30_FRM_A01_Audit_Checklist.pdf) | [DOCX](./L30_FRM_A01_Audit_Checklist_JP.docx) | [PDF](./L30_FRM_A01_Audit_Checklist_JP.pdf) |

---

<a id="supporting-detailed-forms"></a>
## Supporting / Detailed Forms ｜ 補助・詳細帳票

The following forms are part of the L30-BAS practical form family, but they are not the first entry point for most users.  
Use `L30_FRM_B01`, `L30_FRM_I01`, or `L30_FRM_A01` first when a minimum practical entry point is needed. Use the supporting forms when more detailed refusal-preservation or incident-review analysis is required.

以下の帳票は、L30-BAS実務帳票群の一部ですが、多くの利用者にとって最初の入口ではありません。  
最小限の実務入口が必要な場合は、まず `L30_FRM_B01`、`L30_FRM_I01`、または `L30_FRM_A01` を使用します。より詳細な拒否権保全確認または事故レビュー分析が必要な場合に、補助・詳細帳票を使用します。

| Document ID | Title | Primary use | Default DOCX | Default PDF | JP DOCX | JP PDF |
|---|---|---|---|---|---|---|
| `L30_FRM_B02` | Operational Refusal Preservation Minimum ｜ 運用上の拒否権保全ミニマム | Pre-incident operational refusal-preservation check ｜ 事故前の運用上の拒否権保全確認 | [DOCX](./L30_FRM_B02_Operational_Refusal_Preservation_Minimum.docx) | [PDF](./L30_FRM_B02_Operational_Refusal_Preservation_Minimum.pdf) | — | — |
| `L30_FRM_I02` | Incident Review Protocol ｜ 事故レビュープロトコル | Detailed post-incident review protocol ｜ 詳細事故後レビュープロトコル | [DOCX](./L30_FRM_I02_Incident_Review_Protocol.docx) | [PDF](./L30_FRM_I02_Incident_Review_Protocol.pdf) | — | — |
| `L30_FRM_I03` | Incident Review Protocol Extended ｜ 拡張事故レビュープロトコル | Extended post-incident structural analysis ｜ 拡張事故後構造分析 | [DOCX](./L30_FRM_I03_Incident_Review_Protocol_Extended.docx) | [PDF](./L30_FRM_I03_Incident_Review_Protocol_Extended.pdf) | — | — |

---

<a id="recommended-use-order"></a>
## Recommended use order ｜ 推奨使用順

Use the forms in this order when possible:  
可能な場合は、以下の順で使用します。

```text
L30_FRM_B01 -> L30_FRM_I01 -> L30_FRM_A01
Optional detail / 必要時の詳細: B02 / I02 / I03
```

### 1. `L30_FRM_B01`: Boundary Check ｜ 境界判定表

Use first when the reviewer needs to determine whether effective human refusal remained possible before irreversibility.  
不可逆化前に有効な人間拒否が残っていたかを最小判定する場合、最初に使用します。

### 2. `L30_FRM_I01`: Incident Review Template ｜ 事故レビュー記録表

Use after an incident, near-incident, or boundary-failure concern to record the timeline, refusal conditions, control conditions, and review findings.  
事故・準事故・境界失敗懸念の後に、時系列、拒否条件、制御条件、レビュー所見を記録するために使用します。

### 3. `L30_FRM_A01`: Audit Checklist ｜ 監査チェックリスト

Use for governance, deployment, procurement, internal review, or external audit contexts where refusal effectiveness and control conditions must be checked.  
ガバナンス、導入、調達、内部レビュー、外部監査などで、拒否の有効性と制御条件を確認するために使用します。

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
L30_FRM_[Category][Number]_[English_Title]_JP.docx
```

Examples:  
例：

```text
L30_FRM_B01_Boundary_Check.pdf
L30_FRM_B01_Boundary_Check_JP.pdf
```

---

<a id="relationship-to-boundary-kernel"></a>
## Relationship to Boundary Kernel ｜ Boundary Kernel との関係

The L30_FRM practical forms translate the LUMINA-30 Boundary Kernel into human-readable review fields.  
L30_FRM 実務帳票は、LUMINA-30 Boundary Kernel を人間が使えるレビュー欄に変換したものです。

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
| `B01` | `L30_FRM_B01: Boundary Check` |
| `I01` | `L30_FRM_I01: Incident Review Template` |
| `A01` | `L30_FRM_A01: Audit Checklist` |
| `B02` | `L30_FRM_B02: Operational Refusal Preservation Minimum` |
| `I02` | `L30_FRM_I02: Incident Review Protocol` |
| `I03` | `L30_FRM_I03: Incident Review Protocol Extended` |

[⬆ TOP](#top)
