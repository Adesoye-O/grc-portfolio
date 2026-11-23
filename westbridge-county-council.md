# Westbridge County Council

Every artefact in this portfolio concerns this organisation. It does not exist. I checked the
name against the register of UK local authorities before writing anything, and no council,
borough, district or parish of this name is in use.

This page holds the shared context the five artefacts draw on. I wrote it first. Without it the
artefacts would have drifted: the asset register would have named systems the risk assessment
never mentioned, and the policy suite would have set standards for an estate nobody had defined.

## The council

A unitary authority in the East Midlands.

| | |
|---|---|
| Population served | 412,000 |
| Workforce | 4,750 employees, plus around 380 contractors |
| Gross revenue budget | £684m (2026/27) |
| Headquarters | County Hall, Westbridge |
| Estate | 3 area offices, 27 libraries, 4 highways depots, 11 children's homes |
| Data centres | County Hall (primary, 210 servers), Marchwood (secondary, 62 servers) |

Services: adult social care, children's services, highways and transport, waste, planning,
revenues and benefits, libraries, public health, trading standards and licensing, electoral
services, emergency planning.

## Governance

| Role | Holder |
|---|---|
| Chief Executive | Dr Miriam Chowdhury |
| Executive Director Corporate Services (SIRO) | Paul Ackroyd |
| Director of Finance (s151 Officer) | Nadia Rahman |
| Monitoring Officer | Stephen Vale |
| Director of Adult Social Care (Caldicott Guardian) | Dr Angela Moss |
| Head of ICT and Digital | Laura Kinsella |
| IT Security Manager | Dominic Ofori |
| Data Protection Officer | Helen Bright |
| Head of HR and Organisational Development | Karen Duffy |
| Head of Procurement | Sanjay Bhatt |
| Head of Property and Facilities | Ian Marsh |
| Head of Applications | Tom Reidy |
| Head of Highways | Marcus Bell |

Decision-making bodies: Audit and Governance Committee (member-level assurance), Corporate
Leadership Team, Information Governance Board.

The role structure is deliberately realistic. SIRO, Caldicott Guardian, Monitoring Officer and
s151 Officer are statutory or quasi-statutory positions in English local government, and several
of the artefacts turn on which of them can approve what. The Data Protection Officer's
independence is written into the incident response policy for the same reason: the decision to
notify the ICO cannot be overridden by the Chief Executive, and a policy that leaves that
ambiguous will fail at the worst possible moment.

## Technology estate

Identity and platform: Microsoft 365 (E3, with 400 E5 seats), Entra ID in hybrid configuration
with on-premises Active Directory, an Azure landing zone in UK South.

There are 140 line-of-business applications, 62 of them SaaS. These recur across the artefacts:

| Asset ID | System | Purpose |
|---|---|---|
| AST-01 | ARIA | Adult and children's social care case management (SaaS) |
| AST-02 | LEDGER-X | ERP: finance, HR, payroll |
| AST-03 | REVX | Revenues and benefits |
| AST-05 | WestbridgeOne | Public website, forms, payments, customer account |
| AST-10 | TRAFFICNET | Traffic signal control, operational technology |
| AST-12 | | Public space CCTV, 428 cameras |
| AST-17 | | 42TB of legacy unstructured shared drives |
| AST-20 | | Electoral management system |

Endpoints: 3,800 managed laptops, 1,400 mobile devices, 84 unmanaged field devices.

Security function: an IT Security Manager and two analysts. Managed detection and response
covers endpoint telemetry only, 08:00 to 18:00 Monday to Friday. That is 50 hours of each
168-hour week, which turns out to matter.

## Compliance obligations

UK GDPR and the Data Protection Act 2018. The Caldicott Principles for social care. PCI DSS for
card payments. The Freedom of Information Act 2000. The Local Government Transparency Code. The
Public Sector Bodies Accessibility Regulations. The Surveillance Camera Code. NHS Data Security
and Protection Toolkit obligations arising from health data sharing.

## Incident history

Two events run through the artefacts, and several findings exist because of them.

November 2025, ransomware deployment attempt. Contained before encryption. Escalated eleven
hours after the first indicator, because no out-of-hours security escalation path existed. The
activity began at 02:40 on a Saturday, outside the monitoring window.

March 2026, credential compromise. A Revenues and Benefits account was compromised through a
phishing message. The affected device was reimaged within three hours, which destroyed the
evidence needed to establish how entry was obtained. The ICO notification went out without being
able to describe the initial access vector.

Those are why the incident response policy mandates evidence preservation before rebuild, and
why forensic readiness appears as a non-compliant control rather than a theoretical gap.

## Why the profile has this shape

I designed the council to be averagely bad rather than catastrophically so, because that is the
harder and more realistic case.

It has a real security function, certifications in some places, a working DPIA process and a
mature data protection posture. It also has a flat network, no privileged access management, no
central logging, and backups sitting inside the ransomware blast radius. Competent in the places
that get audited, weak in the places that do not. That is what mid-sized UK councils actually
look like, and it is what makes the prioritisation exercise worth doing. An organisation failing
everything needs no prioritisation. One failing selectively does.

The two incidents were chosen on the same principle. Neither involved an exotic attack. Both
turned on a missing organisational control rather than a bypassed technical one, which is where
the evidence says local government tends to lose.
