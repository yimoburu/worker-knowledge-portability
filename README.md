# Worker Knowledge Portability

English | [简体中文](README.zh-CN.md)

> An open discussion draft for separating a portable worker capability claim from protected originating-organization evidence.

AI-assisted work produces composite records. A single AI-assisted work record may contain employer-confidential knowledge, shared work product, and reusable skills or judgment developed by a worker. Treating the whole record as either employer-owned or worker-portable is too crude.

Here, a **worker** is a natural person performing work for or through an organization, whether or not they are an employee. An **employee** is a worker in a legally recognized employment relationship, and an **employer** is that relationship's counterpart. The **originating organization** is the broader source-side organization controlling relevant work systems or records; it may be an employer, client, platform, agency, partnership, or another organization.

This project asks a narrower and harder question:

> **When a worker leaves, what stays, what may follow, and who decides?**

The proposal begins with a principles-first **Worker Knowledge Portability Charter**. It may later inform an open protocol, potential implementations, and independent assurance and governance institutions, but it does not authorize any implementation today.

AI memory portability and worker knowledge portability are not synonyms.
Technically exportable conversations, agent state, reusable prompt patterns,
knowledge-graph entries, and model-generated summaries may be used to propose
or support a capability claim, but they do not automatically become authorized
portable claims. The current investigation asks whether existing credential
and provenance standards need an additional workplace confidential-evidence
profile; it does not assume that a new protocol is required.

![Worker Knowledge Portability Ecosystem](assets/worker-knowledge-portability-ecosystem.png)

## The offboarding test

A worker asks to carry a generalized capability claim developed through AI-assisted work.

- The former employer retains confidential sources and protected evidence.
- The worker may carry a generalized capability claim assessed under a defined policy, method, and threat model to reduce protected-source disclosure or reconstruction risk.
- A receiving organization can inspect whether the claim is self-asserted or attested; a verifier can check authorship, integrity, technical validity, and status; and a relying party separately assesses fitness for purpose.
- Mixed or disputed evidence cannot move unilaterally.
- Delay cannot silently erase a visibly self-asserted and not independently attested worker claim that has been assessed under the stated disclosure-minimization policy, method, and threat model.

The governed dispositions are:

1. **Retained in protected custody**
2. **Authorized for specified use**
3. **Worker-portable claim**
4. **Restricted or pending dispute**

Dispositions apply per governed object and can coexist in one case. Claims and evidence may have different custody, applicable restrictions and permissions, attestation, verification, authorization, relying-party assessment, and review status.

## Start here

- [Charter v0.2.2](CHARTER.md) - proposed rights, safeguards, procedures, governance, and red lines
- [Terminology](TERMINOLOGY.md) - controlled vocabulary and governed dispositions
- [Change log](CHANGELOG.md) - discussion-draft version history
- [Ecosystem](ECOSYSTEM.md) - charter, future protocol, potential implementations, and assurance and governance
- [Stress test](STRESS-TEST.md) - the offboarding scenario and five questions for critics
- [Related landscape](LANDSCAPE.md) - adjacent standards and the proposed missing layer
- [Governance](GOVERNANCE.md) - how this discussion draft records decisions and dissent
- [Contributing](CONTRIBUTING.md) - how to challenge, amend, or add related work
- [Objection register](feedback/objection-register.md) - public record of substantive criticism and disposition

## Feedback wanted

This project is asking for criticism, not endorsement.

[Start with the first adversarial Discussion: **Break the Charter: What fails when a worker leaves after AI-assisted work?**](https://github.com/yimoburu/worker-knowledge-portability/discussions/1)

Please identify:

1. A worker right that is missing, unsafe, or impractical.
2. A legitimate originating-organization interest that remains exposed.
3. A way a worker, originating organization, AI provider or operator, reviewer, or conformity-assessment or certification body could game the process.
4. A governance role that lacks legitimacy or independence.
5. Evidence that the project should continue, narrow, or stop.

Use [GitHub Discussions](https://github.com/yimoburu/worker-knowledge-portability/discussions) for open-ended conversation or choose a structured [issue template](https://github.com/yimoburu/worker-knowledge-portability/issues/new/choose).

Do not submit confidential workplace information, personal data, trade secrets, or examples that you are not authorized to disclose.

## Status and independence

This repository is an independent thought starter. It is not an employer policy, vendor product, legal opinion, endorsed standard, or claim that implementation is ready. Its first objective is to determine whether a real cross-industry gap exists.

## License

Except where noted otherwise, the documents and diagrams in this repository are available under the [Creative Commons Attribution 4.0 International License](LICENSE.md).
