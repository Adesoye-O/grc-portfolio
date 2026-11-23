# 03. NIST SP 800-30 Risk Assessment and Register

**File:** [Westbridge-CC-NIST-Risk-Assessment-and-Register.xlsx](./Westbridge-CC-NIST-Risk-Assessment-and-Register.xlsx) (7 sheets)

A risk assessment conducted under NIST SP 800-30 Rev.1, with risks mapped to NIST CSF 2.0 and
cross-referenced to the Annex A controls that treat them.

## Context

The council maintains a corporate risk register through Internal Audit, but information security
appears on it as a single line reading "cyber attack". That is not a risk, it is a category, and
it cannot be owned, treated or measured.

This assessment produces the register that line should have pointed to.

## Approach

SP 800-30 gives four steps: prepare, conduct, communicate, maintain. The prepare step matters
most and is the one usually skipped. Scope, purpose, assumptions and constraints were agreed
with the SIRO before anything was assessed, along with the council's risk appetite and
tolerance.

Appetite is stated as averse for personal data protection and statutory service delivery,
cautious for everything else. Tolerance is a residual score of 9 or below. Ten to fourteen needs
documented SIRO acceptance, fifteen or above needs Audit and Governance Committee acceptance
with a time-limited plan. Those thresholds decide what the register means, and without them a
score of 12 is just a number.

Likelihood and impact are both scored 1 to 5. The impact scale is defined across five dimensions
at once: service delivery, harm to individuals, financial, legal and regulatory, and reputation.
A risk takes the highest dimension that applies. That is what stops every risk drifting to a 5,
because a reader can check the claim against the definition.

Threat sources come from SP 800-30 Appendix D, characterised by capability, intent and
targeting, with a column explaining why each one is relevant to this council specifically.
Vulnerabilities come from the gap analysis, so the two documents share a single source of truth.

## A note on inherent risk

Inherent risk here is assessed after existing controls, not before them. That is a departure
from the textbook definition and the methodology sheet says so.

A true control-free inherent score is a theoretical number nobody can act on, and when you put
it in front of elected members it makes the organisation look negligent in a way that is not
accurate. Assessing after existing controls but before the proposed treatment shows members what
the investment actually buys. Existing controls are listed for every risk so the reader can see
what is already credited.

## Findings

Thirty-two risks on the register.

| Band | Inherent | Residual | Movement |
|---|---|---|---|
| Critical (15 to 25) | 12 | 0 | −12 |
| High (10 to 14) | 16 | 4 | −12 |
| Moderate (5 to 9) | 4 | 27 | +23 |
| Low (1 to 4) | 0 | 1 | +1 |

Aggregate inherent score 435, residual 239, a 45% reduction. Mean inherent 13.59, mean residual
7.47.

Twelve risks currently need Committee acceptance and sixteen need SIRO acceptance. Four remain
outside tolerance even after full treatment, which is the honest answer rather than a failure of
the plan. R-001, privileged account compromise leading to estate-wide ransomware, is the only
risk scored 25, and its residual is 10 because you cannot engineer that one down to moderate.

By CSF function, PROTECT holds 19 of the 32 risks and 318 of the 435 inherent points. GOVERN
holds five, including the one I think is most often missed: R-032, where the aggregate risk
accepted through informal policy exceptions is unknown to the SIRO, so the council's stated risk
position is wrong by an unknown margin.

There are no Low inherent risks, and the methodology explains why. Risks scoring below 5 are
managed in directorate registers and never escalate to the corporate one.

## What is in the workbook

Twenty-eight assets with confidentiality, integrity and availability rated separately, plus
tier, hosting, Information Asset Owner and scale. Twelve threat sources. The register itself
carries 23 columns including threat event, vulnerability, existing controls, both score sets,
treatment strategy, planned treatment, owner, linked Annex A controls, target date and review
frequency.

Dual heat maps, inherent and residual side by side, both calculated live from the register.
Aggregate measures including the counts requiring each level of acceptance. A treatment plan
sheet ordered by inherent score.

## What I would do differently

Review frequencies range from weekly to annually and I set them per risk, which is correct in
principle and will not survive contact with reality. Thirty-two risks at mixed cadences needs a
tracking mechanism the council does not have, and within two quarters the monthly ones will be
getting reviewed quarterly like everything else. I would set three tiers and accept the loss of
precision.

The residual scores are forecasts, which the workbook states clearly in two places. I would go
further and add a column recording the date each residual was actually verified, because an
unverified residual reported to members as achieved is the most likely way this document becomes
misleading.
