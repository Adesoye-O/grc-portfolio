# 05. Security Awareness and Phishing Simulation Programme

**Files:**
[Westbridge-CC-Security-Awareness-Programme.docx](./Westbridge-CC-Security-Awareness-Programme.docx) (10 pages) ·
[Westbridge-CC-Phishing-Simulation-Results.xlsx](./Westbridge-CC-Phishing-Simulation-Results.xlsx) (5 sheets)

Programme design, two campaigns of simulation results, and a follow-up model that distinguishes
clicking a link from handing over a credential.

## Context

The council spends most of its security budget on technology. Both of its incidents began with a
person: a phishing message opened in November 2025, a credential entered into a fraudulent
sign-in page in March 2026.

Existing provision was a twenty-minute e-learning module assigned once a year. Completion was
64%. The content had not been updated since 2023 and did not mention the Report Phishing button,
which is the council's primary detection mechanism. Elected members, casual workers and agency
staff were out of scope entirely.

## Approach

The programme is built on one proposition, stated at the top of the document: the objective is
not to stop people clicking. People will always click. The objective is to make reporting fast,
normal and free of consequence, so the council hears about an attack in minutes rather than
hours.

That changes what gets measured. Report rate and time to first report lead the metrics, and
click rate follows. A single click is one endpoint to investigate. An unreported campaign
running three hours across 4,600 mailboxes is an incident.

Six measures with baselines and targets, including one deliberately awkward addition: real
reports per 100 workers per month, separate from simulation performance. A rising count of real
reports means the programme is working. A programme that improves simulation numbers while real
reporting stays flat has taught people to pass a test.

## Simulation design

Quarterly, four scenarios per campaign at graded difficulty, randomised so nobody gets the same
scenario twice in a year and difficulty stays comparable between campaigns.

Scenarios come from lures the council has actually received rather than vendor templates,
because generic templates train people to spot generic templates.

Two rules were set with the trade unions and are stated in the document. Individual results are
visible only to the IT Security Manager and one analyst, with everything above that reported by
directorate and cohort. And no simulation uses a lure relating to redundancy, pay cuts,
disciplinary action, bereavement or a safeguarding emergency. Those cause real distress and the
reputational cost outweighs the training value.

## Results

| Measure | June 2026 | September 2026 | Movement |
|---|---|---|---|
| Delivered | 4,576 | 4,592 | |
| Clicked | 1,093 (23.9%) | 681 (14.8%) | −9.1 pts |
| Credentials submitted | 426 (9.3%) | 190 (4.1%) | −5.2 pts |
| Reported | 178 (3.9%) | 594 (12.9%) | +9.0 pts |
| Report-to-click ratio | 0.16 | 0.87 | +0.71 |
| Median time to first report | 184 min | 36 min | −148 min |
| Training completion | 64% | 89.1% | +25.1 pts |

## What the results actually show

The headline improvement is narrower than the aggregate suggests, and the document says so
rather than presenting the fall in click rate as a win.

Nearly all the reduction came from the two easy commodity lures. The delivery failure notice
fell from 18.4% to 10.2% and the generic password expiry notice from 27.7% to 16.5%. The pay
award scenario, timed two days after the real pay award announcement with internal-looking
branding and no spelling errors, fell only from 31.5% to 20.7%. That scenario is the closest
approximation to how the council would really be attacked. Staff are learning to recognise badly
made phishing.

The report rate is where the programme genuinely worked, and tripling it while cutting time to
first report by five sixths is worth more operationally than the fall in click rate.

Eleven holders of privileged access clicked or submitted credentials across the two campaigns.
Sixteen of the council's forty-seven privileged accounts are used for daily email and browsing,
so a single successful harvest against this group is the shortest path to R-001 on the risk
register. The recommendation is to strip standing privileged access from those eleven now rather
than waiting for the wider programme.

Elected members recorded the worst click rate in both campaigns, 36.4% then 25.4%, while sitting
outside the training framework and holding no confidentiality undertaking beyond the Code of
Conduct. That is a governance gap, and the Monitoring Officer rather than HR needs to own it.

## The follow-up model

Seven cohorts, scaled to what someone actually did. Single clickers get the four-minute
point-of-click micro-learning and nothing further. Repeat clickers get an instructor-led
session. Credential submitters get a workshop. Repeat submitters get one-to-one coaching plus a
review of whether their role needs the access it holds.

Cohort 5 is the only one where a technical consequence follows a simulation result: privileged
users lose standing privileged access. The unions agreed it on the basis that it removes a
privilege rather than applies a sanction, and that the gap analysis had already recommended
removing that privilege from everyone.

No simulation result goes on a personnel file, into an appraisal or into a disciplinary process.

## What I would do differently

The 98% completion target is wrong. It sounds rigorous and it will drive gaming, because the
last 2% are long-term sick, on maternity leave or working a rota that does not touch a desk.
Managers will complete modules on their behalf to clear the report. I would set 95% and chase
the remainder individually.

The quarterly cadence is also probably too frequent at this maturity. Four campaigns a year
against a workforce that had never had one produces fatigue before it produces habit, and the
second campaign already shows some evidence of recognition rather than detection. I would run
three in year one.
