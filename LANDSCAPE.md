# Related Landscape

This project should reuse mature standards rather than inventing every
primitive. A protocol is not the starting assumption. The question is whether
an interoperability and governance profile is needed at the intersection of
AI-assisted work records, protected source material, portable capability
claims, evidence custody, procedural safeguards, and independent assurance.

| Existing work | Reusable contribution | Proposed remaining question |
|---|---|---|
| [Data Transfer Initiative AI portability](https://dtinit.org/ai) and [AI Conversation History schema](https://schemas.pub/schemas/24) | AI-conversation export, service portability, and registry thinking | How should mixed protected source material, work artifacts, capability claims, disclosure minimization, and work-relationship disputes be handled? |
| [ApertoMemory Internet-Draft](https://datatracker.ietf.org/doc/draft-ferro-apertomemory/) | Proposed encrypted portable memory objects, signed provenance, custody records, derived technical status, and test vectors. Datatracker identifies it as an active individual Internet-Draft without IETF endorsement or formal standing. | How should applicable restrictions and permissions be handled when workplace evidence is protected or mixed? |
| [W3C Verifiable Credentials 2.0](https://www.w3.org/TR/vc-data-model-2.0/) | Tamper-evident credentials and presentations; issuer, holder, and verifier roles; status; terms; and privacy. Verifiability does not imply that encoded claims are true; a verifier applies its own policies before relying on them. | How should protected-evidence custody and work-relationship dispute procedures work? |
| [1EdTech Open Badges 3.0](https://www.1edtech.org/standards/open-badges) | Achievement and skill claims, supporting evidence, verifiability, portable exchange, and conformance requirements and certification for implementations | How should a capability claim derived from protected AI-assisted work records be represented without credential laundering? |
| [1EdTech Comprehensive Learner Record 2.0](https://www.1edtech.org/standards/clr) | Secure, verifiable learning and employment records; learner-controlled transport; claims with issuer metadata and possible supporting evidence; compatibility with Open Badges and W3C Verifiable Credentials | What process can support a useful claim when its underlying workplace evidence must remain protected? |
| [Experience You Phase 2](https://www.uschamberfoundation.org/workforce/experience-you-phase-2-final-report) | Field testing across nine partner organizations showing how AI and open data standards can translate real-world experience into portable Learning and Employment Records | How should this translation work when the source experience is evidenced by confidential AI-assisted work records? |
| [JFF digital-wallet field test](https://www.jff.org/blog/veterans-tested-digital-wallets-heres-what-we-learned/) | A small-sample, eight-partner test of moving verified credentials through wallets into a talent platform; it surfaced schema interpretation, synchronization, transfer, device, security-review, and governance-coordination friction | What additional safeguards are needed for employer authorization, protected-evidence custody, reconstruction risk, and offboarding disputes? |
| [W3C PROV](https://www.w3.org/TR/prov-overview/) and [OpenLineage](https://github.com/OpenLineage/OpenLineage) | Provenance and lineage for entities, activities, agents, runs, jobs, and datasets | Who decides authorization, relying-party assessment, review, and remedy? |
| [OpenTelemetry semantic conventions](https://opentelemetry.io/docs/concepts/semantic-conventions/) and [OpenInference](https://github.com/Arize-ai/openinference) | Cross-vendor semantics for traces and AI operations | How should observed work support governed capability claims and evidence items? |
| [EU Platform Work Directive 2024/2831](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024L2831) | Requirements addressing algorithmic-management transparency, explanation, human oversight and review, worker-representative involvement, personal-data protections and portability, and redress | How should broader capability-claim portability be governed without implying that the Directive creates that right? |
| [MyData principles](https://www.mydata.org/wp-content/uploads/2022/07/Understanding-MyData-Operators-2022-1.pdf) | Human-centric control, portability, transparency, accountability, and interoperability | How should applicable restrictions and permissions for protected work artifacts be handled where employment is assumed? |

## What this landscape changes

- Credential packaging, signing, wallet custody, transfer, and presentation
  already have standards and real-world field tests. This project should not
  rebuild them.
- AI memory objects can be inputs to a claim process, but technical
  exportability does not make them authorized portable claims.
- The candidate gap is **governed derivation**: protected workplace evidence →
  generalized capability candidate → disclosure or reconstruction-risk
  assessment → authorization or attestation → reviewable portable claim.

Whether that gap merits a profile over existing standards, a new protocol, or
no new layer remains an open question. Please submit missing projects,
conflicting standards, legal precedents, or evidence that the proposed layer is
unnecessary through the [related-work issue form](https://github.com/yimoburu/worker-knowledge-portability/issues/new/choose).
