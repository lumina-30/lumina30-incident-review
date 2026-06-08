<!-- L30_LANG_LOCK: EN_JP_PAIRED -->
# Public-Source Review and Actor-Authority-Evidence Mapping ｜ 公開情報レビューと Actor-Authority-Evidence マッピング

> **HTML reading route ｜ HTML閲覧導線**  
> [Open English HTML](https://lumina-30.github.io/lumina30-incident-review/reference/Public_Source_Review_and_Actor_Authority_Evidence_Mapping.html) ｜ [日本語HTMLを開く](https://lumina-30.github.io/lumina30-incident-review/reference/Public_Source_Review_and_Actor_Authority_Evidence_Mapping_ja.html)

## Status ｜ ステータス

This document is a public-source review aid for LUMINA-30 incident and boundary review. It does not claim access to private logs, internal incident records, official attribution, certification status, regulatory findings, or legal conclusions.

本書は、LUMINA-30のインシデントレビューおよび境界レビューのための公開情報レビュー補助です。非公開ログ、内部事故記録、公式な原因認定、認証状態、規制上の判断、法的結論へのアクセスまたは確定を主張するものではありません。

## Purpose ｜ 目的

Use this mapping when an AI-related case is known only through public reporting, public statements, public documentation, screenshots, papers, or third-party summaries. The goal is to separate what is known, what is inferred, what is missing, and what must not be concluded.

公開報道、公開声明、公開文書、スクリーンショット、論文、第三者要約だけでAI関連事案を確認する場合に、このマッピングを使います。目的は、確認済み事項、推定事項、不足している証拠、結論してはいけない事項を分けることです。

## Actor-Authority-Evidence map ｜ Actor-Authority-Evidence マップ

| Layer | What to identify | Evidence to retain | What not to assume |
|---|---|---|---|
| Human requester or operator | Who initiated, approved, used, or relied on the AI-mediated action. | Public statement, workflow description, timestamp, review record, approval record if public. | Do not assume actual control merely because a human was nominally present. |
| Affected human or account owner | Who was affected and who could appeal, recover, contest, or stop the result. | Public report, notice, appeal path, recovery path, support record if public. | Do not assume appeal or recovery was effective without evidence. |
| AI assistant or agent | What the AI judged, recommended, routed, generated, or executed. | Product description, transcript, prompt log if public, incident report, visible output. | Do not treat a model-output error as the only possible failure mode. |
| Platform automation layer | Which automated workflow acted after the AI output or user interaction. | Public architecture description, support-flow documentation, API behavior, public postmortem. | Do not assume the AI had final authority if automation or platform rules executed the action. |
| Privileged system or API | Whether account recovery, credential changes, production actions, tool execution, or rollback suppression occurred. | Public technical note, audit excerpt if public, timeline, affected-state record. | Do not infer privileged access without evidence. |
| Accountable organization or human authority | Who could have paused, reversed, escalated, or contained the action before irreversibility. | Governance statement, incident response note, escalation path, responsible team statement. | Do not convert organizational responsibility into proof that refusal was available in time. |
| External attacker, if any | Whether an external actor manipulated, induced, exploited, or routed the AI-mediated process. | Public vulnerability report, disclosure timeline, exploit description, official statement. | Do not attribute intent, identity, or causation beyond public evidence. |
| Evidence custodian | Who preserves logs, messages, timestamps, recovery records, approvals, and missing-evidence notes. | Public preservation statement, investigation scope, evidence inventory if public. | Do not treat missing evidence as proof of safety, refusal, or procedural validity. |

| 層 | 確認すること | 保全する証拠 | 推定してはいけないこと |
|---|---|---|---|
| 人間の依頼者・運用者 | AI媒介行為を開始、承認、使用、または依拠した人。 | 公開声明、ワークフロー説明、時刻、レビュー記録、公開された承認記録。 | 人間が名目上存在しただけで、実際の制御があったと推定しない。 |
| 被影響者・アカウント所有者 | 影響を受けた人、および異議申立て、回復、争い、停止が可能だった人。 | 公開報道、通知、異議申立て経路、回復経路、公開されたサポート記録。 | 異議申立てや回復が実効的だったと、証拠なしに推定しない。 |
| AIアシスタント・エージェント | AIが判断、推奨、振り分け、生成、または実行したこと。 | 製品説明、公開された会話記録、公開プロンプトログ、事故報告、可視出力。 | モデル出力ミスだけを唯一の失敗モードとして扱わない。 |
| プラットフォーム自動化層 | AI出力または利用者操作の後に作動した自動ワークフロー。 | 公開された構成説明、サポートフロー文書、API挙動、公開ポストモーテム。 | 自動化やプラットフォーム規則が実行した行為を、AIの最終権限と即断しない。 |
| 特権システム・API | アカウント復旧、認証情報変更、本番操作、ツール実行、rollback抑制が起きたか。 | 公開技術メモ、公開監査抜粋、時系列、影響状態の記録。 | 証拠なしに特権アクセスがあったと推定しない。 |
| 責任組織・人間権限者 | 不可逆化前に一時停止、撤回、エスカレーション、封じ込めが可能だった主体。 | ガバナンス声明、事故対応メモ、エスカレーション経路、責任チームの声明。 | 組織責任があることを、時間内の拒否可能性の証拠へ変換しない。 |
| 外部攻撃者がいる場合 | 外部主体がAI媒介プロセスを操作、誘導、悪用、経路化したか。 | 公開脆弱性報告、開示時系列、exploit説明、公式声明。 | 公開証拠を超えて意図、身元、原因を断定しない。 |
| 証拠管理者 | ログ、メッセージ、時刻、回復記録、承認、不足証拠メモを保全する主体。 | 公開された保全声明、調査範囲、公開証拠一覧。 | 証拠不在を、安全性、拒否可能性、手続き的有効性の証明として扱わない。 |

## Minimal public-source review questions ｜ 公開情報レビューの最小質問

1. What did the AI judge, recommend, route, generate, or execute?  
   AIは何を判断、推奨、振り分け、生成、または実行したのか。
2. Which authority path was involved: account recovery, credential change, tool execution, production action, privileged API, rollback, or appeal removal?  
   どの権限経路が関与したのか。アカウント復旧、認証情報変更、ツール実行、本番操作、特権API、rollback、異議申立て手段の喪失が含まれるか。
3. Could an accountable human stop, suspend, reverse, or escalate the action before irreversible effect?  
   責任ある人間は、不可逆的影響の前に、その行為を停止、保留、撤回、またはエスカレーションできたのか。
4. What evidence is public, what is inferred, and what is missing?  
   何が公開証拠で、何が推定で、何が不足しているのか。
5. What conclusions must remain unresolved because internal logs, private records, or official findings are unavailable?  
   内部ログ、非公開記録、公式判断がないため、未解決として残すべき結論は何か。

## Safe public wording ｜ 安全な公開表現

Use this type of wording when facts are incomplete:

事実が不完全な場合は、次のような表現を使います。

> Public-source review only. This note does not claim access to internal logs, private incident records, official attribution, regulatory findings, or legal conclusions. It maps publicly visible actor, authority, and evidence questions under LUMINA-30.

> 公開情報レビューのみ。本メモは、内部ログ、非公開事故記録、公式な原因認定、規制上の判断、法的結論へのアクセスを主張しません。LUMINA-30の下で、公開上見えるActor、Authority、Evidenceの問いを整理するものです。

## How this connects to adoption review ｜ 採用審査との接続

For adoption review, this mapping helps teams ask whether an AI system is being introduced into an authority path where future incidents would become difficult to reconstruct or stop in time. If a public-source review cannot identify the responsible actor, authority path, evidence custodian, or refusal window, the same gap should be checked before deployment, procurement, or expanded access.

採用審査では、このマッピングにより、将来の事故を再構成したり時間内に止めたりすることが難しくなる権限経路へAIシステムが導入されようとしていないかを確認できます。公開情報レビューで、責任主体、権限経路、証拠管理者、拒否可能な時間窓を特定できない場合、同じ空白は、導入、調達、アクセス拡張の前にも確認すべきです。

## Practical template ｜ 実務テンプレート

After using this mapping guide, use the public-source review template to record sources, public facts, inferences, unknowns, authority paths, evidence gaps, and safe summary wording.

このマッピングガイドを確認した後は、公開情報レビュー・テンプレートを使って、情報源、公開事実、推定、不明点、権限経路、証拠ギャップ、安全な要約表現を記録します。

- [Public-Source Review Template](./Public_Source_Review_Template.md) ｜ [公開情報レビュー・テンプレートHTML](https://lumina-30.github.io/lumina30-incident-review/reference/Public_Source_Review_Template_ja.html)

## Limits ｜ 限界

This mapping does not create certification, approval, compliance status, official attribution, legal conclusion, safety guarantee, or proof of institutional adoption. It is a structured way to keep public-source incident review from becoming either speculation or mere output-error commentary.

このマッピングは、認証、承認、準拠状態、公式な原因認定、法的結論、安全保証、制度的採用の証拠を作るものではありません。公開情報ベースの事故レビューが、単なる推測や出力ミスだけの論評に落ちないようにするための構造化手段です。
