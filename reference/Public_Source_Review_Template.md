<!-- L30_LANG_LOCK: EN_JP_PAIRED -->
# Public-Source Review Template: AI-Mediated Authority Path and Effective Refusal Risk ｜ 公開情報レビュー・テンプレート：AI媒介の権限経路と実効的拒否リスク

> **HTML reading route ｜ HTML閲覧導線**  
> [Open English HTML](https://lumina-30.github.io/lumina30-incident-review/reference/Public_Source_Review_Template.html) ｜ [日本語HTMLを開く](https://lumina-30.github.io/lumina30-incident-review/reference/Public_Source_Review_Template_ja.html)

## Status ｜ ステータス

This is a reusable public-source review template. It is not a completed incident review, official attribution, certification, regulatory finding, legal conclusion, safety determination, or proof of institutional adoption.

これは再利用可能な公開情報レビュー用テンプレートです。完成済み事故レビュー、公式な原因認定、認証、規制上の判断、法的結論、安全性判定、制度的採用の証拠ではありません。

## When to use this template ｜ このテンプレートを使う場面

Use this when an AI-related case is known through public reporting, public statements, public documentation, public screenshots, papers, or third-party summaries, and the review must avoid overstating what is known.

AI関連事案について、公開報道、公開声明、公開文書、公開スクリーンショット、論文、第三者要約だけが利用可能であり、確認済みでない内容を断定してはいけない場合に使います。

## Required label ｜ 必須ラベル

> **Public-source review only.** This review does not claim access to internal logs, private incident records, official attribution, regulatory findings, legal conclusions, or safety determinations.

> **公開情報レビューのみ。** 本レビューは、内部ログ、非公開事故記録、公式な原因認定、規制上の判断、法的結論、安全性判定へのアクセスまたは確定を主張しません。

## Review fields ｜ レビュー記入欄

### 1. Case title ｜ 事案タイトル

- Working title:
- Public-source review date:
- Reviewer / maintainer:
- Scope of public sources used:

- 作業用タイトル：
- 公開情報レビュー日：
- レビュー担当・保守者：
- 使用した公開情報の範囲：

### 2. Source register ｜ 情報源一覧

| Source | Date | Type | What it supports | What it does not prove |
|---|---|---|---|---|
|  |  | Public report / official statement / paper / post / documentation |  |  |

| 情報源 | 日付 | 種別 | 支える内容 | 証明しない内容 |
|---|---|---|---|---|
|  |  | 公開報道 / 公式声明 / 論文 / 投稿 / 文書 |  |  |

### 3. Public facts ｜ 公開情報から確認できる事実

List only claims directly supported by public sources.

公開情報から直接支えられる内容だけを列挙します。

- Fact 1:
- Fact 2:
- Fact 3:

### 4. Inferences ｜ 推定事項

List plausible inferences separately from facts. Mark uncertainty.

事実とは分けて、可能な推定事項を列挙します。不確実性を明記します。

- Inference 1:
- Confidence level:
- Required evidence to confirm:

### 5. Unknowns and unresolved conclusions ｜ 不明点と未確定結論

List what must remain unresolved because internal logs, private records, official findings, or direct evidence are unavailable.

内部ログ、非公開記録、公式判断、直接証拠がないため、未確定として残すべき内容を列挙します。

- Unknown 1:
- Unknown 2:
- Conclusion that must not be stated:

### 6. Actor-Authority-Evidence mapping ｜ Actor-Authority-Evidence マッピング

| Layer | Review question | Public evidence | Gap / unresolved item |
|---|---|---|---|
| Human requester / operator | Who initiated, approved, used, or relied on the AI-mediated action? |  |  |
| AI assistant / agent | What did the AI judge, recommend, route, generate, or execute? |  |  |
| Platform automation layer | Which automated workflow acted after the AI output or user interaction? |  |  |
| Privileged system / API | Did the process affect account recovery, credentials, production state, tools, rollback, or appeal routes? |  |  |
| Accountable human or organization | Who could pause, reverse, escalate, or contain before irreversibility? |  |  |
| Affected human / account owner | Could the affected party appeal, recover, contest, or stop the result? |  |  |
| Evidence custodian | Who controls logs, timestamps, records, or missing-evidence notes? |  |  |

| 層 | レビュー質問 | 公開証拠 | 空白・未確定事項 |
|---|---|---|---|
| 人間の依頼者・運用者 | 誰がAI媒介行為を開始、承認、使用、または依拠したのか。 |  |  |
| AIアシスタント・エージェント | AIは何を判断、推奨、振り分け、生成、または実行したのか。 |  |  |
| プラットフォーム自動化層 | AI出力または利用者操作の後に、どの自動ワークフローが作動したのか。 |  |  |
| 特権システム・API | アカウント復旧、認証情報、本番状態、ツール、rollback、異議申立て経路に影響したか。 |  |  |
| 責任ある人間・組織 | 不可逆化前に一時停止、撤回、エスカレーション、封じ込めが可能だった主体は誰か。 |  |  |
| 被影響者・アカウント所有者 | 影響を受けた当事者は、異議申立て、回復、争い、停止ができたのか。 |  |  |
| 証拠管理者 | ログ、時刻、記録、不足証拠メモを管理する主体は誰か。 |  |  |

### 7. Effective refusal window ｜ 実効的拒否の時間窓

- Last point at which a human could plausibly refuse, stop, suspend, reverse, or escalate:
- Evidence that this point existed:
- Evidence that this point was effective:
- Evidence gap:

- 人間が拒否、停止、保留、撤回、エスカレーションできた可能性のある最後の時点：
- その時点が存在した証拠：
- その時点が実効的だった証拠：
- 証拠ギャップ：

### 8. Boundary review trigger ｜ 境界レビューのトリガー

Mark whether the public-source case suggests any of the following adoption-review triggers:

公開情報レビュー対象が、次の採用審査トリガーを示唆するかを確認します。

- [ ] AI-mediated account recovery, credential change, production action, tool execution, or privileged API access.
- [ ] Human review existed on paper, but its timing, authority, or evidence is unclear.
- [ ] Rollback, appeal, recovery, or stop authority may have been unavailable after the AI-mediated action.
- [ ] Evidence needed to reconstruct the incident is controlled by a party whose role is also under review.

- [ ] AI媒介のアカウント復旧、認証情報変更、本番操作、ツール実行、特権APIアクセス。
- [ ] 書類上の人間レビューは存在するが、その時点、権限、証拠が不明確。
- [ ] AI媒介行為の後に、rollback、異議申立て、回復、停止権限が利用不能だった可能性。
- [ ] 事故再構成に必要な証拠が、レビュー対象でもある主体に管理されている。

### 9. Safe summary ｜ 安全な要約

Use wording such as:

次のような表現を使います。

> Based on public sources only, this case raises questions about actor identity, authority routing, evidence availability, and whether effective human refusal remained available before irreversible effect. It does not establish official attribution, legal responsibility, regulatory violation, or internal causation.

> 公開情報だけに基づくと、この事案は、主体の特定、権限経路、証拠の利用可能性、不可逆的影響の前に実効的人間拒否が残っていたかについての問いを提起します。公式な原因認定、法的責任、規制違反、内部原因を確定するものではありません。

## Related LUMINA-30 pages ｜ 関連ページ

- [Public-Source Review and Actor-Authority-Evidence Mapping](./Public_Source_Review_and_Actor_Authority_Evidence_Mapping.md)
- [Required Questions 5](../boundary-check/Required_Questions_5.md)
- [LUMINA-30 Boundary Check](../boundary-check/LUMINA-30_Boundary_Check.md)
- [Boundary Check for AI Incident Response](../external-use/Boundary_Check_for_AI_Incident_Response.md)

