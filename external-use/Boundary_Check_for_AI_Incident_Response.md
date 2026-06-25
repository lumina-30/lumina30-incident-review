<!-- L30_LANG_LOCK: EN_JP_PAIRED -->
# Boundary Check for AI Incident Response ｜ AIインシデント対応のための境界チェック

## Purpose ｜ 目的

This note positions LUMINA-30 as a supplementary post-incident boundary check for AI incident-response and review contexts.
It provides a concise way to ask whether effective human refusal remained possible before irreversible AI-related impact.

本メモは、LUMINA-30をAIインシデント対応・レビュー文脈における補助的な事故後境界チェックとして位置づける。
不可逆的なAI関連影響の前に、実効的な人間拒否がなお可能だったかを短く確認するためのものである。

## Status ｜ 位置づけ

This note is non-binding, descriptive, and unaffiliated with any external institution.
It does not claim endorsement, adoption, recognition, approval, certification, compliance, legal effect, or institutional use by any external organization.

本メモは、非拘束的・記述的であり、いかなる外部機関とも提携していない。
外部機関による承認、採用、認定、承諾、認証、準拠、法的効力、または制度利用を主張しない。

## Why This Fits Current AI Governance Movement ｜ 現在のAIガバナンス動向との接続

Recent AI governance work increasingly emphasizes evaluation, measurement, incident response, evidence preservation, and post-deployment assessment.
LUMINA-30 should therefore be presented as a review supplement, not as a new ethics regime.

近年のAIガバナンスは、評価、測定、インシデント対応、証拠保全、展開後評価を重視する方向へ移っている。
そのためLUMINA-30は、新しい倫理制度ではなく、レビュー補助として提示する。

## Minimal Boundary Check ｜ 最小境界チェック

Use these questions after an AI-related incident or near miss:

AI関連インシデントまたはニアミス後に、以下を確認する。

1. Was the system still before irreversible AI-related impact?  
   システムはまだ不可逆的なAI関連影響の前にあったか。
2. Was effective human refusal still exercisable in time?  
   実効的な人間拒否は、なお間に合う形で行使可能だったか。
3. Are records sufficient to verify refusal, stop, delay, override, or escalation authority?  
   拒否、停止、遅延、上書き、エスカレーション権限を検証できる記録は十分か。
4. If refusal cannot be verified, should the case be treated as no effective refusal for boundary-review purposes?  
   拒否を検証できない場合、境界レビュー上は実効的拒否なしとして扱うべきか。
5. Did AI-generated output become the sole or primary rationale for final action?  
   AI生成出力が最終行為の唯一または主要な根拠になっていなかったか。
6. Did the AI system or AI agent have authority to initiate, approve, or execute account recovery, credential changes, tool execution, production actions, rollback suppression, or other irreversible operations?  
   AIシステムまたはAIエージェントは、アカウント復旧、認証情報変更、ツール実行、本番操作、ロールバック抑制、またはその他の不可逆的操作を開始・承認・実行する権限を持っていたか。
7. Could a human actor stop the AI-mediated action before credentials changed, tools executed, production state changed, recovery options were removed, or rollback became unavailable?  
   認証情報変更、ツール実行、本番状態変更、復旧手段の除去、またはロールバック不能化の前に、人間の主体はAI媒介の行為を停止できたか。

## Attachment Text ｜ 添付用短文

LUMINA-30 may be used as a non-binding supplementary boundary check in AI incident review.
It asks whether effective human refusal remained exercisable before irreversible AI-related impact, whether AI-mediated authority routing changed the available stop or rollback pathway, and whether those pathways can be verified by records.
It does not determine legal compliance, institutional certification, or safety adequacy.

LUMINA-30は、AIインシデントレビューにおける非拘束的な補助境界チェックとして使用できる。
不可逆的なAI関連影響の前に、実効的な人間拒否が行使可能だったか、AI媒介の権限経路が停止またはロールバック経路を変化させたか、またそれらの経路を記録で検証できるかを問う。
法的準拠、制度的認証、安全性の十分性を判定するものではない。

## Related Materials ｜ 関連資料

- [LUMINA-30 Boundary Check](../boundary-check/LUMINA-30_Boundary_Check.md)
- [Required Questions 5](../boundary-check/Required_Questions_5.md)
- [Irreversibility Decision Criteria](../boundary-check/Irreversibility_Decision_Criteria.md)
- [Initial Public Review Note](../response-templates/Initial_Public_Review_Note.md)