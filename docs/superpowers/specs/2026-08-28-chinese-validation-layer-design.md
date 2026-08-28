# Chinese Validation Layer Design

**Status:** Approved by the user; implementation planning in progress

**Date:** 2026-08-28

**Project:** Worker Knowledge Portability

**English content baseline:** `399721ad0a4e9c169850eaba8f2fb417d8af1b1e`

## Purpose

Add a small Simplified Chinese discussion layer that tests whether the Worker
Knowledge Portability offboarding question produces serious cross-industry
criticism in Chinese-speaking professional communities. The layer must make the
existing English project understandable without creating a second Charter,
claiming implementation readiness, or implying a right to export protected
organizational knowledge.

The validation objective is substantive falsification, not reach alone. The
project should learn whether the proposed claim-evidence separation, governed
dispositions, and review model survive worker, originating-organization,
receiving-party, legal, security, human-resources, credentialing, and AI-platform
criticism.

## Scope

The public repository receives exactly three Chinese artifacts:

1. `README.zh-CN.md`: a concise Chinese discussion guide.
2. `TERMINOLOGY.zh-CN.md`: a bilingual controlled glossary.
3. `assets/worker-knowledge-portability-ecosystem.zh-CN.svg` and its rendered
   `assets/worker-knowledge-portability-ecosystem.zh-CN.png` download.

`README.md` and `README.zh-CN.md` receive reciprocal `English | 简体中文`
navigation. The Chinese guide links to the existing GitHub Discussion #1; no
parallel Chinese Discussion is created.

The Chinese social launch copy is reviewed in chat and is not committed as a
platform-specific promotional file. Posting it or sending direct outreach
messages requires explicit user approval of the final copy and destination.

## Non-goals

- No full translation of `CHARTER.md`, `GOVERNANCE.md`, `STRESS-TEST.md`, or the
  other normative discussion documents.
- No independent Chinese Charter or independent Chinese governance process.
- No protocol, schema, implementation, pilot, certification program, legal
  opinion, or organizational policy.
- No claim that Chinese law creates a general right to export workplace
  knowledge.
- No automated cross-posting, engagement manipulation, paid promotion, or
  optimization around likes and reposts.
- No mention of NVIDIA, Unified Telemetry, NeMo Relay, CoS, or private internal
  conversations in the public Chinese materials.

## Language authority and versioning

The English files remain the project record. Each Chinese artifact must state
that it is an explanatory discussion edition rather than a legal translation or
separate authoritative Charter.

`README.zh-CN.md` and `TERMINOLOGY.zh-CN.md` must display:

- the English content baseline commit;
- the Chinese publication date;
- a link to the corresponding English source;
- a request to report translation problems; and
- a statement that conflicting meaning should be resolved against the English
  project record at the cited commit.

The Chinese SVG must include the same status in accessible metadata and a short
visible footer. If the English source changes materially after publication, the
Chinese version remains pinned to its cited baseline until reviewed and updated;
it must not silently inherit the new English version.

## Controlled terminology

The Chinese guide uses `从业者` as the umbrella term because it includes
employees and other people performing work without determining legal employment
status. Concrete offboarding examples may use `离职员工` when a legally
recognized employment relationship is actually intended. `劳动者` is reserved
for quotations or jurisdiction-specific legal analysis.

| English term | Chinese discussion term | Boundary |
|---|---|---|
| Worker | 从业者 | Umbrella term; does not determine legal status. |
| Employee | 员工 | Used only for a recognized employment relationship. |
| Worker Knowledge Portability | 从业者知识可携带性 | Project concept, not raw-data export. |
| Worker Knowledge Portability Charter | 从业者知识可携带性原则框架 | Explanatory label; the English Charter remains the project record. |
| Capability claim | 能力声明 | A statement about capability, not the person's capability itself. |
| Protected source material | 受保护的来源材料 | Material subject to confidentiality, privacy, intellectual-property, contractual, security, or other restrictions. |
| Originating organization | 原工作组织 | The source-side organization controlling relevant work systems or records. |
| Attestation | 证明性陈述 | A signed or attributable statement; not technical verification or endorsement of fitness. |
| Verification | 技术核验 | Checks authorship, integrity, technical validity, and status; not truth. |
| Relying-party assessment | 使用方评估 | The receiving party's separate fitness-for-purpose judgment. |
| Governed disposition | 经治理程序确定的处置结果 | A per-object outcome, not a blanket ownership decision for a person or case. |

The four disposition labels are:

1. **保留于受保护的保管环境** — Retained in protected custody.
2. **获准用于特定用途** — Authorized for specified use.
3. **从业者可携带的能力声明** — Worker-portable claim.
4. **受限或争议待决** — Restricted or pending dispute.

The Chinese materials must state prominently:

> 这不是让个人带走公司的知识，也不是让组织在未经治理的情况下永久复制一个人的判断、风格和能力。

## Chinese discussion guide

`README.zh-CN.md` is a standalone, concise introduction rather than a line-by-line
translation. It contains:

1. The concrete AI-assisted offboarding problem.
2. The question: when the relationship ends, what stays, what may follow, and
   who decides?
3. The distinction among a capability claim, protected source evidence,
   attestation, verification, and relying-party assessment.
4. The four per-object governed dispositions.
5. The explanatory-language and no-implementation boundaries.
6. A Chinese response template with perspective, failure mode, why the current
   Charter does not handle it, supporting public evidence, and a
   continue/narrow/stop/investigate recommendation.
7. Links to the English Charter, terminology, stress test, ecosystem, objection
   register, and existing Discussion #1.

The guide must be self-contained enough that a reader can critique the idea
without opening GitHub links first.

## Chinese ecosystem diagram

The Chinese diagram preserves the English diagram's 1600 by 1720 canvas,
geometry, layers, arrows, colors, governed objects, and four dispositions. It
does not add, remove, or reinterpret architectural elements.

The SVG is copied from the current English SVG and translated in place. Its font
stack must support Simplified Chinese, preferring `PingFang SC`,
`Noto Sans CJK SC`, and `Microsoft YaHei` before the existing system sans-serif
fallbacks. Text may wrap or reduce within the existing boxes, but box geometry
and information hierarchy remain recognizable as the same ecosystem.

The title should retain the project identity:

> Worker Knowledge Portability Ecosystem / 从业者知识可携带性生态

Accessible `<title>` and `<desc>` content must be Chinese or bilingual. The PNG
is rendered from the reviewed SVG and remains a directly downloadable artifact.

## Launch narrative

The primary Chinese headline is:

> 公司把离职员工“炼化”成 AI 分身后，什么应该留下，什么可以随人继续？

The subtitle is:

> 一个关于组织知识保护、从业者能力延续与 AI 治理的开放工业问题

The launch article follows five moves:

1. Establish that AI systems can already derive reusable profiles or skills
   from workplace communication and documents.
2. Explain that the same records may mix protected organizational information,
   shared work product, and reusable human judgment.
3. Ask the offboarding question without presuming an ownership answer.
4. Present claim-evidence separation and four per-object dispositions as a
   thought starter rather than a settled solution.
5. Ask readers to break the proposal from worker, originating-organization,
   relying-party, legal, security, HR, credentialing, AI-platform, adversarial,
   and governance perspectives.

The article is native and self-contained. Project links appear at the end as
supporting material. It must not ask for likes, shares, endorsements, or
agreement, and it must not imply that a protocol already exists.

## Distribution sequence

1. Publish the reviewed Chinese GitHub guide, glossary, SVG, and PNG.
2. After explicit approval of the final social copy, publish one substantive
   Zhihu article or answer. Prefer an answer only if a current, relevant question
   already has serious discussion and does not distort the project's framing;
   otherwise publish the standalone article.
3. After explicit approval of recipients and message text, share the article
   personally with 8 to 12 Chinese-speaking critics spanning worker,
   originating-organization, legal, security, HR, credentialing, and AI-platform
   perspectives.
4. Wait for substantive responses before adapting the article for WeChat.
5. Defer Xiaohongshu and Bilibili until the first critique round demonstrates
   that the framing is understandable and worth continuing.

## Feedback handling

Public Chinese feedback may be summarized in English in
`feedback/objection-register.md` when it is substantive. Each entry uses the
existing columns and separately names relevant capability claims, evidence
items, or work artifacts. Its evidence field links to the public source, and the
proposed response preserves uncertainty and dissent.

The register should preserve a short Chinese statement or faithful paraphrase
alongside an English summary when needed to prevent translation loss. Translation
must not strengthen, soften, or convert criticism into endorsement.

Private feedback is not published by default. Names, wording, and identifiable
circumstances require explicit permission. When private feedback materially
changes the Charter or project direction, request permission to publish a safely
generalized summary. Without permission, it may inform private reasoning but
must not be presented as public evidence or consensus.

Do not reproduce confidential information, personal data, trade secrets, private
workplace disputes, or evidence the contributor was not authorized to disclose,
even when it appears in a public comment. Record the safe failure mode without
copying the unsafe material.

## Validation gate

The validation window starts when the Zhihu article is published and lasts 14
calendar days. Success requires all of the following:

- at least five substantive failure modes;
- at least three stakeholder perspectives;
- at least one originating-organization, legal, or security objection; and
- at least one credible recommendation to stop or sharply narrow the project.

Views, likes, reposts, supportive reactions, silence, and private interest do not
count as validation or endorsement.

At the gate, choose one recorded disposition for the project direction:

- **Continue:** the proposed gap survives criticism and multiple stakeholders
  find the distinction useful.
- **Narrow:** evidence supports only a smaller use case, governed object, or
  stakeholder boundary.
- **Investigate:** important evidence remains missing and the current claims
  cannot yet be resolved.
- **Stop:** existing mechanisms solve enough of the problem, or the proposed
  governance cannot become legitimate or safe.

## Verification and acceptance criteria

Before repository publication:

- reciprocal README language links resolve;
- every Chinese controlled term matches `TERMINOLOGY.zh-CN.md`;
- both Chinese documents cite the correct English baseline and date;
- the Chinese guide contains the no-company-knowledge and no-implementation
  boundaries;
- the SVG is well-formed and contains bilingual accessible metadata;
- the PNG is 1600 by 1720 and visually matches the reviewed SVG;
- the diagram is legible at desktop size and at a typical mobile-width preview;
- all project and source links resolve;
- no NVIDIA, Unified Telemetry, NeMo Relay, CoS, private-person, or confidential
  references appear;
- no wording claims legal authority, institutional endorsement, implementation
  readiness, certification, or consensus;
- no new GitHub Discussion or full Chinese Charter is introduced; and
- the complete Git diff contains only the approved language-navigation and
  Chinese validation-layer artifacts plus their design and implementation
  documentation.

Before external publication, the user reviews and explicitly approves the exact
post, account or platform, and any direct-recipient list and message.

## Correction and rollback behavior

Translation or terminology errors are corrected transparently. Update the
Chinese files, their source-baseline marker when applicable, and the repository
change log; do not rewrite public criticism to hide the earlier error.

If the Chinese framing is widely misunderstood as permission to take protected
organizational knowledge, pause distribution, correct the explanatory guide and
headline framing, and record the misunderstanding as validation evidence.

If a platform removes or limits the launch post, do not evade its rules through
duplicate or disguised posting. Preserve the approved repository artifacts and
reassess the distribution channel.

## Self Model synchronization

After repository publication, update the canonical Worker Knowledge Portability
Self Model project page and log with:

- the approved Chinese validation strategy;
- published artifact links and commit;
- the launch date and 14-day gate date;
- verified response counts and stakeholder coverage; and
- the resulting continue, narrow, investigate, or stop decision.

Do not copy private feedback or identify private contributors in the Self Model
unless the content is safe, relevant, and explicitly authorized for that use.

## Implementation boundary

This specification authorizes planning only after written user review. It does
not itself authorize repository implementation, GitHub publication, Zhihu
posting, direct outreach, a protocol, or any reference implementation.
