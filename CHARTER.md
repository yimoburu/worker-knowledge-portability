# Worker Knowledge Portability Charter

**Version:** 0.2.2 discussion draft

**Status:** Request for critique

**Implementation:** Not authorized

## 1. Purpose

AI-assisted work can produce records that combine protected source material,
work artifacts, evidence items, and claims about a worker's capability. This
charter proposes a minimum floor of protection and procedural safeguards for
systems that capture, infer, retain, evaluate, present, or transfer observable
objects arising from that work.

The canonical stress test is worker offboarding. It concerns the ending or
material change of a work relationship, role, or access; it is not the
offboarding of an AI system.

## 2. Terminology and interpretation

This charter incorporates [TERMINOLOGY.md](TERMINOLOGY.md) by reference. Its
controlled vocabulary governs the interpretation of this document. In
particular, a capability is a person's ability, skill, knowledge, or judgment;
the candidate portable object is a capability claim, not the capability itself.

**Worker** is the umbrella term for a natural person performing work for or
through an organization, including an employee or a non-employee worker. The
term does not determine legal status. **Employee** and **employer** apply only
where a legally recognized employment relationship is intended. **Originating
organization** means the source-side organization controlling relevant work
systems or records; it may be an employer, client, platform, agency,
partnership, or another organization. These terms do not allocate universal
legal ownership.

## 3. Scope and limits

The charter applies to workers, originating organizations, receiving
organizations, AI providers and operators, worker representative bodies,
reviewers, conformity assessors, certification bodies, and regulators involved
in claims or evidence arising from AI-assisted work.

It does not replace intellectual-property, employment, privacy, trade-secret,
contract, security, regulatory, or data-protection law. It does not require
raw-trace portability, protected-source disclosure, organizational endorsement
of every worker claim, or one product or business model.

Participation in telemetry or AI-assisted work does not automatically
constitute consent to capability-claim portability, secondary use, an
authorization, or an ownership decision.

## 4. Normative principles

### 4.1 Transparent participation

Affected people must be told what is captured, inferred, retained, disclosed,
presented, and used to evaluate them. The consequences of participating or
declining must be understandable before those choices become consequential.

### 4.2 Capability claims, not capability transfer

Workers may describe, assert, and present generalized claims about their skills
and judgment. An employment relationship or organizational custody alone must
not convert a person's general capability into an exclusively owned record.
The charter cannot revoke a worker's underlying capability; it can govern a
claim, attestation, authorization, evidence item, or work artifact.

### 4.3 Protected source material and disclosure minimization

Portability must not disclose confidential information, trade secrets,
regulated data, or work product subject to applicable restrictions and
permissions. A disclosure-minimized abstraction must identify its policy,
method, and defined threat model, including the protected-source disclosure or
reconstruction risk it is intended to reduce. It does not guarantee that risk
is eliminated.

### 4.4 Governed-object separation

A trace, conversation, case, or file must not receive one disposition merely
for administrative convenience. Decisions apply to each governed object: the
particular claim, evidence item, or artifact receiving that disposition. A
case may contain several governed objects with different dispositions.

### 4.5 Separate claims from evidence and authorization

A capability claim may be presented while supporting evidence remains in
protected custody. Evidence supports evaluation; it does not automatically
prove a claim. Worker-originated content authorized for reuse may be presented
only within its applicable restrictions and permissions. Custody does not by
itself establish ownership, license, authorization, or truth.

An AI memory object may be used to propose or support a capability claim, but
it is not automatically a capability claim or a worker-portable object. Technical
exportability, association with a worker, or storage in a user-facing account
does not by itself authorize portability. Provenance, applicable restrictions
and permissions, disclosure minimization, authorization, claim and attestation
status, review status, and per-object disposition must remain separately
visible.

### 4.6 Meaningful review without retaliation

Workers and originating organizations must be able to inspect, challenge, and
appeal consequential dispositions without hidden penalties. Security and
confidentiality restrictions must be explicit, proportionate, and reviewable.

## 5. Minimum procedural safeguards

1. **Notice and reasons:** Affected parties receive the proposed disposition,
   purpose, governing policy profile, applicable restrictions and permissions,
   asserted source of authority, and a human-understandable explanation.
2. **Visible object and assurance status:** A claim identifies its provenance
   and visible claim, attestation, verification, authorization, and review
   status. A record must distinguish a self-assertion, attestation,
   verification result, and relying-party assessment.
3. **Per-object dispositions:** The four dispositions in Section 6 apply per
   governed object, not to an entire person or case.
4. **Time-bounded review:** Silence does not imply endorsement, authorization,
   or release of protected evidence. It also does not create an indefinite veto
   over a disclosure-minimized capability claim whose limits and unresolved
   status are visible.
5. **Dispute containment:** During a dispute, protected evidence remains in
   its applicable custody and only an authorized, disclosure-minimized claim or
   artifact may be presented. Unresolved claim, evidence, and authorization
   relationships remain visible.
6. **Authorized protected-evidence review:** An independent reviewer may
   inspect protected evidence only with applicable authorization and
   confidentiality safeguards. That review must not require disclosure of the
   evidence to the worker, receiving organization, or relying party.
7. **Durable history:** Decisions, rationales, challenges, attestations,
   authorizations, corrections, revocations, and superseding claims remain
   auditable and are not silently rewritten.

## 6. Governed dispositions

The following dispositions apply per governed object and can coexist in one
case. For example, a case can contain retained evidence, an authorized shared
artifact, and a worker-portable self-asserted claim.

| Disposition | Meaning |
| --- | --- |
| **Retained in protected custody** | The governed object is not authorized to move from its protected source-side custody. |
| **Authorized for specified use** | Access, use, disclosure, or transfer is authorized for a stated purpose, scope, recipient, duration, and other applicable conditions. |
| **Worker-portable claim** | A capability claim may be presented by or for the worker with provenance, attestation, verification, and review status visible. |
| **Restricted or pending dispute** | Movement or reliance is restricted while an authorization, evidence, or claim relationship remains unresolved. |

## 7. Separate roles and assessments

A capability claim can contain independently visible statements and records
from distinct roles:

- **Worker / claim subject:** makes, accepts, challenges, withdraws, or
  presents a claim about their capability.
- **Evidence custodian:** holds or controls evidence and records its custody;
  this role does not decide ownership, authorization, or truth.
- **Attestor:** makes a scoped statement following a stated review or process.
- **Verifier:** checks authorship, integrity, technical validity, and current
  status; verification does not determine a claim's truth or fitness for use.
- **Relying party:** determines whether a claim and its assurance information
  are fit for a particular purpose.
- **Independent reviewer:** conducts an authorized review or dispute review
  under a stated procedure and with required confidentiality safeguards.
- **Conformity assessor or certification body:** evaluates an implementation
  or process against published requirements through conformance assessment.
- **Appeal body:** conducts escalated review of an earlier disposition under a
  stated procedure.

An originating organization may attest to a claim-evidence relationship. An
independent reviewer may issue a separate attestation after authorized review.
Neither action certifies a worker's capability. Certification, if a formal
program exists, applies only to the evaluated implementation or process and
its stated scope.

## 8. Separate lifecycles

The following future lifecycles remain separate:

| Object | Lifecycle |
| --- | --- |
| Claim | draft, assert, present, challenge, withdraw, supersede |
| Attestation | issue, suspend, revoke, expire, supersede |
| Authorization | grant, restrict, revoke, expire |
| Evidence | retain, restrict, disclose for authorized review, archive, or delete under applicable obligations |

An attestation or authorization may be revoked. That action changes the
statement or permission; it cannot revoke a worker's underlying capability.

## 9. Governance and legitimacy

Institutional powers should remain separated:

- A protocol steward may maintain future specifications through transparent,
  multi-stakeholder governance.
- Policy-profile bodies may adapt common safeguards to jurisdictions,
  contracts, and sectors without weakening the minimum floor.
- Independent conformity assessors or certification bodies may evaluate
  implementations only under published requirements and a stated program.
- Appeal bodies may resolve escalated disputes without also controlling a
  future protocol or implementation.
- Worker collectives, unions, guilds, and data trusts may represent workers
  and challenge systemic behavior under worker authorization, applicable law,
  or a stated Charter procedure.
- A public decision-and-rationale registry may publish anonymized decisions
  and rationale, never protected evidence.
- Stewards, reviewers, conformity assessors, certification bodies, and appeal
  bodies must disclose funding and relationships that could compromise
  independence.

The rule maker, implementer, conformity assessor or certification body, and
appeal body must not all be the same institution.

## 10. Incentive alignment

- Workers receive understandable capture rules, continuity for authorized
  claims, review, and remedy.
- Originating organizations receive protected evidence custody, lower
  disclosure risk, clearer offboarding, and defensible audit records.
- AI providers and operators receive common interoperability and assurance
  semantics instead of bespoke bilateral rules.
- Worker representative bodies may receive standing under worker authorization,
  applicable law, or a stated Charter procedure to negotiate policy profiles.
- Auditors and regulators receive inspectable dispositions without
  centralizing all protected evidence.

Basic inspection, correction, dispute, and authorized presentation must not be
paywalled. Participation choices must not use deceptive defaults. Objects
authorized for specified use must state purpose, scope, recipient, duration,
other conditions, and any applicable value terms.

Success must not be measured only by telemetry volume. Relevant measures
include informed adoption, worker and organizational confidence,
protected-information leakage, review latency, dispute patterns, remedy
quality, and authorized portability.

## 11. Red lines

A process fails this charter if it permits:

- Blanket ownership of an entire trace based only on storage, employment, or
  tool ownership.
- Disclosure of protected source material through an abstraction that has not
  been assessed under a defined threat model.
- Credential laundering that presents a self-asserted or inferred capability
  claim as organizationally attested or certified.
- Permanent veto through delay or non-participation.
- Hidden capture, hidden consequences, or coercive participation defaults.
- One interested party controlling rules, implementation, conformance
  assessment, and appeal.
- Silent deletion or rewriting of disputes, attestations, authorizations, or
  claim history.
- Proprietary lock-in presented as interoperability.

## 12. Conformance boundary

Conformance assessment would evaluate the behavior of an implementation or
process and its procedural safeguards under standard and adversarial cases. It
would not determine universal legal ownership, guarantee that every claim is
true, certify a worker, or promise zero risk.

This draft does not define or authorize a protocol, schema, certification
program, adjudicator, pilot, or reference implementation.

## 13. Review question

Does this charter describe a real cross-industry gap that cannot be adequately
addressed through existing law, contracts, credentials, provenance standards,
and data-portability mechanisms? Evidence supporting **continue**, **narrow**,
or **stop** is equally valuable.
