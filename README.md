# GRC Portfolio

Governance, risk and compliance deliverables, built end to end for one fictional UK local
authority.

These are the working documents themselves. A policy suite written for board approval, a
control gap analysis covering every control in the standard, a risk register with a stated
methodology, a supplier assessment with scored evidence, and a training programme with two
campaigns of results.

Adesoye Oloruntoba. Business and Solutions Analyst, System and Product Owner, IT Governance and
GRC. CGRC (ISC2).
[LinkedIn](https://www.linkedin.com/in/adesoyeo)

## Why a fictional council

Everything here concerns Westbridge County Council, an invented unitary authority in the East
Midlands. The council does not exist. I checked the name against the register of UK local
authorities before writing anything, and the systems, suppliers, officers, incident dates and
figures are all made up.

Real GRC work is confidential. A genuine gap analysis names exploitable weaknesses in live
systems, and no employer would let you publish one. So a portfolio built on real work is either
redacted into uselessness or it should not exist.

Inventing the organisation also had a benefit I did not expect. A real assessment inherits its
asset register, its risk appetite and its severity definitions from whoever set them up years
ago, and you can go a long way without ever questioning them. Here there was nothing to
inherit. Every number had to be chosen and then defended: the 4,750 staff, the 47 privileged
accounts, the secondary data centre sitting in Flood Zone 2, the 23.9% baseline phishing click
rate. Each one then had to stay consistent across five documents that reference each other.

[Full organisational profile](./westbridge-county-council.md)

## The artefacts

| # | Artefact | Format | What it covers |
|---|---|---|---|
| 01 | [Information Security Policy Suite](./01-security-policy-suite/) | Word | Four policies, plus the committee report that gets them adopted |
| 02 | [ISO/IEC 27001:2022 Annex A Gap Analysis](./02-iso27001-gap-analysis/) | Excel | All 93 controls assessed, scored and sequenced into a roadmap |
| 03 | [NIST SP 800-30 Risk Assessment and Register](./03-nist-risk-assessment/) | Excel | 28 assets, 12 threat sources, 32 risks, inherent and residual |
| 04 | [Third Party Vendor Risk Assessment](./04-third-party-risk-assessment/) | Excel | 66 questions, three suppliers scored against evidence |
| 05 | [Security Awareness and Phishing Programme](./05-security-awareness-programme/) | Word, Excel | Programme design, two campaigns of results, follow-up model |

## How they connect

These are five views of one organisation's security position rather than five separate
exercises sharing a letterhead. They reference each other on purpose.

Take the worst finding in the set. Sixteen of the council's forty-seven privileged accounts are
used for daily email and browsing, with no privileged access management anywhere.

In the gap analysis it is control A.8.2, rated non-compliant at maturity 1, with 45 officer days
of remediation scheduled for Q1 2027. In the risk register it is R-001, the only risk scored 25
at inherent level, because it is the shortest route from one phishing click to ransomware across
the whole estate. In the policy suite it is section 6 of the Access Control Policy, which sets
the standard the remediation is working towards. In the awareness programme it is Cohort 5: the
eleven privileged users who clicked or submitted credentials during simulations, who lose
standing privileged access straight away rather than waiting for the wider programme. In the
vendor assessment it is question Q4.4, where the council demands of its suppliers a control it
has not yet achieved itself.

Most GRC output fails for want of exactly this. The individual documents are usually fine. It is
the risk register, the policy and the remediation plan describing three different organisations
that does the damage.

## Findings

All figures are consistent across the five artefacts.

Of the 93 Annex A controls, 8 are compliant, 65 partial and 20 non-compliant. Average maturity
is 2.05 against a minimum target of 3.00, and thirteen of the twenty non-compliant controls sit
in the Technological theme. Remediation comes to 1,748 officer days over four quarters.

The corporate risk register holds 32 risks. At inherent level that is 12 Critical, 16 High and 4
Moderate. After the planned treatment it becomes 4 High, 27 Moderate and 1 Low, a 45% reduction
in aggregate score, with four risks still outside appetite and needing formal acceptance.

Three suppliers were assessed. One came out Moderate and renewable subject to contract
conditions. One came out Critical and is recommended for non-renewal, having failed 21 critical
controls and failed to disclose a ransomware incident that the assessment found through open
source research. The third came out High: good engineering, but training a model on live social
care data with no lawful basis established for that purpose.

Phishing click rate fell from 23.9% to 14.8% across two campaigns, reporting rose from 3.9% to
12.9%, and median time to first report dropped from 184 minutes to 36. The write-up argues this
is partial progress rather than success, because nearly all the improvement came on the easy
lures.

## Reading them

The Excel files carry live formulas, conditional formatting and data validation. GitHub will not
render them, so download them and open in Excel or LibreOffice. Each folder has a write-up
covering the context, the method, the findings and what I would do differently, so you can judge
the thinking without opening a file at all.

If you read one thing, read the
[gap analysis write-up](./02-iso27001-gap-analysis/). It explains why a first assessment that
rates only 8 of 93 controls compliant is the right answer rather than a harsh one.

## Scope

This is illustrative professional work. It is not advice, it describes no real organisation, and
it should not be used as a template for an actual compliance programme without assessing the
organisation it would be applied to.
