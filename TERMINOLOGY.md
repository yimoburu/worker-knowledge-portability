# Terminology

This controlled vocabulary applies to the Worker Knowledge Portability Charter
and related discussion documents. It distinguishes claims from a person's
underlying capability, and does not allocate universal legal ownership.

## Project terms

- **Worker Knowledge Portability:** A project-defined concept for governing how
  capability claims may continue across contexts. It does not mean exporting
  raw data, memory, or organizational knowledge, and it does not assert a
  statutory portability right.
- **Worker Knowledge Portability Charter:** The project's principles-first
  discussion draft. The word **Charter** does not imply an adopted standard,
  binding agreement, or established governance institution.

## Roles

- **Worker:** A natural person performing work for or through an organization,
  including an employee or a non-employee worker. This term does not determine
  legal status.
- **Employee:** A worker in a legally recognized employment relationship.
- **Employer:** The counterpart in that employment relationship.
- **Originating organization:** The source-side organization controlling
  relevant work systems or records. It can be an employer, client, platform,
  agency, partnership, or another organization.
- **Receiving organization:** The organization to which a claim is presented.
- **Relying party:** The actor deciding whether a claim is fit for a particular
  purpose.
- **Claim attestor:** An identified actor that provides attributable support
  for a capability claim or a claim-evidence relationship under a stated
  review or process.
- **Technical verifier:** An actor that checks authorship, integrity, technical
  validity, and current status. This role does not determine truth or fitness
  for purpose.
- **Conformity assessment body or certification body:** A body that conducts formal
  conformity assessment under an established scheme, or certification under
  an established certification program. These terms are reserved for those
  formal contexts; an independent assessor under this discussion draft is not
  automatically such a body.

## Records, claims, and evidence

- **Knowledge:** The broad problem-domain word in the project name. Operational
  text should identify the observable object instead.
- **Observable object:** An AI-assisted work record, capability claim, evidence
  item, protected source material, or work artifact. Do not use **knowledge
  unit** as a decision object: it implies that knowledge can always be atomized
  and assigned one status.
- **AI-assisted work record:** Content, outputs, metadata, events, feedback,
  and derived information produced through AI-assisted work.
- **AI memory record:** A stored representation created or maintained for AI
  recall, personalization, or adaptation, including extracted facts,
  summaries, profiles, learned instructions, or relationships. Association
  with a worker does not make it a worker-portable capability claim.
- **Agent-state package:** A serialized or exported package of agent state,
  such as prompts, message history, memory, tools, skills, or configuration.
  Technical portability does not authorize the package or its contents to move
  across an organizational boundary.
- **Candidate capability abstraction:** An implementation-generated proposal
  for a generalized capability claim. It remains an input or candidate rather
  than a worker-portable claim until the applicable provenance,
  disclosure-minimization, restrictions and permissions, authorization,
  status, review, and disposition requirements are satisfied.
- **Trace:** A technical telemetry object composed of spans. It is not the
  umbrella for prompts, work product, memory, evidence, and capability.
- **Work artifact:** An observable work product. It must be identified as such
  rather than treated as a person's capability.
- **Capability:** A worker's ability, skill, knowledge, or judgment. It is not itself a transferable digital object. No system can revoke a person's underlying capability. A system may transfer or present only a claim about capability.
- **Capability claim:** An assertion about a worker's capability. It is the
  candidate portable object and can be self-asserted, supported by a claim
  attestation, challenged, withdrawn, or superseded.
- **Evidence item:** Information used to assess a claim. It supports evaluation
  but does not automatically prove the claim.
- **Protected source material:** Evidence or content subject to an applicable
  confidentiality, trade-secret, privacy, contractual, security, regulatory,
  or third-party restriction. The label records a restriction; it does not
  decide ownership.
- **Confidential information:** The broader category for protected information.
  Use **trade secret** only where the applicable legal criteria are intended.
- **Personal data:** Information concerning identifiability, not ownership or
  portability. Do not use **personal content** to mean content a worker owns or
  may export; use **worker-originated content authorized for reuse** when that
  is the intended meaning.
- **Provenance:** Information about the entities, activities, and actors
  involved in producing, influencing, or deriving a record, claim, or evidence
  item.
- **Custody:** Technical or administrative possession and control of a record.
  Custody does not establish ownership, license, authorization, or truth.
- **Authorization:** Permission to access, use, disclose, present, or transfer
  something under an applicable source of authority, such as law, contract,
  policy, or consent.
- **Applicable restrictions and permissions:** The asserted restrictions or
  permissions and their source of authority. This replaces a generic
  "rights status" and does not infer a license.

## Assurance and assessment

- **Claim attestation:** A scoped, attributable statement supporting a
  capability claim or a claim-evidence relationship under a stated review or
  process. It does not establish universal truth, perform technical
  verification, or determine fitness for purpose. This project term is
  distinct from formal attestation of conformity.
- **Technical verification:** Checking authorship, integrity, technical
  validity, and current status. Technical verification does not establish
  truth or determine whether the underlying claim is fit for use.
- **Relying-party assessment:** The relying party's evaluation of whether a
  claim and its assurance information are fit for a particular purpose.
- **Conformance test:** A technical test of an implementation or process
  against published requirements. Passing a test does not itself constitute
  formal conformity assessment or certification.
- **Independent assessment against published requirements:** An evaluation of
  an implementation or process against published requirements by an assessor
  independent of the implementer and relying party. In this discussion draft,
  this phrase does not imply an established conformity assessment scheme.
- **Conformity assessment:** The formal standards term for demonstrating
  whether specified requirements are fulfilled. This term is reserved here for
  a future established scheme.
- **Certification:** Formal third-party attestation that specified requirements
  have been fulfilled, issued under an established certification program. It
  applies only to the evaluated implementation or process and stated scope,
  not to the universal truth of a worker's capability.
- **Portability:** The ability to present or reuse an authorized claim across
  systems or contexts. This term does not itself assert a statutory
  data-portability right.
- **Disclosure-minimizing abstraction:** A generalized claim produced and
  assessed under a defined policy, method, and threat model to reduce
  protected-source disclosure or reconstruction risk. It is not an
  unconditional guarantee of safety.

## Governance and lifecycle

- **Governed object:** The particular claim, evidence item, or artifact
  receiving a disposition. A single case can contain several governed objects
  with different dispositions.
- **Governed disposition:** The recorded outcome assigned to one governed
  object. It is not a blanket ownership determination for a person, case,
  conversation, or file.
- **Offboarding:** The ending or material change of a work relationship, role,
  or access. It does not mean decommissioning an AI system.
- **Review:** Reconsideration of a proposed or completed disposition by an
  authorized actor.
- **Appeal:** Escalated review of an earlier decision under a stated procedure.
- **Remedy:** A corrective response available under the applicable policy,
  agreement, or law after an error or violation is established.

Future lifecycles remain separate:

| Object | Lifecycle |
| --- | --- |
| Claim | draft, assert, present, challenge, withdraw, supersede |
| Claim attestation | issue, suspend, revoke, expire, supersede |
| Authorization | grant, restrict, revoke, expire |
| Evidence | retain, restrict, disclose for authorized review, archive, or delete under applicable obligations |

## Governed dispositions

Dispositions apply per governed object and can coexist in one case. For
example, a case can contain retained evidence, an authorized shared artifact,
and a worker-portable self-asserted claim.

| Disposition | Meaning |
| --- | --- |
| **Retained in protected custody** | The governed object is not authorized to move from its protected source-side custody. |
| **Authorized for specified use** | Access, use, disclosure, or transfer is authorized for a stated purpose, scope, recipient, duration, and other applicable conditions. |
| **Worker-portable claim** | A capability claim may be presented by or for the worker with provenance, claim attestation, technical verification, and review status visible. |
| **Restricted or pending dispute** | Movement or reliance is restricted while an authorization, evidence, or claim relationship remains unresolved. |
