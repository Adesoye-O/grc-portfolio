# 02. ISO/IEC 27001:2022 Annex A Gap Analysis

**File:** [Westbridge-CC-ISO27001-Annex-A-Gap-Analysis.xlsx](./Westbridge-CC-ISO27001-Annex-A-Gap-Analysis.xlsx) (5 sheets)

All 93 Annex A controls assessed against current state, with a prioritised remediation plan.

## Context

The council has never operated a formal ISMS. Internal Audit reviewed ICT general controls in
2024, which covered maybe a fifth of the ground and all of it technical. Nothing has ever
assessed the organisational, people and physical controls.

The 2022 revision of the standard restructured 114 controls into 93 and introduced new ones
covering threat intelligence, cloud services, data masking, data leakage prevention and secure
coding. The council's existing policy is written against the 2013 version, so those controls
have no policy basis at all.

## Approach

Assessment ran from April to June 2026: 31 control owner interviews across ICT, Information
Governance, HR, Procurement, Property and Facilities and Legal Services, plus technical
configuration review and sample testing of leaver deprovisioning, access recertification, change
records and DSAR handling.

Every control got a maturity score on a CMMI-derived scale from 0 to 5, with 3 set as the
minimum target and 4 for anything rated Critical. Compliance status is separate from maturity
on purpose. Compliant requires the control to be documented, implemented, evidenced and
measured, so a control can be operating in practice and still not be compliant if nobody can
prove it.

Priority is assigned against a stated criterion rather than by feel. Critical means an
exploitable weakness with severe service, financial or data protection consequence, or a control
failure implicated in one of the two recent incidents.

## Findings

Eight controls compliant, 65 partial, 20 non-compliant. Average maturity 2.05 against a target
of 3.00.

| Theme | Controls | Compliant | Partial | Non-compliant | Avg maturity |
|---|---|---|---|---|---|
| A.5 Organizational | 37 | 4 | 26 | 7 | 2.03 |
| A.6 People | 8 | 2 | 6 | 0 | 2.63 |
| A.7 Physical | 14 | 1 | 13 | 0 | 2.43 |
| A.8 Technological | 34 | 1 | 20 | 13 | 1.79 |

Thirteen of the twenty non-compliant controls are technological. That concentration is the
finding, not the headline count.

The worst individual results are A.8.2 privileged access rights, A.8.20 networks security, A.8.15
logging, A.8.33 test information and A.8.12 data leakage prevention. Three of those five are
prerequisites for others, which is why the roadmap is sequenced rather than sorted by severity.

Remediation totals 1,748 officer days: 841 Critical, 681 High, 181 Medium, 45 Low. Spread across
Q4 2026 to Q3 2027, with the heaviest quarter at 586 days.

## Why only 8 compliant is the right answer

A reader who knows the standard will look at 8.6% compliance and assume the assessment was
written to be harsh, so the dashboard says plainly why it is not.

Compliant requires documented, implemented, evidenced and measured. An organisation that has
never run an ISMS will fail the fourth test almost everywhere, because measurement is the thing
nobody does until an auditor asks. Several controls here are operating perfectly well and are
still rated partial for that reason alone. A.7.2 physical entry works, but the data hall access
list had not been reviewed since 2023 and contained nine leavers.

The diagnostic measures are average maturity and the distribution of failures by theme, not the
compliant count. An assessment that inflated the compliant number to look reasonable would be
useless the first time anyone tested it.

## What is in the workbook

Cover and methodology sheets stating the maturity scale, status definitions, priority criteria,
evidence sources, assumptions and limitations. The limitation that matters: operational
technology was assessed by documentation review only, and commissioning a specialist OT
assessment is itself one of the remediation actions.

The gap analysis sheet carries all 93 controls with current state, status, maturity, target,
gap, remediation, owner, target quarter and effort. Filterable, with conditional formatting on
status and priority.

The dashboard calculates everything from the assessment sheet, so changing an assessment updates
the summary. The roadmap sheet holds the 68 Critical and High actions in delivery sequence with
dependencies noted, including which ones are blocked by procurement lead time and which need a
business case to Cabinet.

## What I would do differently

Effort estimates are internal officer days and exclude capital and supplier implementation cost,
which is stated but still unsatisfying. The network segmentation programme at 70 officer days is
the largest internal line, and the capital cost is the number that will actually decide whether
it happens.

I would also split A.8.20 into phases in the roadmap rather than carrying it as one item. It
spans three financial years and sitting in the plan as a single row makes the Q3 2027 column
look achievable when it is not.
