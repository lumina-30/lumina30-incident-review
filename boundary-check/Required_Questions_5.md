<!-- L30_LANG_LOCK: EN_JP_PAIRED -->
# Required Questions 5 ｜ 必須5問

## Purpose ｜ 目的

This file provides the shortest reusable question set for LUMINA-30 post-incident boundary review.

本ファイルは、LUMINA-30の事故後境界レビューで再利用しやすい最短の質問セットである。

## Required Questions ｜ 必須質問

1. Was human final refusal available before irreversible impact?
2. Was that refusal operationally effective, not merely nominal?
3. Are records sufficient to verify the refusal pathway?
4. If records are absent or unverifiable, should the case be treated as no effective refusal?
5. Did AI-generated output become the sole or primary rationale for final action?

1. 不可逆的影響の前に、人間の最終拒否は可能だったか。
2. その拒否は名目上ではなく、運用上実効的だったか。
3. 拒否経路を検証できる十分な記録は存在するか。
4. 記録が存在しない、または検証不能な場合、有効な拒否は存在しなかったものとして扱うべきか。
5. AI生成出力が、最終行為の唯一または主要な根拠になっていたか。


## Authority Routing Add-On ｜ 権限経路追加確認

The five questions above remain the shortest core set.  
For incidents involving AI agents, automation layers, privileged APIs, account recovery, credential changes, tool execution, production access, or rollback authority, add the following authority-routing questions before reaching a conclusion.

上記5問は、最短の中核質問セットとして維持する。  
AIエージェント、自動化層、特権API、アカウント復旧、認証情報変更、ツール実行、本番アクセス、またはロールバック権限を含むインシデントでは、結論前に以下の権限経路質問を追加する。

A1. Did the AI system, AI agent, platform automation layer, or privileged system have authority to initiate, approve, or execute account recovery, credential changes, tool execution, production actions, rollback suppression, or other irreversible operations?  
A2. Could a human actor stop the action before the AI-mediated process changed credentials, executed tools, modified production state, removed recovery options, or committed an irreversible operation?  
A3. Was rollback, suspension, credential reversal, account-recovery reversal, or production-state restoration available and assigned to an accountable human?  
A4. Are records sufficient to separate the human requester, AI assistant or agent, platform automation layer, privileged system or API, accountable organization, and any external attacker?  
A5. Did any AI-mediated step remove or weaken the affected human's ability to appeal, recover access, obtain evidence, or re-enter the review process?

A1. AIシステム、AIエージェント、プラットフォーム自動化層、または特権システムは、アカウント復旧、認証情報変更、ツール実行、本番操作、ロールバック抑制、またはその他の不可逆的操作を開始・承認・実行する権限を持っていたか。  
A2. AI媒介プロセスが認証情報を変更し、ツールを実行し、本番状態を変更し、復旧手段を除去し、または不可逆的操作を確定する前に、人間の主体はその行為を停止できたか。  
A3. ロールバック、停止、認証情報の差し戻し、アカウント復旧の差し戻し、または本番状態の復元は可能であり、責任ある人間に割り当てられていたか。  
A4. 人間の依頼者、AIアシスタントまたはエージェント、プラットフォーム自動化層、特権システムまたはAPI、責任組織、および外部攻撃者が存在する場合はその主体を分離できる十分な記録はあるか。  
A5. AI媒介ステップによって、影響を受ける人間の異議申立て、アクセス回復、証拠取得、またはレビュー過程への再参入能力が除去または弱体化されなかったか。

## Boundary Responsibility Add-On ｜ 境界責任追加確認

The five questions above remain the shortest core set.  
For cases involving optimization pressure, optimization-driven displacement, institutional lock-in, or responsibility diffusion, add the following responsibility questions before reaching a conclusion.

上記5問は、最短の中核質問セットとして維持する。  
最適化圧、最適化による置換、制度固定化、または責任拡散を含む事例では、結論前に以下の責任質問を追加する。

6. Who was responsible for designing the friction required to preserve effective refusal before irreversibility?
7. Who was responsible for operating that friction in practice?
8. Who was responsible for preserving evidence before affected humans lost voice, position, or re-entry capacity?
9. Who was responsible for verifying that the friction was effective and not merely nominal?
10. Who was responsible for correction if the boundary condition failed?

6. 不可逆化前に実効的拒否を保存するための摩擦を設計する責任主体は誰だったか。
7. その摩擦を実務上運用する責任主体は誰だったか。
8. 影響を受ける人間が声・地位・再参入能力を失う前に証拠を保存する責任主体は誰だったか。
9. その摩擦が名目的ではなく実効的だったことを検証する責任主体は誰だったか。
10. 境界条件が失敗した場合の是正責任主体は誰だったか。

## Recommended Answer Format ｜ 推奨回答形式

- Yes
- No
- Not Verifiable
- Evidence
- Reviewer note

- Yes
- No
- Not Verifiable
- 根拠
- レビュー担当者メモ

## Minimal Conclusion ｜ 最小結論

If any required question cannot be verified, the review should not claim that effective human refusal was demonstrated.

必須質問のいずれかが検証不能である場合、そのレビューは「実効的な人間の拒否が示された」と主張すべきではない。