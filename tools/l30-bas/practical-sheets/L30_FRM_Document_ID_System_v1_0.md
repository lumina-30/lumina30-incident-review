<a id="top"></a>

# L30_FRM Document ID System ｜ LUMINA-30 帳票ID体系

Version: 1.0  
Date: May 2026  
Repository path: `lumina30-incident-review/tools/l30-bas/practical-sheets/L30_FRM_Document_ID_System_v1_0.md`  
License: CC0 1.0 Universal (Public Domain)

[All Forms Index](./L30_FRM_All_Forms_Index_v1_0.md) ｜ [ID Format](#filename-format) ｜ [Language Rule](#language-rule) ｜ [Current Register](#current-form-register)

---

## Purpose ｜ 目的

This document defines the document ID system for LUMINA-30 practical forms, sheets, templates, and checklists.  
この文書は、LUMINA-30 が提供する実務用帳票・シート・テンプレート・チェックリストの管理番号体系を定義します。

The purpose is to make each form easy to reference, review, update, and use in incident review, audit, and boundary-evaluation contexts.  
目的は、各帳票を事故検証・監査・境界評価の中で、一貫して参照・レビュー・更新・利用できるようにすることです。

---

## What this system is not ｜ この体系ではないもの

The L30_FRM numbering system is not a certification scheme, compliance label, safety approval, legal classification, or replacement for PCR-C or the LUMINA-30 Boundary Kernel.  
L30_FRM 番号体系は、認証制度、適合ラベル、安全承認、法的分類、PCR-C または LUMINA-30 Boundary Kernel の代替ではありません。

It is a document-control system for practical forms only.  
これは実務帳票に限定した文書管理体系です。

---

<a id="document-id"></a>
## Document ID ｜ 文書ID

The official document ID does not include a language suffix.  
正式な文書IDには、言語接尾辞を含めません。

Official document IDs:  
正式文書ID：

```text
L30_FRM_B01
L30_FRM_I01
L30_FRM_A01
```

---

<a id="language-rule"></a>
## Language rule ｜ 言語ルール

English files are the default and do not use a language suffix.  
英語版ファイルは標準版として扱い、言語接尾辞を付けません。

Japanese files use `_JP` immediately before the file extension.  
日本語版ファイルは、拡張子の直前に `_JP` を付けます。

The `_JP` suffix is not part of the document ID.  
`_JP` は文書IDの一部ではありません。

The practical form body should show only the document ID and should not show language code as part of the ID.  
実務帳票本文では文書IDのみを表示し、言語コードをIDの一部として表示しません。

Examples:  
例：

```text
Document ID: L30_FRM_B01
Default English file: L30_FRM_B01_Boundary_Check_v1_0.docx
Japanese file: L30_FRM_B01_Boundary_Check_v1_0_JP.docx
```

---

<a id="filename-format"></a>
## Filename format ｜ ファイル名形式

```text
L30_FRM_[Category][Number]_[English_Title]_vX_Y.docx
L30_FRM_[Category][Number]_[English_Title]_vX_Y.pdf
L30_FRM_[Category][Number]_[English_Title]_vX_Y_JP.docx
L30_FRM_[Category][Number]_[English_Title]_vX_Y_JP.pdf
```

| Component | Meaning |
|---|---|
| `L30_FRM_[Category][Number]` | Official document ID |
| `[English_Title]` | Underscore-separated English title |
| `vX_Y` | Public version number |
| `_JP` | Japanese-language suffix, not part of the document ID |

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
| `L30_FRM_B01` | `L30_FRM_B01_Boundary_Check_v1_0` | `L30_FRM_B01_Boundary_Check_v1_0_JP` | Minimum boundary judgment sheet for effective human refusal before irreversibility |
| `L30_FRM_I01` | `L30_FRM_I01_Incident_Review_Template_v1_0` | `L30_FRM_I01_Incident_Review_Template_v1_0_JP` | Incident or near-incident review record aligned with the LUMINA-30 Boundary Kernel |
| `L30_FRM_A01` | `L30_FRM_A01_Audit_Checklist_v1_0` | `L30_FRM_A01_Audit_Checklist_v1_0_JP` | Audit checklist for pre-critical control readiness and refusal validity |

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

English and Japanese versions of the same form should share the same document ID and version number.  
同じ帳票の英語版と日本語版は、同じ文書IDとバージョン番号を共有します。

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
