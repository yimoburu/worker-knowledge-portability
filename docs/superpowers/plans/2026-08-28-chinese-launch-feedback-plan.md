# Chinese Launch and Feedback Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Launch the approved Chinese industrial question through one native Chinese discussion surface, gather governed multi-stakeholder criticism for 14 days, and make an evidence-backed continue, narrow, investigate, or stop decision.

**Architecture:** This operational plan starts only after the Chinese GitHub repository layer is live. Social copy, destination, direct recipients, monitoring, public objection entries, and the final project decision each have separate user gates; private feedback never becomes public evidence without permission.

**Tech Stack:** GitHub Discussions, Zhihu or another explicitly approved Chinese discussion destination, browser or user-assisted publication, Markdown objection register, CoS Self Model

**Spec:** `docs/superpowers/specs/2026-08-28-chinese-validation-layer-design.md`

## Global Constraints

- Start only after the repository plan is published and its live URLs and hashes are verified.
- The primary framing is an open industrial question, not advocacy, anti-company messaging, anti-AI messaging, or a claim that a protocol exists.
- Do not mention NVIDIA, Unified Telemetry, NeMo Relay, CoS, or private internal conversations.
- The post must be native and self-contained; GitHub links appear at the end as supporting material.
- Do not ask for likes, shares, endorsements, agreement, or artificial engagement.
- Do not post or message externally until the user explicitly approves the exact copy, account or platform, and destination or recipient list.
- Public criticism may be recorded with a faithful bilingual summary and source link. Private feedback is not published without explicit permission.
- Do not reproduce personal data, trade secrets, confidential workplace information, private disputes, or evidence the contributor lacks authority to disclose.
- The 14-day validation window begins only when the approved Chinese launch post is live.
- Do not create a recurring monitor or scheduled automation unless the user explicitly requests one.

## File Map

- Read live: `README.zh-CN.md`, `TERMINOLOGY.zh-CN.md`, Chinese diagram, Discussion #1.
- Modify as evidence arrives: `feedback/objection-register.md`.
- Update after repository publication and at the decision gate: `/Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/worker_knowledge_portability.md` and `/Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/log.md`.
- Do not commit platform-specific launch copy to the public repository; present it in chat for review.

---

### Task 1: Choose the Launch Surface and Draft the Native Chinese Post

**Files:**
- Read live: `README.zh-CN.md`
- Read live: `TERMINOLOGY.zh-CN.md`
- No committed output file

**Interfaces:**
- Consumes: Verified live Chinese repository URLs and approved terminology.
- Produces: One exact post draft plus a recommended destination and format for user approval.

- [ ] **Step 1: Verify the repository prerequisite**

Open the live Chinese README, glossary, PNG, and Discussion #1. Confirm each is reachable and the README baseline marker matches the published English baseline. Stop if any artifact is missing or stale.

- [ ] **Step 2: Research the current Zhihu surface**

Search for current substantive questions about `同事.skill`, `离职员工 AI 分身`, `炼化同事`, and workplace AI knowledge ownership. Record candidate URLs, dates, answer counts, and whether the existing framing invites serious industrial criticism.

Selection rule:

- Recommend an answer only when an existing question is current, substantively discussed, and compatible with the project's neutral offboarding question.
- Otherwise recommend a standalone Zhihu article.
- Do not create both in the first round.

- [ ] **Step 3: Draft the exact native post**

Use this approved title and subtitle:

```text
公司把离职员工“炼化”成 AI 分身后，什么应该留下，什么可以随人继续？

一个关于组织知识保护、从业者能力延续与 AI 治理的开放工业问题
```

Open with this argument, polished into natural Chinese without changing its meaning:

```text
当一个人离开组织时，账号可以关闭、设备可以归还、文档可以移交。但如果 AI 已经从他的消息、文档、邮件和工作过程里学会了一部分判断方式，离职交接就不再只是文件归谁的问题。

同一批记录里，可能同时存在组织必须保护的机密、共同形成的工作产物，以及这个人在工作中逐渐形成的可复用技能和判断。把全部内容都视为组织资产，或者全部视为个人可以带走的知识，都过于简单。
```

The body must then:

1. state the offboarding question verbatim from `README.zh-CN.md`;
2. include the sentence `这不是让个人带走公司的知识，也不是让组织在未经治理的情况下永久复制一个人的判断、风格和能力。`;
3. explain capability claim, protected source material, attestation, technical verification, and relying-party assessment using the approved terms;
4. list the four Chinese dispositions exactly;
5. describe them as a thought starter, not a settled architecture or existing protocol;
6. ask for worker, originating-organization, relying-party, legal, security, HR, credentialing, AI-platform, adversarial, and governance failure modes; and
7. end with the Chinese response template and links to the live Chinese README, diagram, terminology, English Charter, and Discussion #1.

Use this closing posture:

```text
我更想听到反例，而不是赞同。如果这个问题已经被现有法律、合同、凭证体系或技术标准解决了，请指出来；如果这套区分在现实中无法执行、会被滥用，或者根本不值得继续，也请直接说明原因。
```

- [ ] **Step 4: Run the editorial checks**

Check the draft manually and report pass/fail for:

- all controlled Chinese terms match `TERMINOLOGY.zh-CN.md`;
- no legal-right claim or implementation-readiness claim;
- no company-specific or internal references;
- no engagement bait;
- no confidential example;
- all source claims have a direct public link; and
- the post is understandable without opening GitHub.

- [ ] **Step 5: Present one destination recommendation and the full exact draft**

Show the user the selected destination, why it passed the selection rule, and the complete final copy. Stop for explicit approval; do not publish.

---

### Task 2: Publish and Establish the Validation Window

**Files:**
- Modify after publication: `/Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/worker_knowledge_portability.md`
- Modify after publication: `/Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/log.md`

**Interfaces:**
- Consumes: Explicit approval of the exact post, platform, and account from Task 1.
- Produces: One `LaunchRecord` with fields `public_post_url: string`, `platform: string`, `account: string`, `published_at: ISO-8601 timestamp`, `validation_start: YYYY-MM-DD`, and `validation_end: YYYY-MM-DD`.

- [ ] **Step 1: Reconfirm the external-write boundary**

Repeat the exact title, destination, and account to the user and obtain explicit approval if any of them changed after Task 1. If browser authentication or manual user action is required, request only that action and preserve the approved copy unchanged.

- [ ] **Step 2: Publish once**

Publish the approved post through the available browser surface or provide the user with the final copy for manual publication. Do not duplicate it across multiple questions, articles, or accounts.

- [ ] **Step 3: Verify the live post**

Open the public URL and compare the rendered title, body, links, and diagram against the approved copy. Record the public URL and publication timestamp. If the platform altered or truncated the copy, report the exact difference and obtain approval before correcting it.

- [ ] **Step 4: Calculate the validation gate**

Set:

```text
validation_start = public post publication date in America/Los_Angeles
validation_end = validation_start + 14 calendar days
```

Do not count repository publication as the start.

- [ ] **Step 5: Update the Self Model with verified launch state**

Use `apply_patch` to add the approved Chinese strategy, repository links and commit, public post URL, verified start date, and gate date. Mark response counts as zero at launch and preserve the continue/narrow/investigate/stop decision as pending. Add a timestamped entry to `log.md`. Do not include private feedback.

- [ ] **Step 6: Verify the Self Model update**

```bash
rg -n 'Chinese|中文|validation|验证|Zhihu|知乎' \
  /Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/worker_knowledge_portability.md \
  /Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/log.md
```

Expected: the new artifact links, exact dates, zero-count launch state, and pending decision are visible.

---

### Task 3: Prepare Targeted Chinese Critic Outreach

**Files:**
- No committed output file

**Interfaces:**
- Consumes: `LaunchRecord.public_post_url` from Task 2 and the approved stakeholder categories.
- Produces: A user-approved recipient list and one copy-ready direct-share message; sending remains separately authorized.

- [ ] **Step 1: Build a candidate matrix**

Propose 8 to 12 candidates covering at least:

- one worker or practitioner perspective;
- one originating-organization or operator perspective;
- one legal or privacy perspective;
- one security or trade-secret perspective;
- one HR or talent perspective;
- one credentialing or standards perspective; and
- one AI platform or agent-tooling perspective.

For each candidate, state only verified role relevance, relationship or channel, and why their criticism would be useful. Do not infer endorsement.

- [ ] **Step 2: Draft one neutral direct-share message**

Use this structure:

```text
我最近在整理一个开放的工业问题：当一个人长期使用 AI 工作并离开组织时，什么材料必须留下，什么经过概括的能力声明可以继续使用，又由谁来判断？

我不是在推一个已经成形的方案，反而想找最强的反例。这里是中文说明和讨论链接：${LaunchRecord.public_post_url}

如果你愿意，我最想听的是：从你的角度看，哪一部分在现实中不可执行、会伤害组织或个人，或者已经被现有机制解决了？
```

Render `${LaunchRecord.public_post_url}` using the exact verified URL from Task 2; do not personalize with unverified claims.

- [ ] **Step 3: Obtain explicit recipient and channel approval**

Present the exact list, message, and channel. If the user does not approve sending, provide copy-ready text only. Do not use another channel as a workaround.

- [ ] **Step 4: Send or hand off exactly once per approved recipient**

Use an available messaging tool only for recipients and channels explicitly approved by the user. Otherwise, hand the message to the user for manual sending. Report sent, prepared-only, failed, and skipped recipients separately.

---

### Task 4: Govern Public and Private Feedback

**Files:**
- Modify when substantive public evidence exists: `feedback/objection-register.md`
- Read: `CHARTER.md`
- Read: `TERMINOLOGY.md`
- Read: `TERMINOLOGY.zh-CN.md`

**Interfaces:**
- Consumes: Public comments or explicitly publishable generalized private feedback.
- Produces: Faithful bilingual `CritiqueRecord` entries using the existing register schema. A `CritiqueRecord` has fields `id`, `chinese_summary`, `english_summary`, `perspective`, `governed_objects`, `dispositions`, `evidence`, `proposed_response`, `charter_change`, `response_status`, `recommendation`, `source_type`, `public_source_url`, and `permission_to_publish`.

- [ ] **Step 1: Classify each response before recording it**

For every response, populate one `CritiqueRecord`:

```text
source_type = public | private
substantive = yes | no
permission_to_publish = yes | no | not-needed-for-public-source
perspective = worker | originating organization | relying party | legal | security | HR | credentialing | AI platform | adversarial | governance | other
recommendation = continue | narrow | investigate | stop | unstated
public_source_url = exact public URL | empty for private feedback
response_status = Open
```

Supportive reaction alone is not substantive. A substantive response identifies a failure mode, missing safeguard, prior-art mechanism, practical impossibility, legitimacy problem, or credible boundary change.

- [ ] **Step 2: Protect unsafe or private material**

Do not copy personal data, trade secrets, confidential workplace material, private disputes, or unauthorized evidence into any project surface. Private feedback requires explicit permission before publication; otherwise it may inform private reasoning but cannot be cited as public evidence or consensus.

- [ ] **Step 3: Add each publishable objection using the existing columns**

Use `apply_patch` to append one row per independently governed objection. Render this row by replacing each `${CritiqueRecord.*}` expression with the corresponding populated field from Step 1:

```markdown
| ${CritiqueRecord.id} | ${CritiqueRecord.chinese_summary} / ${CritiqueRecord.english_summary} | ${CritiqueRecord.perspective} | ${CritiqueRecord.governed_objects} | ${CritiqueRecord.dispositions} | ${CritiqueRecord.evidence} | ${CritiqueRecord.proposed_response} | ${CritiqueRecord.charter_change} | ${CritiqueRecord.response_status} |
```

Increment IDs as `CN-001`, `CN-002`, and so on. Never use one disposition for an entire person or case.

- [ ] **Step 4: Verify and commit each coherent objection batch**

```bash
git diff --check
git diff -- feedback/objection-register.md
git add feedback/objection-register.md
git commit -m "feedback: record Chinese critique batch"
```

Push only after the user reviews any entry derived from private feedback. Public-source entries may follow the already approved objection-register governance, but report the exact commit and live URL after push.

- [ ] **Step 5: Report counts without treating them as consensus**

Maintain verified counts for substantive failure modes, distinct stakeholder perspectives, originating-organization/legal/security objections, and credible stop-or-narrow arguments. Report views and likes separately, if available, and never count them toward validation.

---

### Task 5: Apply the Fourteen-Day Decision Gate

**Files:**
- Read: `feedback/objection-register.md`
- Modify after decision: `/Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/worker_knowledge_portability.md`
- Modify after decision: `/Users/xwli/.cos/workspace/self_model/projects/worker_knowledge_portability/log.md`
- Modify only if evidence changes project direction: `CHARTER.md`, `README.md`, `README.zh-CN.md`, or related public documents under a separately reviewed change

**Interfaces:**
- Consumes: `LaunchRecord.validation_end` from Task 2 plus fourteen days of verified public feedback and authorized evidence.
- Produces: One evidence-backed continue, narrow, investigate, or stop recommendation and synchronized project state.

- [ ] **Step 1: Confirm the gate date has arrived**

Use the publication timestamp recorded in the Self Model. Do not close the gate early because of high or low engagement. If the user wants recurring monitoring before the gate, create it only after a separate explicit scheduling request.

- [ ] **Step 2: Calculate the four required measures**

Report exact counts and source links for:

1. substantive failure modes, target at least `5`;
2. distinct stakeholder perspectives, target at least `3`;
3. originating-organization, legal, or security objections, target at least `1`; and
4. credible stop-or-sharply-narrow recommendations, target at least `1`.

Silence, reactions, and private interest do not satisfy any measure.

- [ ] **Step 3: Recommend one decision**

Apply these rules:

- **Continue** only if all four measures are met and the proposed gap survives the strongest objections.
- **Narrow** when evidence supports only a smaller use case, governed object, or stakeholder boundary.
- **Investigate** when missing evidence prevents a defensible conclusion, even if engagement was high.
- **Stop** when existing mechanisms solve enough of the problem or legitimate, safe governance is not achievable.

List dissent and uncertainty before the recommendation. Do not infer consensus from the decision.

- [ ] **Step 4: Obtain user approval of the recorded decision**

Present the evidence table, strongest objection, unresolved dissent, and recommended disposition. Do not change the public Charter or project status until the user approves the recorded decision.

- [ ] **Step 5: Synchronize the Self Model and public project state**

After approval, use `apply_patch` to record exact counts, stakeholder coverage, strongest objections, evidence links, decision, and next boundary in the canonical Self Model project page and `log.md`. If public documents must change, prepare a separate reviewed diff; do not silently rewrite the Charter or delete dissent.

- [ ] **Step 6: Verify final state**

Confirm the Self Model and public repository agree on the phase, evidence status, and decision. Report any public-document changes, exact commit, and whether further implementation remains unauthorized.

---

### Task 6: Handle Translation, Framing, or Platform Corrections

**Files:**
- Modify when correction evidence exists: `README.zh-CN.md`
- Modify when correction evidence exists: `TERMINOLOGY.zh-CN.md`
- Modify when correction evidence exists: `assets/worker-knowledge-portability-ecosystem.zh-CN.svg`
- Regenerate when the SVG changes: `assets/worker-knowledge-portability-ecosystem.zh-CN.png`
- Modify for every public correction: `CHANGELOG.md`
- Modify when misunderstanding is substantive: `feedback/objection-register.md`

**Interfaces:**
- Consumes: A verified translation error, recurring framing misunderstanding, English-baseline change, or platform moderation event.
- Produces: A transparent correction commit, paused or resumed distribution state, or a documented channel reassessment without evasion.

- [ ] **Step 1: Classify the correction trigger**

Use exactly one primary trigger:

```text
translation_error
controlled_term_error
english_baseline_changed
framing_misunderstood_as_company_knowledge_export
platform_removed_or_limited_post
unsafe_material_appeared_in_feedback
```

Record the public source when safe. Do not copy unsafe material into the diagnosis.

- [ ] **Step 2: Stop the affected distribution path**

For translation, terminology, baseline, or framing failures, pause new social distribution until the Chinese repository artifacts are corrected and reviewed. For platform moderation, do not repost duplicate or disguised content and do not move to another platform without user approval.

- [ ] **Step 3: Prepare the smallest transparent correction**

Use `apply_patch` to correct only the affected Chinese text. If the SVG changes, regenerate and re-verify the PNG using the exact renderer and checks from the repository plan. If the English source changed materially, update the cited baseline only after reviewing the Chinese meaning against that new commit.

Append a dated `CHANGELOG.md` entry that states the affected Chinese artifact, prior wording or issue at a safe level, corrected meaning, and whether the English baseline changed. Do not erase the history of public criticism.

- [ ] **Step 4: Record a substantive misunderstanding as evidence**

When readers repeatedly interpret the project as permission to take protected organizational knowledge, add a faithful, safe objection entry through Task 4. Treat the misunderstanding as validation evidence about the framing, even if the text is corrected.

- [ ] **Step 5: Run the full repository verification and request approval**

Repeat Task 4 of the repository plan, show the exact diff and corrected rendered diagram, and obtain user approval before pushing or editing the live social post.

- [ ] **Step 6: Publish the correction and verify live state**

Push without force only after approval. Verify remote SHA and artifact hashes. If the social platform permits an in-place correction, update only the approved wording and note the correction transparently; otherwise leave the original unavailable and link the corrected repository artifact through an approved channel.
