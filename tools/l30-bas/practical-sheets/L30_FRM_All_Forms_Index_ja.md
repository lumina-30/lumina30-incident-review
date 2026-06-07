<!-- L30_MD_SOURCE: generated from existing HTML to restore MD/HTML source parity -->
# L30-FRM 全帳票インデックス

---

## 目的

この文書は、`L30-FRM` 帳票ID体系を用いる LUMINA-30
実務帳票群の公開配布インデックス兼管理レジスターです。

レビュー担当者、監査担当者、管理者、AIアシスタントが、使用すべき帳票、ダウンロードすべき言語版、Boundary
Kernel との関係を迷わず確認できるようにします。

公開ファイル名は安定名とし、バージョン番号を含めません。バージョン情報は文書本文、フッター、Git履歴、リリースノートで管理します。

---

## このインデックスではないもの

このインデックス自体は、帳票・チェックリスト・認証・法的基準・導入承認・PCR-C
または LUMINA-30 Boundary Kernel の代替ではありません。

ここに掲載する帳票は、システムの安全性を認証するものではありません。不可逆化前に有効な人間拒否が可能だったかを確認するための構造化された記入欄を提供するものです。
各DOCX/PDF帳票には、レビュー日、レビュー担当者/組織、対象システム/案件IDの記入欄があります。帳票版日付は小さなフッター注記としてのみ保持します。

---

## 言語・ローカライズ方針

英語版の実務帳票ファイルは正規テンプレートとして扱い、言語接尾辞を付けません。

各言語版は、英語正規テンプレートを複製し、人間が読む本文だけを翻訳して作成します。

Document
ID、L30-BASコード、入力欄構造、チェックボックス制御、表、コード配置、レイアウトは、各言語版でも維持します。

各言語版の実務帳票ファイルは、拡張子の直前に大文字の言語接尾辞を付けます。

英語正本テンプレートには接尾辞を付けません。日本語ローカライズ版には
`_JA` を使用します。

言語接尾辞は文書IDの一部ではありません。

実務帳票本文では、`L30-FRM-B01`
のような文書IDのみを表示し、言語コードをIDの一部として表示しません。

例：

国・地域差を示す接尾辞は、法制度・制度運用・言語差により地域版が必要な場合だけ使用します。例：`_EN_US`,
`_EN_GB`, `_ZH_TW`, `_PT_BR`。

日本語ローカライズ版は、各言語版作成の参考例として提供できます。ただし、日本語での実務利用を想定する場合を除き、すべての補助・詳細フォームに日本語版を必須とはしません。

インデックスと管理文書は、GitHub上の導線・保守用文書であるため、英日併記を維持できます。

---

## 上位参照

ここに掲載する帳票は、LUMINA-30 Boundary Kernel
を、人間によるレビュー・事故分析・監査文脈で運用可能にするための補助文書です。

主要境界要件：

> 不可逆化前に、有効な人間拒否が可能でなければならない。

これらの帳票は PCR-C を緩和・代替・延期しません。

---

## 最初に使う帳票の選び方

どの文書を開くべきか迷う場合は、まずこの表から選んでください。

| 状況 | 最初に使うもの | 目的 |
| --- | --- | --- |
| 最小限の境界判定だけを行いたい | `L30-FRM-B01` 境界判定表 | 不可逆化前に有効な人間拒否が残っていたかを確認する |
| 事故・準事故・境界失敗懸念がすでにある | `L30-FRM-I01` 事故レビュー記録表 | 時系列・拒否条件・制御条件・証拠・所見を記録する |
| ガバナンス・導入・調達・内部レビュー・外部監査の文脈である | `L30-FRM-A01` 監査チェックリスト | 拒否権と制御条件が制度上追跡可能かを確認する |
| ガバナンスまたは承認経路の基本パターンが必要 | `L30-FRM-G01` ガバナンスレビュー雛形 | 承認経路、エスカレーション統治、制度的プロセスの健全性を確認する |
| 責任・説明責任の基本パターンが必要 | `L30-FRM-R01` 責任・説明責任レビュー | 責任経路、判定帰属、説明責任の追跡可能性を確認する |
| 初動安定化または封じ込めの基本パターンが必要 | [`L30-FRM-S01` 初動安定化チェックリスト](./L30_FRM_S01_Stabilization_Checklist_JA.md) | 封じ込め、証拠保全、拒否権保全の回復条件を確認する |
| 背景理論や概念説明を確認したい | LUMINA-30本体・参照文書 | 帳票利用前に境界フレームワークを理解する |

---

## 現行帳票

| 文書ID | 表題 | 主用途 | 標準DOCX | 標準PDF | 日本語DOCX | 日本語PDF |
| --- | --- | --- | --- | --- | --- | --- |
| 境界判定表 | 最小境界判定 | [DOCX](./L30_FRM_B01_Boundary_Check.docx) | [PDF](./L30_FRM_B01_Boundary_Check.pdf) | [DOCX](./L30_FRM_B01_Boundary_Check_JA.docx) | [PDF](./L30_FRM_B01_Boundary_Check_JA.pdf) |  |
| 事故レビュー記録表 | Post-incident review record ｜ 事故後レビュー記録 | [DOCX](./L30_FRM_I01_Incident_Review_Template.docx) | [PDF](./L30_FRM_I01_Incident_Review_Template.pdf) | [DOCX](./L30_FRM_I01_Incident_Review_Template_JA.docx) | [PDF](./L30_FRM_I01_Incident_Review_Template_JA.pdf) |  |
| 監査チェックリスト | Audit and governance review ｜ 監査・ガバナンス確認 | [DOCX](./L30_FRM_A01_Audit_Checklist.docx) | [PDF](./L30_FRM_A01_Audit_Checklist.pdf) | [DOCX](./L30_FRM_A01_Audit_Checklist_JA.docx) | [PDF](./L30_FRM_A01_Audit_Checklist_JA.pdf) |  |
| ガバナンスレビュー雛形 | 承認経路・エスカレーション統治の基本パターン | [DOCX](./L30_FRM_G01_Governance_Review_Template.docx) | [PDF](./L30_FRM_G01_Governance_Review_Template.pdf) | — | — |  |
| 責任・説明責任レビュー | 責任経路・説明責任の基本パターン | [DOCX](./L30_FRM_R01_Responsibility_Accountability_Review.docx) | [PDF](./L30_FRM_R01_Responsibility_Accountability_Review.pdf) | — | — |  |
| 初動安定化チェックリスト [HTML guide](./L30_FRM_S01_Stabilization_Checklist_JA.md) / [JA HTML](./L30_FRM_S01_Stabilization_Checklist_JA.md) | 事故後安定化・封じ込めの基本パターン | [DOCX](./L30_FRM_S01_Stabilization_Checklist.docx) | [PDF](./L30_FRM_S01_Stabilization_Checklist.pdf) | — | — |  |

---

## 補助・詳細帳票

以下の帳票は、L30-BAS実務帳票群の一部ですが、多くの利用者にとって最初の入口ではありません。  
最小限の実務入口が必要な場合は、まず
`L30-FRM-B01`、`L30-FRM-I01`、または
`L30-FRM-A01`
を使用します。より詳細な拒否権保全確認または事故レビュー分析が必要な場合に、補助・詳細帳票を使用します。

| 文書ID | 表題 | 主用途 | 標準DOCX | 標準PDF | 日本語DOCX | 日本語PDF |
| --- | --- | --- | --- | --- | --- | --- |
| 運用上の拒否権保全ミニマム | Pre-incident operational refusal-preservation check ｜ 事故前の運用上の拒否権保全確認 | [DOCX](./L30_FRM_B02_Operational_Refusal_Preservation_Minimum.docx) | [PDF](./L30_FRM_B02_Operational_Refusal_Preservation_Minimum.pdf) | — | — |  |
| 事故レビュープロトコル | Detailed post-incident review protocol ｜ 詳細事故後レビュープロトコル | [DOCX](./L30_FRM_I02_Incident_Review_Protocol.docx) | [PDF](./L30_FRM_I02_Incident_Review_Protocol.pdf) | — | — |  |
| 拡張事故レビュープロトコル | Extended post-incident structural analysis ｜ 拡張事故後構造分析 | [DOCX](./L30_FRM_I03_Incident_Review_Protocol_Extended.docx) | [PDF](./L30_FRM_I03_Incident_Review_Protocol_Extended.pdf) | — | — |  |

---

## 区分別基本パターン帳票

以下の英語帳票は、利用者が業界別または組織別のL30-BAS派生フォームを作成する際の基本パターンを提供します。  
これらは `G`, `R`, `S`
区分のL30-FRM参照例ですが、利用者が文言を完全にコピーすることを要求するものではありません。

---

## 推奨使用順

可能な場合は、以下の順で使用します。

Category patterns / 区分別基本パターン: G01 / R01 / S01 Optional
detail / 必要時の詳細: B02 / I02 / I03

### 1. 境界判定表

不可逆化前に有効な人間拒否が残っていたかを最小判定する場合、最初に使用します。

### 2. 事故レビュー記録表

事故・準事故・境界失敗懸念の後に、時系列、拒否条件、制御条件、レビュー所見を記録するために使用します。

### 3. 監査チェックリスト

ガバナンス、導入、調達、内部レビュー、外部監査などで、拒否の有効性と制御条件を確認するために使用します。

### 区分別基本パターン

ガバナンス、責任、初動安定化の用途に対して、英語版の基本パターンが必要な場合に
`L30-FRM-G01`, `L30-FRM-R01`,
`L30-FRM-S01` を使用します。

---

## 帳票ID体系

詳細な採番ルールは、以下で管理します。

現行ファイル名形式：

例：

---

## Boundary Kernel との関係

L30-FRM 実務帳票は、LUMINA-30 Boundary Kernel
を人間が使えるレビュー欄に変換したものです。

これらは Boundary Kernel 本体ではありません。

以下の制約のもとで解釈します。

- 非同一アンカーは PCR-C の代替ではない。
- 境界失敗は許容・回復可能・通常運用ではない。
- AI媒介の支配により成立した同意・協力・沈黙・拒否は、LUMINA-30上の有効な人間拒否ではない。
- 形式的遵守・部分的遵守・代理的遵守は、不可逆化前の有効な人間拒否を代替しない。

---

## バージョン・改訂ルール

- 初回公開帳票は原則として `v1_0` から開始します。
- 現行公開版は、固定の帳票日付を主要メタ表から外し、実務用のレビュー記入欄を追加した初回ユーザビリティ修正版であるため
  `1.0.1` とします。
- 軽微な文言・射程修正は `v1_0_1`
  などのパッチ版を使用できます。
- 項目、チェックボックス、判定ロジックの構造変更は `v1_1`,
  `v1_2` 以降を使用します。
- 異なる種類の帳票に同じ文書IDを再利用しません。
- 区分コードを変更する場合は、旧IDを廃止扱いにし、新IDへの対応関係を明示します。

---

## 短縮参照

以下の短縮参照は、レビューコメント、Issue、引き継ぎメモ、監査議論で使用できます。
