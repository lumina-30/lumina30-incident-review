<!-- L30_LANG_LOCK: EN_JP_PAIRED -->
<a id="top"></a>

# L30-FRM Document ID System ｜ LUMINA-30 帳票ID体系

Current Version: 1.0.2  
Last Updated: May 2026  
Repository path: `lumina30-incident-review/tools/l30-bas/practical-sheets/L30_FRM_Document_ID_System.md`  
License: CC0 1.0 Universal (Public Domain)

[All Forms Index](./L30_FRM_All_Forms_Index.md) ｜ [ID Format](#filename-format) ｜ [Language Rule](#language-rule) ｜ [Current Register](#current-form-register)

---

## Purpose ｜ 目的

This document defines the document ID system for LUMINA-30 practical forms, sheets, templates, and checklists.  
この文書は、LUMINA-30 が提供する実務用帳票・シート・テンプレート・チェックリストの管理番号体系を定義します。

The purpose is to keep each form consistently referenceable, reviewable, updateable, and usable in incident review, audit, and boundary-evaluation contexts.  
目的は、各帳票を事故検証・監査・境界評価の中で、一貫して参照・レビュー・更新・利用できる状態に保つことです。

---

## What this system is not ｜ この体系ではないもの

The L30-FRM document ID system is not a certification scheme, compliance label, safety approval, legal classification, or replacement for PCR-C or the LUMINA-30 Boundary Kernel.  
L30-FRM 文書ID体系は、認証制度、適合ラベル、安全承認、法的分類、PCR-C または LUMINA-30 Boundary Kernel の代替ではありません。

It is a document-control system for practical forms only.  
これは実務帳票に限定した文書管理体系です。

---

<a id="document-id"></a>
## Document ID ｜ 文書ID

The stable document ID uses hyphens, not underscores, and does not include a language suffix.  
安定文書IDはアンダースコアではなくハイフンを使用し、言語接尾辞を含めません。

Public filenames use underscores for filesystem and URL compatibility.  
公開ファイル名は、ファイルシステムおよびURL互換性のためアンダースコアを使用します。

Stable document IDs:  
安定文書ID：

```text
L30-FRM-B01
L30-FRM-B02
L30-FRM-I01
L30-FRM-I02
L30-FRM-I03
L30-FRM-A01
L30-FRM-G01
L30-FRM-R01
L30-FRM-S01
```

---

<a id="language-rule"></a>
## Language rule ｜ 言語ルール

English files are the canonical templates and do not use a language suffix.  
英語版ファイルは正規テンプレートとして扱い、言語接尾辞を付けません。

Localized versions should be created by copying the English canonical template and translating only the human-readable text.  
各言語版は、英語正規テンプレートを複製し、人間が読む本文だけを翻訳して作成します。

Document IDs, L30-BAS codes, field structure, checkbox controls, tables, code placement, and layout should be preserved across localized versions.  
Document ID、L30-BASコード、入力欄構造、チェックボックス制御、表、コード配置、レイアウトは、各言語版でも維持します。

Localized files use an uppercase language suffix immediately before the file extension.  
各言語版ファイルは、拡張子の直前に大文字の言語接尾辞を付けます。

Japanese files use the `_JA` language suffix.  
日本語版ファイルは `_JA` 言語接尾辞を使用します。

The language suffix is not part of the document ID.  
言語接尾辞は文書IDの一部ではありません。

The practical form body should show only the document ID and should not show language code as part of the ID.  
実務帳票本文では文書IDのみを表示し、言語コードをIDの一部として表示しません。

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

---

<a id="filename-format"></a>
## Filename format ｜ ファイル名形式

Public filenames do not include version numbers. English files use the default filename. Localized files use an uppercase language suffix before the file extension.  
公開ファイル名にはバージョン番号を入れません。英語版は標準ファイル名を使用し、各言語版は拡張子の直前に大文字の言語接尾辞を付けます。

```text
L30_FRM_[Category][Number]_[English_Title].docx
L30_FRM_[Category][Number]_[English_Title].pdf
L30_FRM_[Category][Number]_[English_Title]_[LANGUAGE].docx
L30_FRM_[Category][Number]_[English_Title]_[LANGUAGE].pdf
```

Public filenames do not include version numbers. Version information is stored inside the document, footer, Git history, releases/tags, and review-candidate ZIP names.  
公開ファイル名にはバージョン番号を入れません。バージョン情報は、文書内、フッター、Git履歴、Release/Tag、レビュー候補ZIP名で管理します。

| Component | Meaning |
|---|---|
| `L30-FRM-[Category][Number]` | Stable document ID shown inside the form |
| `L30_FRM_[Category][Number]_[English_Title]` | Public filename base using underscores |
| `_[LANGUAGE]` | Localized language suffix, used only in filenames and not part of the document ID |

---

<a id="category-codes"></a>
## Category codes ｜ 区分コード

| Code | Category | Use |
|---|---|---|
| `B` | Boundary | Boundary judgment, refusal validity, pre-irreversibility checks |
| `I` | Incident | Incident review, post-incident records, near-miss analysis |
| `A` | Audit | Audit, governance review, operational readiness checks |
| `G` | Governance | Approval flow, institutional process, escalation governance |
| `R` | Responsibility | Responsibility mapping, accountability, role assignment |
| `S` | Stabilization | Post-incident stabilization, containment, recovery tracking |

A new category should be created only when the form has a clearly different operational purpose.  
新しい区分は、その帳票が既存区分とは明確に異なる実務目的を持つ場合に限って作成します。

---

<a id="current-form-register"></a>
## Current form register ｜ 現行帳票レジスター

| Document ID | Default English file base | Japanese file base | Primary use |
|---|---|---|---|
| `L30-FRM-B01` | `L30_FRM_B01_Boundary_Check` | `L30_FRM_B01_Boundary_Check_JA` | Minimum boundary judgment sheet for effective human refusal before irreversibility |
| `L30-FRM-B02` | `L30_FRM_B02_Operational_Refusal_Preservation_Minimum` | — | Minimum operational conditions for preserving reviewable human refusal authority |
| `L30-FRM-I01` | `L30_FRM_I01_Incident_Review_Template` | `L30_FRM_I01_Incident_Review_Template_JA` | Incident or near-incident review record aligned with the LUMINA-30 Boundary Kernel |
| `L30-FRM-I02` | `L30_FRM_I02_Incident_Review_Protocol` | — | Detailed post-incident review protocol |
| `L30-FRM-I03` | `L30_FRM_I03_Incident_Review_Protocol_Extended` | — | Extended post-incident structural analysis |
| `L30-FRM-A01` | `L30_FRM_A01_Audit_Checklist` | `L30_FRM_A01_Audit_Checklist_JA` | Audit checklist for pre-critical control readiness and refusal validity |
| `L30-FRM-G01` | `L30_FRM_G01_Governance_Review_Template` | — | Governance review pattern for approval flow and escalation governance |
| `L30-FRM-R01` | `L30_FRM_R01_Responsibility_Accountability_Review` | — | Responsibility and accountability review pattern |
| `L30-FRM-S01` | `L30_FRM_S01_Stabilization_Checklist` | — | Stabilization, containment, and recovery-tracking checklist |

---

<a id="relationship-to-boundary-kernel"></a>
## Relationship to Boundary Kernel ｜ Boundary Kernel との関係

These forms do not replace PCR-C or the LUMINA-30 Boundary Kernel.  
これらの帳票は、PCR-C または LUMINA-30 Boundary Kernel を代替しません。

They operationalize the Boundary Kernel for human review, incident analysis, and audit contexts.  
Boundary Kernel を、人間によるレビュー・事故分析・監査文脈で運用可能にするための補助帳票です。

They must not be used as certification marks or as claims that a system is safe.  
これらの帳票を、認証マークや「システムが安全である」という主張として使用してはなりません。

---

<a id="versioning-rule"></a>
## Versioning rule ｜ バージョン管理ルール

A form version changes when its content, checklist structure, judgment criteria, or practical use changes.  
帳票の内容、チェックリスト構造、判定基準、実務用途が変わる場合は、バージョンを変更します。

English and localized versions of the same form should share the same document ID and version number.  
同じ帳票の英語版と各言語版は、同じ文書IDとバージョン番号を共有します。

Use v1_0_1 for the first usability correction that moves fixed form dates out of the main metadata table and adds practical review fields.  
固定の帳票日付を主要メタ表から外し、実務用のレビュー記入欄を追加する初回ユーザビリティ修正にはv1_0_1を使用します。

---

<a id="assignment-rule"></a>
## Assignment rule ｜ 採番ルール

New IDs should be assigned conservatively.  
新しいIDは慎重に割り当てます。

Use a new category only when the form has a clearly different operational purpose.  
帳票の実務目的が明確に異なる場合のみ、新しい区分を使用します。

Do not reuse retired IDs for different forms.  
廃止済みIDを別帳票に再利用しません。

Do not assign a form ID to a theoretical paper, README, diagram, slide, or general explanatory document.  
理論論文、README、図版、スライド、一般説明文書には帳票IDを付与しません。

[⬆ TOP](#top)
