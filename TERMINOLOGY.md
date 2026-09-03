# Terminology

This controlled vocabulary applies to the Worker Knowledge Portability Charter
and related discussion documents. It distinguishes claims from a person's
underlying capability, and does not allocate universal legal ownership.

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
- **Attestor:** An identified actor that makes a scoped statement following a
  stated review or process.
- **Verifier:** An actor that checks authorship, integrity, technical validity,
  and current status.
- **Conformity-assessment or certification body:** An actor that evaluates an
  implementation or process against published requirements. An independent
  assessor may issue an attestation after authorized review; that is not the
  same as certifying an implementation.

## Records, claims, and evidence

- **Knowledge:** The broad problem-domain word in the project name. Operational
  text should identify the observable object instead.
- **Observable object:** An AI-assisted work record, capability claim, evidence
  item, protected source material, or work artifact. Do not use **knowledge
  unit** as a decision object: it implies that knowledge can always be atomized
  and assigned one status.
- **AI-assisted work record:** Content, outputs, metadata, events, feedback,
  and derived information produced through AI-assisted work.
- **AI memory object:** A conversation export, agent-state package, reusable
  prompt pattern, knowledge-graph entry, model-generated summary, or similar
  retained runtime artifact. It may be an evidence item, work artifact, or
  another kind of AI-assisted work record; it is not automatically a
  capability claim or an authorized portable object.
- **Trace:** A technical telemetry object composed of spans. It is not the
  umbrella for prompts, work product, memory, evidence, and capability.
- **Work artifact:** An observable work product. It must be identified as such
  rather than treated as a person's capability.
- **Capability:** A worker's ability, skill, knowledge, or judgment. It is not itself a transferable digital object. No system can revoke a person's underlying capability. A system may transfer or present only a claim about capability.
- **Capability claim:** An assertion about a worker's capability. It is the
  candidate portable object and can be self-asserted, attested, challenged,
  withdrawn, or superseded.
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

- **Attestation:** A scoped statement made by an identified actor following a
  stated review or process. It states who asserted what under which criteria;
  it does not establish universal truth.
- **Verification:** Checking authorship, integrity, technical validity, and
  current status. Verification does not establish truth or determine whether
  the underlying claim is true or fit for use.
- **Relying-party assessment:** A receiving actor's evaluation of whether a
  claim and its assurance information are fit for a particular purpose.
- **Conformance assessment:** Evaluation of an implementation or process
  against published requirements.
- **Certification:** A formal conformance result issued under an established
  certification program. It applies to the evaluated implementation or process
  and scope, not to the universal truth of a worker's capability.
- **Portability:** The ability to present or reuse an authorized claim across
  systems or contexts. This term does not itself assert a statutory
  data-portability right.
- **Disclosure-minimized abstraction:** A generalized claim produced and
  assessed under a defined policy, method, and threat model to reduce
  protected-source disclosure or reconstruction risk. It is not an
  unconditional guarantee of safety.

## Governance and lifecycle

- **Governed object:** The particular claim, evidence item, or artifact
  receiving a disposition. A single case can contain several governed objects
  with different dispositions.
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
| Attestation | issue, suspend, revoke, expire, supersede |
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
| **Worker-portable claim** | A capability claim may be presented by or for the worker with provenance, attestation, verification, and review status visible. |
| **Restricted or pending dispute** | Movement or reliance is restricted while an authorization, evidence, or claim relationship remains unresolved. |
