# 04. Third Party Vendor Risk Assessment

**File:** [Westbridge-CC-Third-Party-Vendor-Risk-Assessment.xlsx](./Westbridge-CC-Third-Party-Vendor-Risk-Assessment.xlsx) (8 sheets)

A 66-question due diligence questionnaire across 11 weighted domains, with three suppliers
assessed, scored and rated.

## Context

The council's old rule was that suppliers above £100,000 had to hold Cyber Essentials. Nothing
else was assessed. That threshold is the reason this artefact exists, because contract value has
almost no relationship to data risk.

One of the three suppliers here sits below the threshold and had never been assessed. It handles
the names, addresses and account details of 198,000 households.

## Approach

Each question scores 0 to 3, with N/A removed from both numerator and denominator so a supplier
is not penalised for a control that does not apply to the service it provides. Domain scores are
weighted, with data protection and privacy highest at 15% because the council stays the
controller and keeps the liability whatever the contract says.

Twenty-one questions are flagged as critical controls. These drive an override: one or two
failures cap the assurance band at Adequate, three to nine cap it at Weak, ten or more at
Inadequate. The override only ever lowers a band.

The graduation is deliberate. A binary override would treat a supplier with 94.6% and two
contractual gaps the same as one failing twenty-one critical controls, and that model would not
survive challenge at contract award. The scoring sheet states this reasoning in the workbook,
because a supplier that gets rated down is entitled to see the rule.

The final rating combines the assurance band with inherent criticality, which is assessed
independently of anything the supplier says. Criticality comes from data classification, the
number of people affected and the criticality of the service supported.

Scores are not the supplier's self-assessment. Every answer carries an assessor comment naming
the evidence reviewed, and where evidence did not support the claim the score was lowered and
the comment says why.

## Findings

| | Vendor A, Arlington Care Systems | Vendor B, Halgate Print | Vendor C, Quantus Analytics |
|---|---|---|---|
| Service | Social care case management (SaaS) | Bulk print and mail | AI demand forecasting (pilot) |
| Data | 86,000 special category records | 198,000 households | Special category, pilot |
| Inherent criticality | Critical | High | Critical |
| Assurance score | 94.6% | 19.3% | 69.6% |
| Critical control failures | 2 | 21 | 9 |
| Band after override | Adequate | Inadequate | Weak |
| **Final rating** | **Moderate** | **Critical** | **High** |

Vendor A is the strongest and is renewable subject to three contract conditions. Certification
scope was verified against the service actually supplied rather than accepted at face value,
which is the check most often skipped. The two gaps are a missing exit plan and a subprocessor
clause giving notice but no right to object.

Vendor B should not be renewed. Data for 198,000 households sits unencrypted on a production
file server and on an unencrypted USB drive that leaves site weekly. No logging, no monitoring,
no vulnerability management, an out-of-support operating system, no incident response plan. The
supplier declared no incidents, and open source research found an industry press report of a
2024 ransomware incident at its facility, which the supplier described as an IT outage when
questioned.

Vendor C is the interesting one. Encryption, identity, pipeline security and backup are better
than several larger suppliers. But council social care data is being used to train the
forecasting model, which the supplier disclosed openly and regards as inherent to the service.
No separate lawful basis has been established for training as a distinct purpose, the supplier
cannot explain how council data would be removed from an already-trained model, and live data
sits in the development environment. The recommendation is suspend and remediate rather than
terminate, because the capability has value and the supplier was candid.

## Why Vendor B is the point of the exercise

Vendor B is the cheapest contract in the set, the least technically interesting, and by a long
way the biggest risk. It went unassessed for three years because the rule looked at the wrong
number.

The undisclosed incident is what turns this from a weak supplier into an unusable one. Whether
it was misunderstanding or concealment, the council cannot rely on this supplier's
self-declarations, and every control that depends on the supplier telling you something has
failed.

## What is in the workbook

Scoring model sheet with the response scale, domain weightings and rationale, the calculation
method, assurance bands and the final rating matrix. The questionnaire itself, with critical
controls flagged and evidence requirements stated per question. Three response sheets carrying
supplier profile, all 66 scored answers with assessor commentary, domain roll-up and the final
rating chain. A comparison sheet with domain-by-domain scores and written conclusions and
recommendations for each supplier.

## What I would do differently

Sixty-six questions is too many for a low-criticality supplier. The questionnaire should branch:
a 20-question tier for suppliers handling no personal data, the full set above that. As drafted
it would get filled in badly by small suppliers, and badly filled in is worse than not asked.

Eleven weighted domains also produce a number with more precision than the underlying judgement
supports. Vendor C at 69.6% versus a Weak threshold of 70% is a 0.4-point difference deciding a
band, and nothing in the evidence justifies that resolution. The critical control override saves
it here, which is partly luck.
