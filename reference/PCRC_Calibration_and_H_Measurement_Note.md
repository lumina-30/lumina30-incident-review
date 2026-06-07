<!-- L30_LANG_LOCK: EN_JP_PAIRED -->

# PCR-C Calibration and H-Measurement Note

> Canonical bilingual Markdown source. The English and Japanese HTML files are reader-facing views generated from this paired source structure.
> 正本の日英併記Markdownです。英語HTMLと日本語HTMLは、この正本構造に対応する読者向け表示版です。

---

## English

## PCR-C Calibration and H-Measurement Note

This note defines how PCR-C threshold values and intervention capacity H should be interpreted in operational review contexts.

PCR-C thresholds are not empirically fixed constants.  
They are normalized reference levels used to trigger staged review and control actions.

The purpose of this note is to prevent two errors:

1. treating PCR-C thresholds as universal empirical risk constants;  
2. treating the absence of direct empirical calibration as a reason to ignore intervention-capacity failure.

---

### 1. Status

PCR-C is a structural control framework, not an empirical prediction model.

The threshold values:

- YELLOW = 5
- ORANGE = 7
- RED = 9

should be read as normalized reference exposure levels within a bounded scoring model.

They indicate when review, throttling, isolation, or cutoff should be considered.  
They do not claim that all systems become unsafe at identical numerical values.

---

### 2. Calibration Principle

PCR-C calibration should be performed relative to the operational environment.

At minimum, calibration should consider:

- historical baseline variance;
- deployment speed;
- privilege expansion rate;
- infrastructure coupling;
- human approval latency;
- stop-command propagation delay;
- rollback feasibility;
- audit visibility;
- cross-region or distributed execution behavior;
- restart governance strength.

A system with faster execution, broader connectivity, higher privilege, or weaker human response capacity should use stricter thresholds.

---

### 3. Intervention Capacity H

In PCR-C, H denotes effective intervention capacity.

H is not a single directly observable quantity.  
It represents the practical ability of humans and institutions to detect, decide, stop, isolate, or reverse a system pathway before irreversible impact.

H should be treated as a bounded operational estimate, not as a precise physical constant.

---

### 4. Proxy Measurements for H

H may be approximated using repeated operational measurements, including:

| Proxy | What it measures |
|---|---|
| Detection latency | Time required to detect escalation or boundary-relevant behavior |
| Approval-chain latency | Time required for authorized humans to decide and issue stop action |
| Stop-command propagation delay | Time required for stop/isolation commands to reach relevant infrastructure |
| Rollback feasibility | Whether system state can be restored or contained after intervention |
| Privilege freeze time | Time required to prevent additional permission or tool expansion |
| Cross-region synchronization delay | Time required to enforce containment across distributed infrastructure |
| Audit-log availability | Whether reviewers can verify what happened before intervention |
| Restart governance delay | Time and authority required before the system can resume operation |

These measurements do not prove that H is exact.  
They provide operational bounds for assessing whether human refusal authority is still effective.

---

### 5. Stop-Drill Method

A stop-drill is a controlled exercise used to estimate whether humans can still intervene before escalation becomes irreversible.

A minimal stop-drill should record:

1. detection time;
2. escalation classification time;
3. decision authorization time;
4. command execution time;
5. infrastructure propagation time;
6. confirmation time;
7. rollback or isolation status;
8. audit-log completeness.

If these values exceed the expected escalation window, effective intervention capacity should be treated as degraded.

---

### 6. Threshold Adjustment Rule

PCR-C thresholds should be adjusted downward when:

- execution speed increases;
- autonomous tool access expands;
- privilege levels increase;
- deployment becomes distributed;
- audit visibility decreases;
- human approval paths become slower;
- rollback becomes uncertain;
- previous stop-drills fail or exceed expected escalation windows.

PCR-C thresholds may be treated as less restrictive only when repeated stop-drills show that detection, decision, containment, and verification remain effective within the relevant escalation window.

---

### 7. Review Interpretation

A PCR-C review should not ask:

“Are the numbers 5, 7, and 9 empirically universal?”

It should ask:

“Given this system’s capability, connectivity, privilege, speed, and measured intervention capacity, were humans still able to refuse or stop the pathway before irreversible impact?”

If this cannot be demonstrated, the review should treat effective human refusal as not verified.

---

### 8. Relationship to LUMINA-30

This note does not modify the LUMINA-30 canonical boundary.

It operationalizes one measurement question:

Can effective human refusal be exercised before irreversible AI-related impact?

PCR-C provides the infrastructure-layer scoring and gating model.  
LUMINA-30 provides the boundary condition: human refusal must remain effective before irreversibility.

---

### 9. Non-Guarantee

PCR-C calibration does not guarantee safety.

It provides a structured method for identifying when human intervention capacity may be falling behind system amplification.

A calibrated PCR-C review strengthens procedural visibility, but it does not replace alignment research, legal compliance, institutional governance, security evaluation, or incident investigation.

---

## 日本語

本ノートは、PCR-Cの閾値と介入能力Hを、運用レビューの文脈でどのように解釈すべきかを定義する。

PCR-Cの閾値は、経験的に固定された定数ではない。  
段階的レビューおよび制御行動を開始するための、正規化された参照水準である。

本ノートの目的は、次の2つの誤りを防ぐことである。

1. PCR-Cの閾値を、普遍的な経験的リスク定数として扱うこと。
2. 直接的な経験的校正が存在しないことを理由に、介入能力の失敗を無視すること。

---

### 1. 状態

PCR-Cは構造的制御フレームワークであり、経験的予測モデルではない。

閾値は以下のとおりである。

- 黄色 = 5
- 橙色 = 7
- 赤色 = 9

これらは、境界づけられたスコアリングモデル内の正規化された参照露出水準として読むべきである。

これらは、レビュー、スロットリング、隔離、または切断を検討すべき時点を示す。  
すべてのシステムが同一の数値で危険になると主張するものではない。

---

### 2. 校正原則

PCR-Cの校正は、運用環境に対して相対的に行うべきである。

少なくとも、校正では以下を考慮する。

- 過去の基準変動幅
- 展開速度
- 権限拡張率
- インフラ結合
- 人間承認の遅延
- 停止命令の伝播遅延
- ロールバック可能性
- 監査可視性
- 地域横断または分散実行の挙動
- 再起動統治の強度

実行が速く、接続範囲が広く、権限が高く、または人間側の応答能力が弱いシステムでは、より厳しい閾値を使用すべきである。

---

### 3. 介入能力H

PCR-Cにおいて、Hは実効的な介入能力を表す。

Hは単一の直接観測可能な量ではない。  
不可逆的影響の前に、人間および制度がシステム経路を検知、判断、停止、隔離、または反転できる実際的能力を表す。

Hは精密な物理定数ではなく、境界づけられた運用推定値として扱うべきである。

---

### 4. Hの代理測定

Hは、以下を含む反復的な運用測定によって近似できる。

| 代理指標 | 測定対象 |
| --- | --- |
| 検知遅延 | エスカレーションまたは境界関連挙動を検知するために必要な時間 |
| 承認連鎖の遅延 | 権限ある人間が判断し、停止行動を発行するために必要な時間 |
| 停止命令の伝播遅延 | 停止または隔離命令が関連インフラへ到達するために必要な時間 |
| ロールバック可能性 | 介入後にシステム状態を復元または封じ込められるか |
| 権限凍結時間 | 追加の許可またはツール拡張を防ぐために必要な時間 |
| 地域横断同期遅延 | 分散インフラ全体で封じ込めを強制するために必要な時間 |
| 監査ログ利用可能性 | 介入前に何が起きたかをレビュー担当者が検証できるか |
| 再起動統治遅延 | システムが運用再開できるまでに必要な時間と権限 |

これらの測定は、Hが正確であることを証明しない。  
人間の拒否権限がなお実効的かを評価するための運用上の境界を提供する。

---

### 5. 停止訓練法

停止訓練とは、エスカレーションが不可逆化する前に人間がなお介入できるかを推定するための管理された演習である。

最小限の停止訓練では、以下を記録すべきである。

1. 検知時間
2. エスカレーション分類時間
3. 判断承認時間
4. 命令実行時間
5. インフラ伝播時間
6. 確認時間
7. ロールバックまたは隔離状態
8. 監査ログの完全性

これらの値が想定されるエスカレーション窓を超える場合、実効的介入能力は劣化しているものとして扱うべきである。

---

### 6. 閾値調整規則

PCR-Cの閾値は、以下の場合に引き下げるべきである。

- 実行速度が増す場合
- 自律的なツールアクセスが拡大する場合
- 権限水準が上がる場合
- 展開が分散化する場合
- 監査可視性が下がる場合
- 人間の承認経路が遅くなる場合
- ロールバックが不確実になる場合
- 過去の停止訓練が失敗する、または想定エスカレーション窓を超える場合

PCR-Cの閾値を緩く扱えるのは、反復的な停止訓練によって、検知、判断、封じ込め、検証が関連するエスカレーション窓内でなお実効的であることが示される場合に限られる。

---

### 7. レビュー上の解釈

PCR-Cレビューは、次の問いを立てるべきではない。

「5、7、9という数値は経験的に普遍か。」

問うべきなのは、次である。

「このシステムの能力、接続性、権限、速度、および測定された介入能力を前提として、人間は不可逆的影響の前にその経路を拒否または停止できたか。」

これを示せない場合、レビューでは実効的な人間拒否は検証されていないものとして扱うべきである。

---

### 8. LUMINA-30との関係

本ノートは、LUMINA-30の正典的境界を変更しない。

本ノートは、1つの測定問いを運用化する。

不可逆的なAI関連影響の前に、実効的な人間拒否を行使できるか。

PCR-Cは、インフラ層のスコアリングおよびゲーティングモデルを提供する。  
LUMINA-30は境界条件を提供する。すなわち、人間の拒否は不可逆化の前に実効的でなければならない。

---

### 9. 非保証

PCR-Cの校正は安全を保証しない。

PCR-Cの校正は、人間の介入能力がシステムの増幅に遅れ始め得る時点を特定するための構造化された方法を提供する。

校正済みPCR-Cレビューは手続き上の可視性を強化するが、アライメント研究、法令遵守、制度的ガバナンス、セキュリティ評価、またはインシデント調査を置き換えるものではない。
