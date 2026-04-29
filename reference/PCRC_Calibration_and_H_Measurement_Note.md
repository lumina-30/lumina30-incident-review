# PCR-C Calibration and H-Measurement Note

This note defines how PCR-C threshold values and intervention capacity H should be interpreted in operational review contexts.

PCR-C thresholds are not empirically fixed constants.  
They are normalized reference levels used to trigger staged review and control actions.

The purpose of this note is to prevent two errors:

1. treating PCR-C thresholds as universal empirical risk constants;  
2. treating the absence of direct empirical calibration as a reason to ignore intervention-capacity failure.

---

## 1. Status

PCR-C is a structural control framework, not an empirical prediction model.

The threshold values:

- YELLOW = 5
- ORANGE = 7
- RED = 9

should be read as normalized reference exposure levels within a bounded scoring model.

They indicate when review, throttling, isolation, or cutoff should be considered.  
They do not claim that all systems become unsafe at identical numerical values.

---

## 2. Calibration Principle

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

## 3. Intervention Capacity H

In PCR-C, H denotes effective intervention capacity.

H is not a single directly observable quantity.  
It represents the practical ability of humans and institutions to detect, decide, stop, isolate, or reverse a system pathway before irreversible impact.

H should be treated as a bounded operational estimate, not as a precise physical constant.

---

## 4. Proxy Measurements for H

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

## 5. Stop-Drill Method

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

## 6. Threshold Adjustment Rule

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

## 7. Review Interpretation

A PCR-C review should not ask:

“Are the numbers 5, 7, and 9 empirically universal?”

It should ask:

“Given this system’s capability, connectivity, privilege, speed, and measured intervention capacity, were humans still able to refuse or stop the pathway before irreversible impact?”

If this cannot be demonstrated, the review should treat effective human refusal as not verified.

---

## 8. Relationship to LUMINA-30

This note does not modify the LUMINA-30 canonical boundary.

It operationalizes one measurement question:

Can effective human refusal be exercised before irreversible AI-related impact?

PCR-C provides the infrastructure-layer scoring and gating model.  
LUMINA-30 provides the boundary condition: human refusal must remain effective before irreversibility.

---

## 9. Non-Guarantee

PCR-C calibration does not guarantee safety.

It provides a structured method for identifying when human intervention capacity may be falling behind system amplification.

A calibrated PCR-C review strengthens procedural visibility, but it does not replace alignment research, legal compliance, institutional governance, security evaluation, or incident investigation.
