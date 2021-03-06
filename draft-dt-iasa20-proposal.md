---

title: Proposed Structure of the IETF Administrative Organization
abbrev: IAO DT Proposal
docname: draft-dt-iasa20-proposal-01
category: info

ipr: trust200902
area: General
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    role: editor
    ins: J. Hall
    name: Joseph Lorenzo Hall
    organization: CDT
    email: joe@cdt.org
 -
    role: editor
    ins: B. Haberman
    name: Brian Haberman
    organization: Johns Hopkins University
    email: brian@innovationslab.net
 -
    ins: J. Arkko
    name: Jari Arkko
    organization: Ericsson Research
    email: jari.arkko@piuha.net
 -
    ins: L. Daigle
    name: Leslie Daigle
    organization: Thinking Cat Enterprises LLC
    email: ldaigle@thinkingcat.com
 -
    ins: J. Livingood
    name: Jason Livingood
    organization: Comcast
    email: Jason_Livingood@comcast.com
 -
    ins: E. Rescorla
    name: Eric Rescorla
    organization: RTFM, Inc.
    email: ekr@rtfm.com

informative:
  RFC4071:
  I-D.daigle-iasa-retrospective:
  I-D.hall-iasa20-workshops-report:
  I-D.arkko-ietf-iasa-thoughts:
  I-D.arkko-ietf-finance-thoughts:
  I-D.haberman-iasa20dt-recs:
  I-D.hall-iasa2-struct:

  ML-memo:
    title: Options for New Organization to Conduct IETF Administrative Support Activities
    author:
      org: Morgan Lewis
    date: 2018-02
    target: https://mailarchive.ietf.org/arch/msg/iasa20/XT_3vfd3OWVFCW335mRrvWuusaI/

  Diagrams:
    title: IASA 2.0 Strawman Diagram
    author:
      name: Richard Barnes
      ins: R. Barnes
    date: 2018-02-16
    target: https://ipv.sx/iasa2.0/IASA-Strawman.pdf

  Diagrams-no-trust:
    title: IASA 2.0 Strawman Diagram, IETF Trust Not Shown
    author:
      name: Richard Barnes
      ins: R. Barnes
    date: 2018-02-16
    target: https://ipv.sx/iasa2.0/IASA-Strawman-NoTrust.pdf

--- abstract

The IETF Administrative Support Activity (IASA) was originally
established in 2005.  In the intervening years, the needs of the IETF
have evolved in ways that require changes to its administrative
structure.  The IETF Chair started an effort in November of 2016 to
begin the process of changing the IETF administrative structure,
starting with a set of virtual workshops to get input from the IETF
community, and then encompassing a series of BOF sessions at IETF meetings to
define the problem, develop requirements, explore potential options
for changes, and a Design Team -- the authors of this document -- that
would make recommendations.  The purpose of this document is to
collect all of the various materials that have lead up to the Design
Team recommendation that IETF be a Disregarded Limited Liability
Company (LLC) of the Internet Society.


--- middle

# Introduction

The arrangements relating to administrative support for the IETF
(referred to as the "IETF Administrative Support Activity" (IASA)
({{RFC4071}})) were created more than ten years ago, when the IETF
initially took charge of its own administration.  The arrangements
have served the IETF reasonably well, but there's been considerable
change in the necessary tasks, in the world around us, and our own
expectations since the creation of the IASA.

The system has experienced various challenges and frustrations along
the way. IETF participants have experienced some questions over
administrative choices made for the organization (e.g., meeting venue
selections, hotel availability and costs), and then voiced concerns
about the seeming lack of transparency and responsiveness from the
components of IASA, or even clarity about who is responsible for the
decisions, or who to follow up with to address stated concerns.

The IETF community has discussed and continues to discuss these
topics, most recently on the "IASA 2.0" mailing list and BOFs at IETFs
98, 99, 100, and 101.  The IETF Chair convened
a small design team (the authors of this document) in 2017 to start
evaluating potential options.  The purpose of the design team is to
provide material that informs the community discussion, both in terms
of providing a bit more worked through solution ideas, as well as
supporting analysis of the implications of those options.

To be clear, the community is in charge of adopting any
recommendations or making any decisions.  This draft, the output of
the design team's considerations, merely collects the activities
around IASA 2.0 and the Design Team's work into one place.  It should
also be noted that IETF administrative matters have been organized
jointly with ISOC, and it is important that ISOC continue to be
involved in IETF's reorganization.

It should of course be acknowledged that there is no perfect, or even
great solution.  Changing the IETF organizational structure will not
fix every problem and may bring new problems of its own.  But it seems
that the current structure is brittle and the issues around lack of
staff and authority, clarity, and responsibility are sufficiently
serious to explore different options.

This document defines a problem statement and a set of goals for the IASA 2.0 effort in terms of an
abstract administrative structure, called IETFAdminOrg (or IAO).
Then, it discusses four possible legal structures of IAO and
describes specifically how the LLC model (what this document refers to as
Option 3) addresses the goals.  In no case does IAO have
anything to do with defining, changing, or operating the IETF's
standards process and structure (participants (not members), WGs, IESG
and so on), which remain as they stand today.

As a base for this document, there was a good articulation of the set of
problems we are facing after an initial set of virtual workshops in
early 2017 in [I-D.hall-iasa20-workshops-report] and a number of
drafts describing problems from specific perspectives:
[I-D.daigle-iasa-retrospective], [I-D.arkko-ietf-iasa-thoughts],
[I-D.arkko-ietf-finance-thoughts]. The Design Team specified the types
of organizational models and recommendations in
[I-D.haberman-iasa20dt-recs] for IETF 100, and proposed elements of a
specific structure in [I-D.hall-iasa2-struct] for discussion at IETF 101.
Some of the content from these documents has been
incorporated into this document.

The next two sections ({{background}} and {{problem-statement}})
describe the background and summarize the challenges noted in the
community discussion.  The two sections after that ({{goals}} and
{{legal-options}}) describe the goals and discuss the primary legal
options for changes.  The following two sections ({{dt-rec}} and
{{imp-issues}}) discuss, respectively, the Design Team's rationale for
recommending the LLC option (Option 3) and issues that will need to be
carefully considered by a Working Group established to further specify
the new organizational structure.

#  Background {#background}

##  Terminology

The following acronyms are used in this document:

* IASA - IETF Administrative Support Activity - An organized activity
  that provides administrative support for the IETF, the IAB, and the
  IESG.

* IAOC - IETF Administrative Oversight Committee in the current IASA
  system - A largely IETF-selected committee that oversees and directs
  IASA.  Accountable to the IETF community.

* IAOC committees - Recognizing the need for specialized attention for
  different branches of work requiring IAOC oversight, the IAOC
  expanded its support by creating committees.  Currently, the
  committees do the heavy lifting on specific tasks, while the IAOC is
  the one responsible for final decisions.

* IAO - An abbreviation referring to the new IETF administrative
  organization (called "IETFAdminOrg" in past documents).

* ISOC - The Internet Society - The organizational home of the IETF,
  and one that in the current IASA system assists the IETF with legal,
  administrative, and funding tasks.

* IAD - IETF Administrative Director - In the current system, the sole
  staff member responsible for carrying out the work of the IASA.  An
  ISOC employee.

* IETF Trust - In the current system, the IETF Trust acquires,
  maintains, and licenses intellectual and other property used in
  connection with the administration of the IETF.  Same composition as
  IAOC.

##  Current IASA Arrangements

The administrative support structure is intended to be responsive to
the administrative needs of the IETF technical community.

RFC 4071 {{RFC4071}} defines the current IETF Administrative Support
Activity (IASA).  It is an activity housed within the Internet Society
(ISOC), as is the rest of the IETF.  RFC 4071 defines the roles and
responsibilities of the IETF Administrative Oversight Committee
(IAOC), the IETF Administrative Director (IAD), and ISOC in the fiscal
and administrative support of the IETF standards process.  It also
defines the membership and selection rules for the IAOC.

As RFC 4071 notes, IASA is distinct from IETF-related technical
functions, such as the RFC Editor, the IANA, and the IETF standards
process itself.  The IASA has no influence on the technical decisions
of the IETF or on the technical contents of IETF work.

Today, IASA's activities support a number of functions within the IETF
system:

* Meeting planning

* Budget and financial management

* Contracting with and overseeing the secretariat

* Contracting with and overseeing the RFC Editor (together with the
  IAB)

* Contracting with and overseeing IANA (together with the IAB)

* Legal ownership of IETF materials, domain names and copyright

* Ownership of IANA-related domain names and copyright

* General legal support (including topics beyond domains and IPR)

* The IETF website

* IETF IT services

* Tooling support, maintenance, and development (together with
  volunteers)

* Meeting network support

* Remote attendance support

* Communications assistance for the IETF

* Sponsorship and funding (together with ISOC)

# Problem Statement {#problem-statement}

The purpose of this part of the document is to describe a few problem
areas with enough detail to allow the comparison of potential IASA
structure updates (among themselves, as well as comparison to the
status quo) that must be addressed by IAO.  This is
intentionally illustrative, rather than an exhaustive enumeration of
all possible and perceived issues with the current structure and
implementation.  Nevertheless, the examples are concrete and real.
(For a fuller description of the perceived issues with the current
IASA arrangements, see {{?I-D.daigle-iasa-retrospective}},
{{?I-D.hall-iasa20-workshops-report}},
{{?I-D.arkko-ietf-iasa-thoughts}}, {{?I-D.arkko-ietf-finance-thoughts}}, and ongoing discussion on the
iasa20@ietf.org mailing list.)

In general, the range of IETF administrative tasks have grown
considerably, our organizational structure is not as clear, efficient,
or as fully resourced as it should be, the division of
responsibilities between the IETF and ISOC continues to evolve,
expectations on transparency have changed, and we face continued
challenges related to funding IETF activities on a background of
increasing costs and lack of predictability in our funding streams.

## Lack of Clarity {#lack-clarity}

In general, as the IETF has grown and aged, an increasing lack of
clarity exists in a number of specific areas.  We discuss four areas
where this lack of clarity is specifically acute: responsibility,
representation, authority, and oversight.

### Responsibility

The line between the IETF and ISOC is not organizationally clear-cut,
which has led to issues around transparency, allocation of staff time
and priorities, budgeting, and clarity of who is responsible for what.

Often, it can be unclear what part of the IETF or ISOC is responsible
for a particular function.  Things as simple as ensuring there is a
lanyard sponsor/coordinator, but also functions as important as
fundraising and sponsorship development have suffered from a lack of
clear responsibility.

IAO must have lines of responsibility that are clear enough
for non-IETFers to understand where responsibilities lie, and how to
make changes as necessary over time.

### Representation

The respective roles of ISOC, the IETF chair, the IAOC, and the
secretariat in representing the IETF to sponsors and donors and
communicating with them are not clear.

Having ISOC represent the IETF to sponsors and donors:

* creates confusion about why the IETF does not represent itself,

* yields questions about why ISOC does not instead increase its IETF
  support and how donations can be guaranteed to be dedicated to the
  IETF,

* can result in those soliciting sponsorships and donations having a
  lack of familiarity with IETF work, and

* creates a lack of an integrated and understandable representation of
  the IETF.  People not familiar with the IETF (e.g., potential
  sponsors) must be able to recognize when or how an entity speaks for
  the IETF.

### Authority

Another significant problem concerns authority, and to what extent can
IETF make decisions on its own in the current structure compared to
decisions that require ISOC approval and agreement.

For example, due to IETF's lack of legal status, contractual
agreements must be signed by ISOC on behalf of the IETF.  There are
occasions when a decision that is right for the IETF and desired by
IETF leadership cannot be executed due to constraints posed by what
ISOC can and cannot agree to itself.  For example, when IETF sought to
acquire a recent piece of software for business purposes, ISOC would
initially not agree to entering into an agreement with the software
provider.  Ideally, IETF could make decisions free from operational
and other constraints imposed by its relationship with ISOC.

IAO must have enough and appropriate authority to carry out
the IETF's administrative requirements and activities in a timely
fashion, and as the IETF desires (within reason of normal business and
legal requirements).

### Oversight {#oversight}

The IAOC is the primary oversight body in the current IASA model, but
there can be confusion or mismatches in roles.  For example, to the
extent that ISOC staff besides the IAD become engaged in
administrative work for the IETF, to whom do they report?  The IAOC,
the IAD, or their management at ISOC? Ultimately, any employee will recognize
their primary responsibility to their employer (i.e,. ISOC, and
specifically to their ISOC management chain). Even in a
well-balanced relationship between the IETF and ISOC, this leads to
conflicting priorities and availability, with the ISOC staff person having
to continuously explain and validate IETF priorities within the ISOC
reporting chain.

Furthermore, when we're in a position where we need more staff
support, it's not obvious what the most appropriate path is to obtain
that support and how the IAOC's oversight fits into the kind of
performance review and career planning that ISOC staff would expect.
We have used a variety of models for acquiring staff support from ISOC
in the past, ranging from the IAD informally soliciting help from
others at ISOC, to the IAOC establishing more formal staff
relationships with ISOC personnel, to ISOC taking responsibility for
finding staff with an internal-to-ISOC reporting chain.  The role of
the IAOC with respect to such staff is not defined, nor is the
mechanism for reflecting the work that they do for the IETF back to
their ISOC management.

IAO's oversight and management functions must be complete and coherent. For
example, it might either take on full oversight responsibility for
staff employment functions (including reporting structures for management reporting and career
development), or the oversight role must be limited to review input
submitted to the external sources responsible for employment, leaving the question of competing priorities unsolved.

## Lack of Resources {#lack-resources}

IETF faces growing constraints on resources essential for IETF to
function, notably in volunteers and staff.

### Volunteers

The IAD is the sole full-time employee for IETF, and the IASA
arrangement encompasses a series of volunteer committees that help to
work through issues such as finance, legal, meetings, technology
management, requests for proposals, and sponsorship. These responsibilities are
expanding in both time requirements, and scope. In some cases, the IETF is verging on
requiring volunteers to take on actual work items — which is beyond the scope of what
is reasonable to ask of a volunteer. As a result, it is
becoming close to impossible to find qualified volunteers who are
willing to stand for open slots on the IAOC.  In general, on both the
IAOC and the committees, the time that committee members have to
devote to the tasks at hand falls far short of what is required to do
much of anything beyond keeping the organization afloat.  At a time
when the IETF is faced with administrative and financial challenges,
barely having enough volunteers and volunteer time to keep the current
operation running is not a sustainable model.

IAO must rely less on volunteers or be better assured of
engagement of willing and capable volunteers.

### Staff

IETF faces serious constraints on staff capacity under the current
IASA model.  The one IAD role and support from contractors have been
used to assure that capacity needed is for the most part in place.
However, it seems clear that the IAD role is overly complex and taxing
for a single human at this point, necessitating measures such as
providing an administrator for the IAOC to better run that body and
their meetings.  IAO will require more paid employment
support dedicated to IETF work.

## Lack of Transparency {#lack-transparency}

The IAOC has sometimes been perceived to operate less transparently
than what is the norm for IETF processes and other IETF leadership
bodies.  This can be observed, for example, in the failure to publicly
share agreed information in a timely fashion.  The reasons behind this
vary but can sometimes be caused by lack of resources to review and
prepare material for community review, or even fear of community
reaction to potential administrative decisions.

Work to increase transparency has made progress, but we must continue
to address and improve this.  At the same time, a balance must be
struck to reach the right level of transparency, so that certain
aspects of contracts, business terms, and negotiations can remain
confidential, according to legal and business practice norms.  It will
be important for the community and any future IASA function to better
define this in order to better meet well-defined, balanced community
expectations on transparency and information sharing.  IAO
will be required to operated in a transparent fashion per community
expectations set as part of this IASA 2.0 process.

## Funding/Operating Model Mismatch and Rising Costs {#funding}

The IETF is facing a changing financial landscape, and is ill-equipped to set itself up for the future.

Meeting fees are currently an important source of revenue, but the
emergence of more viable remote participation tools and other factors
are likely responsible for declining in-person meeting attendance
going forward.

While there has been a lot of sponsor support for, e.g., meeting
hosting, getting support for the full costs of operating the IETF is
not easy.  The costs are quite large, the value to sponsors is not
always obvious, the IETF community is sometimes critical or
unappreciative, and the same sponsors get tapped again and again for
many related but different opportunities.

In addition, relying heavily on meeting-based revenue is somewhat at
odds with the fact that much of the IETF's work takes place outside of
in-person meetings.

Further exacerbating the situation, the IETF is increasingly relying on professional services to support
its activities - in order to more efficiently operate the IETF's
activities and better enable IETF participants to contribute to the
IETF's core technical work rather than administrative and supporting
activities work -- which is also causing expenses to grow.

IAO must have appropriate expertise/resource to identify better funding models for the future for the IETF to deal with its evolving realities, as well as the authority and tools to implement them.

# Goals {#goals}

The IASA redesign effort needs to address the main issues listed above
in {{problem-statement}}.  More specifically, the future organizational
structure needs to do at least the following:

* Protect the IETF's Culture and Technical Work: Ensure that the
  future IASA organizational structure and processes preserve and
  protect the IETF's unique culture of individual contribution, clear
  separation of financial support from technical work, as well as the
  "rough consensus and running code" approach to the development of
  open Internet standards.

* Improve the IETF's Technical Environment: Undertake changes to
  better enable technical contributors to focus more on that technical
  work and less on administrative work or support activities.  This
  could for example mean directing more financial resources towards
  the creation of new or improvement of existing tools, which might be
  produced by contractors rather than solely by volunteers.  As a
  result, volunteers could instead focus on developing the standards
  themselves.  Thus, if the core competency of IETF attendees and
  their reason for participating in the IETF is to develop standards,
  then create an environment where they can focus exclusively on that
  activity and delegate to contractors, staff, or other resources the
  responsibility for creating and maintaining tools and processes to
  support this activity.

* Clearly Define the IETF-ISOC Relationship: Define the roles of IETF
  and ISOC in a way that helps the above structure be as clear as
  possible, in terms of who does what, how are things accounted for,
  and who is in charge of adjustments and control (e.g., staff
  resources).  This also includes consideration of a new funding model
  that takes into account the historical responsibility for the IETF
  that ISOC has had since its inception.

* Support a Re-Envisioned Funding Model: Provide the staff support and
  resources needed to adapt the funding model of the IETF to changes
  in the industry, participation, and expenses.  The structure should
  also allow for and be able to support new funding streams or changes
  to the proportion of funds from various sources.

* Provide Clarity About the IETF-ISOC Financial Arrangements: A
  redesign needs to clear up ambiguities in the financial arrangements
  between IETF and ISOC.  It must also be clear to people outside the
  IETF and ISOC organizations (e.g., sponsors) what the arrangements
  are and what their contributions affect and do not affect.

* Clarify Overall Roles and Responsibilities: Ensure that all staff,
  contractor, and volunteer roles are clearly documented.  This
  necessarily includes documenting how each of these parties may
  interact or interface with one another in order to conduct and
  support the business of the IETF.  This also includes documenting
  key work processes, decision-making processes and authority (such as
  pertaining to meeting venue selection), etc.  A key objective is to
  minimize ambiguity and uncertainty so that it is clear who is
  responsible for what and who has the power to make certain
  decisions.

    There also needs to be a clear definition of what issues belong to
    the IESG or IETF Chair vs. the IASA organization or staff.  In
    many cases that is not clear today, and the IETF Chair role
    includes a lot of administrative leadership responsibility beyond
    a rational scope for the position.

* Define Support Staff Roles and Responsibilities: Clearly define the
  roles of the oversight entities and staff/contractors to match the
  expanded work scope facing the IETF.  Ensure that any changes create
  a structure that can adapt flexibly to future growth and other
  changes (including changes in IETF community expectations, such as
  increased transparency or more rapid decision-making).

* Re-Define the Role of the IETF Community in Relation to
  Administrative Activities: As the roles and responsibilities for
  support staff and volunteer roles are clarified more precisely, the
  role of the IETF community in relation to those staff and volunteer
  roles must be better defined.  This should acknowledge the limited
  time and availability of IETF volunteers, better defining
  expectations around oversight of and involvement in strategic,
  operational, and execution tasks within the administrative efforts.

     The new design needs to ensure that volunteers are not overloaded
     in such things as low level operational decisions, which are
     properly the responsibility of staff, and volunteers can instead
     focus on strategic changes, critical decisions, and so on.  In
     particular, this should focus on clearly documenting the lines
     between responsibility, representation, authority, and oversight.

* Define Improved Transparency Requirements: The general level of
  operational transparency and information-sharing between IETF
  administrative staff and groups to the IETF community must be kept
  at an acceptable level, and improved where it makes sense in the
  future.  This includes ensuring the timeliness of sharing of
  information and decisions, as well as seeking comment on prospective
  decisions.  At the same time, we need to reset
  expectations around responsibility and authority so that once staff or an
  administrative support organization has been delegated certain
  authority by the definition of the new structure, it is clear that they
  are empowered to proceed in a
  particular area .  This will improve organizational efficiency,
  reduce friction, and improve the pace of work and decision-making.
  However, it is clear that enabling a group or staff to act within
  their proscribed authority depends upon a clearer definition of
  roles and responsibilities, on improved transparency, on improved
  communications, and on trust (which is built upon all of those
  things over time).

* Define a Transition Plan: Determine what new IASA structure we need
  and define a transition plan from the model the IETF has today to
  the new structure.

# Legal Options for IETF Organizational Change {#legal-options}

After IETF 100 in November of 2017, the IETF community clearly wanted
more input on the various legal options available for IETF
restructuring as well as the trade-offs among the various options.
The Design Team working with the IETF Chair asked the Internet
Society's tax law attorneys to outline a series of options based on
the requirements developed in this process. The result is a memorandum
{{ML-memo}} that outlines the various options and their trade-offs.
In this section, we summarize those options. We also include a tabular
summary for each option of the legal analysis from Morgan Lewis.

## Option 1 - Independent 501(c)(3)

On one end of the spectrum is complete independence from ISOC. The
natural choice for this would be for IETF to incorporate as an
independent organization, incorporating as a non-profit in a
particular state and then applying at the federal level to the IRS for
tax exemption to achieve 501(c)(3) status.  In this case, all
functions of IAO would be legally independent of ISOC, including board
appointments, hiring and firing, etc. IAO would face increased
one-time and ongoing administrative complexities, including maintenance
of tax-exempt status, separate audits, financial statements, and tax
filing. ISOC could continue to provide funding to the IAO and ISOC
could set the terms of funding through a grant agreement or contract.

|-------------------------------------------+-----|
| Governance: 501(c)(3)                     |     |
|-------------------------------------------+-----|
| Is ISOC involved in appointing IAO Board? | No  |
|-------------------------------------------+-----|
| Can IAO Board hire and fire the IAO ED?   | Yes |
|-------------------------------------------+-----|
| ISOC liable for IAO debts and obligations?| No  |
|-------------------------------------------+-----|

|--------------------------------------------------+-----|
| Finance and Fundraising: 501(c)(3)               |     |
|--------------------------------------------------+-----|
| Can IAO have separate bank account from ISOC?    | Yes |
|--------------------------------------------------+-----|
| Can donors write checks to IAO?                  | Yes |
|--------------------------------------------------+-----|
| IAO needs to maintain its own non-profit status? | Yes |
|--------------------------------------------------+-----|

|-------------------------------------------------------+-----|
| Administration/Staffing: 501(c)(3)                    |     |
|-------------------------------------------------------+-----|
| Would IAO need to conduct its own audit?              | Yes |
|-------------------------------------------------------+-----|
| Would IAO need to file its own tax return?            | Yes |
|-------------------------------------------------------+-----|
| IAO ED can hire/fire, contract without ISOC approval? | Yes |
|-------------------------------------------------------+-----|

## Option 2 - Type 1 Supporting Organization

IAO could be set up as a Type 1 Supporting Organization of ISOC. In
this model, IAO would be set up a 501(c)(3) organization but then list
ISOC as the named supported organization, essentially specifying that
it's a separate entity but one that works to support ISOC's
mission. In this model ISOC would have to be the sole controlling
parent entity, with ISOC retaining formal control of the IAO
Board. This would require incorporation as a non-profit, filing for
federal and state tax exemption, filing separate taxes, but audits and
financial statements would be consolidated with those of ISOC.

|-------------------------------------------+---------|
| Governance: Type 1 Supporting Org.        |         |
|-------------------------------------------+---------|
| Is ISOC involved in appointing IAO Board? | Yes(1)  |
|-------------------------------------------+---------|
| Can IAO Board hire and fire the IAO ED?   | Yes     |
|-------------------------------------------+---------|
| ISOC liable for IAO debts and obligations?| No      |
|-------------------------------------------+---------|

|--------------------------------------------------+-----|
| Finance and Fundraising: Type 1 Supporting Org.  |     |
|--------------------------------------------------+-----|
| Can IAO have separate bank account from ISOC?    | Yes |
|--------------------------------------------------+-----|
| Can donors write checks to IAO?                  | Yes |
|--------------------------------------------------+-----|
| IAO needs to maintain its own non-profit status? | Yes |
|--------------------------------------------------+-----|

|-------------------------------------------------------+-----|
| Administration/Staffing: Type 1 Supporting Org.       |     |
|-------------------------------------------------------+-----|
| Would IAO need to conduct its own audit?              | Yes |
|-------------------------------------------------------+-----|
| Would IAO need to file its own tax return?            | Yes |
|-------------------------------------------------------+-----|
| IAO ED can hire/fire, contract without ISOC approval? | Yes |
|-------------------------------------------------------+-----|

(1) ISOC would be required to appoint majority of the IAO Board,
perhaps upon IETF recommendations.

## Option 3 - Disregarded LLC

IAO could form a Limited Liability Company (LLC) that is a disregarded
entity of ISOC, essentially treating it as a branch or division of
ISOC for most tax purposes. The term "disregarded" here means that the
LLC is disregarded by ISOC for some purposes; that is, while ISOC's
non-profit status and tax exemption applies downward to the LLC, legal
liability and financial impacts do not apply upwards from the LLC to
ISOC.  In contrast to the previous option, ISOC in this case could
delegate the appointment of the IAO Board to a nominating committee
within the IAO. This option would not require tax exemption filing,
filing separate taxes, or separate audits or financial statements.

|-------------------------------------------+-------|
| Governance: Disregarded LLC               +       |
|-------------------------------------------+-------|
| Is ISOC involved in appointing IAO Board? | No(2) |
|-------------------------------------------+-------|
| Can IAO Board hire and fire the IAO ED?   | Yes   |
|-------------------------------------------+-------|
| ISOC liable for IAO debts and obligations?| No    |
|-------------------------------------------+-------|

|--------------------------------------------------+-----|
| Finance and Fundraising: Disregarded LLC         |     |
|--------------------------------------------------+-----|
| Can IAO have separate bank account from ISOC?    | Yes |
|--------------------------------------------------+-----|
| Can donors write checks to IAO?                  | Yes |
|--------------------------------------------------+-----|
| IAO needs to maintain its own non-profit status? | No  |
|--------------------------------------------------+-----|

|-------------------------------------------------------+-----|
| Administration/Staffing: Disregarded LLC              |     |
|-------------------------------------------------------+-----|
| Would IAO need to conduct its own audit?              | No  |
|-------------------------------------------------------+-----|
| Would IAO need to file its own tax return?            | No  |
|-------------------------------------------------------+-----|
| IAO ED can hire/fire, contract without ISOC approval? | Yes |
|-------------------------------------------------------+-----|

(2) ISOC can delegate responsibility for appointing all IAO Board
members to IETF bodies, but must retain ultimate control of the LLC.

## Option 4 - Activity of Internet Society

IASA is currently an activity of ISOC, so this option was included in
the analysis to give a baseline for comparison of the other options.

|-------------------------------------------+----------------|
| Governance: Activity of ISOC              |                |
|-------------------------------------------+----------------|
| Is ISOC involved in appointing IAO Board? | Yes, as today  |
|-------------------------------------------+----------------|
| Can IAO Board hire and fire the IAO ED?   | No             |
|-------------------------------------------+----------------|
| ISOC liable for IAO debts and obligations?| Yes            |
|-------------------------------------------+----------------|

|--------------------------------------------------+-----|
| Finance and Fundraising: Activity of ISOC        |     |
|--------------------------------------------------+-----|
| Can IAO have separate bank account from ISOC?    | Yes |
|--------------------------------------------------+-----|
| Can donors write checks to IAO?                  | No  |
|--------------------------------------------------+-----|
| IAO needs to maintain its own non-profit status? | No  |
|--------------------------------------------------+-----|

|-------------------------------------------------------+-----|
| Administration/Staffing: Activity of ISOC             |     |
|-------------------------------------------------------+-----|
| Would IAO need to conduct its own audit?              | No  |
|-------------------------------------------------------+-----|
| Would IAO need to file its own tax return?            | No  |
|-------------------------------------------------------+-----|
| IAO ED can hire/fire, contract without ISOC approval? | No |
|-------------------------------------------------------+-----|

# Design Team Recommendation (Option 3) {#dt-rec}

After discussion and consideration, the design team recommended at the
IASA 2.0 BOF session at IETF 101 that we pursue Option 3, the
disregarded LLC option.

In our view, this option gives increased independence without the full
administrative complexity of the other options. Notably, this option is
easier to set up than the non-profit corporation options and also has
simpler annual reporting requirements; that is, the LLC option does
not require filing for
state and federal tax exempt status, and it allows IETF to continue to
benefit from ISOC's tax exempt status and financial reporting and
auditing. IAO will be a legal entity that can have and control its own
bank accounts and sign contracts without involving ISOC. Crucially,
this option allows the operating agreement to delegate the task of
appointing a board to a committee (likely the IAB) of IETF.

# Important Remaining Issues {#imp-issues}

## Transparency

The issue of increased transparency was important throughout the IASA
2.0 process, with little to no dissent.  It was recognized that there
will naturally be a confidentiality requirement about hotel
contracting, personnel matters, and other narrow areas.  At IETF 101
in the IASA 2.0 BOF, the design team proposed the following default
transparency rule:

> Whatever doesn't have a specific justification for being kept
  confidential, should be made public. There must exist a public list
  of confidential items, describing the nature of the information and
  the reason for confidentiality.

## IAO Board

The composition of the IAO Board requires careful thought and
deliberation. An earlier draft from the design team discussed a small
5-member board, and list discussion saw proposals that included 7 and
9 members, with some mix of the IETF Chair, IETF-appointed ISOC Board
members, NOMCOM-appointed members. Discussion of composition, term
lengths, types of experience needed, liaisons, officers, are all
details the design team will leave in the hands of a chartered IETF
working group in the near future.

## Input from the IETF Community

The current IAOC also involves a structure of 7 substantive committees
(Finance, Legal, Meetings, Technology, RFPs, Sponsorship, and Venue
Review) where IETF community volunteers can contribute to the
administrative work of the IETF. Under a new structure, much of this
activity will be performed by paid IAO staff, potentially limiting the
nature and quantity of feedback that the IAO gets from the IETF
community.  One option discussed heavily and mostly rejected was the
potential notion of an Advisory Council, that could be a venue for
directly marshaling community feedback into the IAO structure.

It is unclear what kind of feedback mechanism -- other than email sent
in response to an ietf@ietf.org mailing list post -- would be
important to ensure that IAO has a good, ongoing sense of the
community, so we leave this to future deliberation.

## Non-US incorporation

Finally, the community rightly challenged the design team in terms of
exploring organizational options in non-US venues, e.g., non-profit
incorporation in Europe or Asia.  However, given that ISOC even under
a complete independence model will still need to be heavily involved
in the business of IAO, there were no clear options that seemed
strictly better given the problem statement and goals outlined above.

# Acknowledgments

Thanks to Richard Barnes, Alissa Cooper, John Levine, and Sean Turner for
discussions of possible structures, and to the attorneys of Morgan
Lewis for their advice on possible legal impacts.
