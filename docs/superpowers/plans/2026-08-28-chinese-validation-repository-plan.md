# Chinese Validation Repository Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a reviewable Simplified Chinese discussion guide, bilingual controlled glossary, and Chinese ecosystem diagram without creating a second Charter or changing the approved ecosystem architecture.

**Architecture:** The English repository remains the project record. A small Chinese presentation layer is pinned to English content baseline `399721ad0a4e9c169850eaba8f2fb417d8af1b1e`, linked through reciprocal README navigation, and validated as an explanatory edition before any remote publication.

**Tech Stack:** Markdown, SVG/XML, PNG, `xmllint`, bundled Node.js with `sharp`, `sips`, Git

**Spec:** `docs/superpowers/specs/2026-08-28-chinese-validation-layer-design.md`

## Global Constraints

- The English files remain the project record; Chinese files are explanatory discussion editions, not legal translations or an independent Charter.
- Add exactly `README.zh-CN.md`, `TERMINOLOGY.zh-CN.md`, `assets/worker-knowledge-portability-ecosystem.zh-CN.svg`, and `assets/worker-knowledge-portability-ecosystem.zh-CN.png`; modify `README.md` only for reciprocal language navigation.
- Do not translate `CHARTER.md`, `GOVERNANCE.md`, `STRESS-TEST.md`, or other normative discussion documents.
- Do not create a Chinese GitHub Discussion, protocol, schema, implementation, pilot, certification program, legal opinion, or organizational policy.
- Public Chinese materials must not mention NVIDIA, Unified Telemetry, NeMo Relay, CoS, or private internal conversations.
- Use `从业者` as the umbrella term; use `员工` only for a recognized employment relationship and reserve `劳动者` for quotations or jurisdiction-specific legal analysis.
- Preserve the English diagram's 1600 by 1720 canvas, geometry, layers, arrows, colors, governed objects, and four dispositions.
- Use `apply_patch` for authored text edits. Mechanical SVG copying and PNG rendering may use dedicated commands.
- Do not push to GitHub until the user has reviewed the rendered Chinese package and explicitly authorized repository publication.

## File Map

- Create `TERMINOLOGY.zh-CN.md`: Chinese controlled vocabulary and translation-status boundary.
- Create `assets/worker-knowledge-portability-ecosystem.zh-CN.svg`: Chinese explanatory diagram source.
- Create `assets/worker-knowledge-portability-ecosystem.zh-CN.png`: rendered downloadable diagram.
- Create `README.zh-CN.md`: self-contained Chinese discussion guide and critique template.
- Modify `README.md`: add only the reciprocal language switch below the title.
- Read `TERMINOLOGY.md`, `CHARTER.md`, `README.md`, and `assets/worker-knowledge-portability-ecosystem.svg` as English source material.

---

### Task 1: Chinese Controlled Glossary

**Files:**
- Create: `TERMINOLOGY.zh-CN.md`
- Read: `TERMINOLOGY.md`

**Interfaces:**
- Consumes: English terminology at baseline `399721ad0a4e9c169850eaba8f2fb417d8af1b1e` and the approved mapping in the design spec.
- Produces: The only Chinese term source used by `README.zh-CN.md` and the Chinese SVG.

- [ ] **Step 1: Run the pre-implementation failure checks**

Run:

```bash
test -f TERMINOLOGY.zh-CN.md
```

Expected: exit status `1` because the Chinese glossary does not exist.

- [ ] **Step 2: Create the glossary with exact authority metadata**

Use `apply_patch` to create `TERMINOLOGY.zh-CN.md` with this heading and status block:

```markdown
# 从业者知识可携带性：中英文术语表

[English](TERMINOLOGY.md) | 简体中文

> 本页是便于公开讨论的中文解释版，不是法律翻译，也不是独立的原则框架。英文项目记录以提交 [`399721ad0a4e9c169850eaba8f2fb417d8af1b1e`](https://github.com/yimoburu/worker-knowledge-portability/tree/399721ad0a4e9c169850eaba8f2fb417d8af1b1e) 为基线。中文发布日期：2026-08-28。如发现中英文含义不一致，请在 [Discussion #1](https://github.com/yimoburu/worker-knowledge-portability/discussions/1) 中指出；解释冲突以该提交下的英文项目记录为准。
```

Add an introductory paragraph stating that the glossary controls wording in the Chinese guide and diagram but does not allocate legal ownership or create portability rights.

- [ ] **Step 3: Add the exact controlled-term table**

Use these rows and boundaries:

```markdown
| English term | 中文讨论用语 | 使用边界 |
|---|---|---|
| Worker | 从业者 | 包括员工及其他为组织或通过组织开展工作的人；不据此判断法律上的雇佣身份。 |
| Employee | 员工 | 仅在明确指依法成立的雇佣关系时使用。 |
| Worker Knowledge Portability | 从业者知识可携带性 | 指受治理的能力声明延续问题，不等于原始数据、记忆或公司知识的导出。 |
| Worker Knowledge Portability Charter | 从业者知识可携带性原则框架 | 中文解释性称呼；英文 Charter 仍是项目记录。 |
| Capability claim | 能力声明 | 关于能力的陈述，不是能力本身，也不自动代表事实或第三方认可。 |
| Protected source material | 受保护的来源材料 | 受到保密、隐私、知识产权、合同、安全或其他限制的来源材料。 |
| Originating organization | 原工作组织 | 控制相关工作系统或记录的来源侧组织，可能是雇主、客户、平台、代理机构或其他组织。 |
| Attestation | 证明性陈述 | 可归因或签署的陈述；不等同于技术核验，也不代表使用目的适配性。 |
| Verification | 技术核验 | 核查作者、完整性、技术有效性和状态；不判断陈述是否真实。 |
| Relying-party assessment | 使用方评估 | 接收方针对特定目的独立作出的适用性判断。 |
| Governed disposition | 经治理程序确定的处置结果 | 针对单个能力声明、证据项或工作产物的结果，不是对整个人或整个案例作出的笼统所有权判断。 |
```

Add the exact four disposition translations:

```markdown
1. **保留于受保护的保管环境** — Retained in protected custody
2. **获准用于特定用途** — Authorized for specified use
3. **从业者可携带的能力声明** — Worker-portable claim
4. **受限或争议待决** — Restricted or pending dispute
```

End with the prominent boundary:

```markdown
> 这不是让个人带走公司的知识，也不是让组织在未经治理的情况下永久复制一个人的判断、风格和能力。
```

- [ ] **Step 4: Verify the glossary**

Run:

```bash
test -f TERMINOLOGY.zh-CN.md
rg -F '399721ad0a4e9c169850eaba8f2fb417d8af1b1e' TERMINOLOGY.zh-CN.md
rg -F '| Worker | 从业者 |' TERMINOLOGY.zh-CN.md
rg -F '| Capability claim | 能力声明 |' TERMINOLOGY.zh-CN.md
rg -F '| Originating organization | 原工作组织 |' TERMINOLOGY.zh-CN.md
rg -F '**受限或争议待决**' TERMINOLOGY.zh-CN.md
rg -F '这不是让个人带走公司的知识' TERMINOLOGY.zh-CN.md
git diff --check
```

Expected: every `rg` prints one matching line; `git diff --check` prints nothing.

- [ ] **Step 5: Commit the glossary**

```bash
git add TERMINOLOGY.zh-CN.md
git commit -m "docs: add Chinese terminology guide"
```

---

### Task 2: Chinese Ecosystem Diagram

**Files:**
- Create: `assets/worker-knowledge-portability-ecosystem.zh-CN.svg`
- Create: `assets/worker-knowledge-portability-ecosystem.zh-CN.png`
- Read: `assets/worker-knowledge-portability-ecosystem.svg`
- Read: `TERMINOLOGY.zh-CN.md`

**Interfaces:**
- Consumes: Exact Chinese terms from `TERMINOLOGY.zh-CN.md` and geometry from the English SVG.
- Produces: Chinese SVG/PNG paths consumed by `README.zh-CN.md`.

- [ ] **Step 1: Run the diagram failure checks**

```bash
test -f assets/worker-knowledge-portability-ecosystem.zh-CN.svg
test -f assets/worker-knowledge-portability-ecosystem.zh-CN.png
```

Expected: both commands exit `1`.

- [ ] **Step 2: Create the Chinese SVG from the reviewed English source**

Mechanically copy the SVG, then use `apply_patch` for authored changes:

```bash
cp assets/worker-knowledge-portability-ecosystem.svg assets/worker-knowledge-portability-ecosystem.zh-CN.svg
```

Change `<title>` to `Worker Knowledge Portability Ecosystem / 从业者知识可携带性生态`. Change `<desc>` to a bilingual description of the same stakeholder, Charter, open-protocol, potential-implementation, assurance-and-governance, and four-disposition flow.

Prepend the font stacks for `.title`, `.subtitle`, `.section`, `.label`, `.small`, `.tiny`, `.coretext`, and `.coretiny` with:

```css
"PingFang SC", "Noto Sans CJK SC", "Microsoft YaHei",
```

- [ ] **Step 3: Replace every visible English text node using this map**

Preserve all coordinates and non-text elements. Use these exact Chinese labels, splitting only where the English SVG already uses multiple lines:

```text
Worker Knowledge Portability Ecosystem => Worker Knowledge Portability Ecosystem / 从业者知识可携带性生态
Open rules, multiple potential implementations, independent assurance, and governed claim and evidence dispositions => 开放规则 · 多种潜在实现 · 独立保障 · 能力声明与证据的治理处置
Stakeholders => 利益相关方
Workers => 从业者
portable capability claims => 可携带的能力声明
Originating organizations => 原工作组织
protected evidence custody => 受保护证据的保管
AI providers and operators => AI 提供方与运营方
interoperability => 互操作性
Worker representative bodies => 从业者代表组织
collective governance => 集体治理
Independent oversight bodies => 独立监督机构
review and remedy => 审查与救济
1 · Worker Knowledge Portability Charter => 1 · 从业者知识可携带性原则框架
Worker capability agency => 从业者的能力主体性
transparency · recognition · mobility => 透明 · 认可 · 流动
Protected organizational information => 受保护的组织信息
secrecy · work product · evidence => 保密 · 工作产物 · 证据
Claim–evidence separation => 能力声明与证据分离
no blanket ownership · no extraction => 不作笼统所有权判断 · 不提取受保护来源
Review, appeal, and remedy => 审查 · 申诉 · 救济
procedural safeguards · evidence · no retaliation => 程序保障 · 证据 · 禁止报复
2 · Open protocol => 2 · 开放协议
Governed capability-claim schema => 受治理的能力声明模式
portable claims—not replayable memory => 可携带的是声明，不是可重放记忆
Claim-level provenance => 声明级来源记录
source · author · derivation · evidence => 来源 · 作者 · 推导 · 证据
Restrictions, permissions, and attestation status => 限制 · 许可 · 证明性陈述状态
access · use · authorization · review => 访问 · 使用 · 授权 · 审查
Disclosure-minimizing abstraction => 最小化披露的抽象
requirements => 要求
reduce protected-source disclosure risk => 降低受保护来源的披露风险
Separate claim, attestation, authorization, => 能力声明 · 证明性陈述 · 授权
and evidence lifecycles => 与证据分别管理生命周期
claim · attestation · authorization · evidence => 声明 · 证明性陈述 · 授权 · 证据
Review, dispute, and decision records => 审查 · 争议 · 决定记录
decisions remain inspectable => 决定始终可供检查
3 · Potential implementations, until a normative protocol exists => 3 · 规范协议形成前的潜在实现
Worker-controlled claim repository => 从业者控制的声明存储库
portable claim custody => 可携带声明的保管
Protected source evidence repository => 受保护来源证据存储库
protected evidence custody => 受保护证据的保管
Abstraction and disclosure-risk services => 抽象与披露风险服务
propose · abstract · explain => 提议 · 抽象 · 解释
Platform adapters => 平台适配器
AI · HR · knowledge · identity systems => AI · 人力资源 · 知识 · 身份系统
Offboarding and review systems => 离职交接与审查系统
4 · Assurance and governance ecosystem => 4 · 保障与治理生态
Conformance tests => 符合性测试
test process and safeguards => 测试流程与保障措施
Independent conformance assessment => 独立符合性评估
assess published requirements => 依据公开要求进行评估
Policy profiles => 政策配置
local rules above a common floor => 在共同底线之上的本地规则
Collective representation => 集体代表机制
guilds · unions · data trusts => 行业组织 · 工会 · 数据信托
Decision-and-rationale registry => 决定及理由登记册
Per-governed-object disposition process => 逐治理对象的处置流程
Each claim, evidence item, or artifact receives its own disposition; => 每个能力声明、证据项或工作产物分别获得处置结果；
one case may contain several dispositions => 同一案例可以包含多种处置结果
Retained in protected custody => 保留于受保护的保管环境
protected source material remains in custody => 受保护的来源材料继续留在保管环境中
Authorized for specified use => 获准用于特定用途
stated purpose, scope, and conditions => 明确目的 · 范围 · 条件
Worker-portable claim => 从业者可携带的能力声明
provenance and status visible => 来源和状态可见
Restricted or pending dispute => 受限或争议待决
authorization, evidence, or claim unresolved => 授权、证据或声明尚未解决
Principles first · worker-centered · multi-stakeholder · vendor-neutral · evidence-seeking => 原则优先 · 以从业者为中心 · 多方参与 · 厂商中立 · 寻求证据
```

Add a visible footer above the existing bottom line in a smaller font:

```text
中文解释版 · 英文内容基线 399721a · 2026-08-28
```

If the footer collides with the existing line, move only the two footer text baselines within the bottom whitespace; do not change canvas dimensions or disposition boxes.

- [ ] **Step 4: Verify XML validity and geometric equivalence**

```bash
xmllint --noout assets/worker-knowledge-portability-ecosystem.zh-CN.svg
diff \
  <(rg '^\s*<(rect|path)' assets/worker-knowledge-portability-ecosystem.svg) \
  <(rg '^\s*<(rect|path)' assets/worker-knowledge-portability-ecosystem.zh-CN.svg)
```

Expected: `xmllint` exits `0`; `diff` prints nothing. If the footer requires a new text node, this comparison still passes because it intentionally compares only geometry.

- [ ] **Step 5: Render the PNG with the bundled `sharp` dependency**

```bash
bundle_node="/Users/xwli/.cache/codex-runtimes/codex-primary-runtime/dependencies/node/bin/node"
bundle_node_modules="/Users/xwli/.cache/codex-runtimes/codex-primary-runtime/dependencies/node/node_modules"
NODE_PATH="$bundle_node_modules" "$bundle_node" - <<'NODE'
const sharp = require('sharp');
sharp('assets/worker-knowledge-portability-ecosystem.zh-CN.svg')
  .png()
  .toFile('assets/worker-knowledge-portability-ecosystem.zh-CN.png')
  .then(info => {
    if (info.width !== 1600 || info.height !== 1720) {
      throw new Error(`unexpected dimensions ${info.width}x${info.height}`);
    }
  });
NODE
sips -g pixelWidth -g pixelHeight assets/worker-knowledge-portability-ecosystem.zh-CN.png
```

Expected: `pixelWidth: 1600` and `pixelHeight: 1720`.

- [ ] **Step 6: Inspect the rendered diagram**

Open `assets/worker-knowledge-portability-ecosystem.zh-CN.png` with the local image viewer. Check every box at original size and a mobile-width preview. Reject clipped glyphs, missing CJK glyphs, overlapping footer text, ambiguous disposition labels, or changes to the ecosystem structure.

- [ ] **Step 7: Commit the diagram pair**

```bash
git add assets/worker-knowledge-portability-ecosystem.zh-CN.svg \
  assets/worker-knowledge-portability-ecosystem.zh-CN.png
git diff --cached --check
git commit -m "docs: add Chinese ecosystem diagram"
```

---

### Task 3: Chinese Discussion Guide and Language Navigation

**Files:**
- Create: `README.zh-CN.md`
- Modify: `README.md`
- Read: `CHARTER.md`
- Read: `TERMINOLOGY.zh-CN.md`
- Read: `assets/worker-knowledge-portability-ecosystem.zh-CN.png`

**Interfaces:**
- Consumes: Chinese terms from Task 1 and diagram paths from Task 2.
- Produces: The Chinese public entry point and reciprocal discovery from the English README.

- [ ] **Step 1: Run the navigation and guide failure checks**

```bash
test -f README.zh-CN.md
rg -F '[简体中文](README.zh-CN.md)' README.md
```

Expected: the first command exits `1`; the second finds no match and exits `1`.

- [ ] **Step 2: Add reciprocal navigation to the English README**

Use `apply_patch` to insert this line immediately after `# Worker Knowledge Portability`:

```markdown
English | [简体中文](README.zh-CN.md)
```

Do not otherwise rewrite `README.md`.

- [ ] **Step 3: Create the Chinese discussion guide**

Use `apply_patch` to create `README.zh-CN.md` with this exact structure and core copy:

```markdown
# 从业者知识可携带性

[English](README.md) | 简体中文

> 本页是便于公开讨论的中文解释版，不是法律翻译，也不是独立的原则框架。英文项目记录以提交 [`399721ad0a4e9c169850eaba8f2fb417d8af1b1e`](https://github.com/yimoburu/worker-knowledge-portability/tree/399721ad0a4e9c169850eaba8f2fb417d8af1b1e) 为基线。中文发布日期：2026-08-28。如有含义冲突，以该提交下的英文项目记录为准。

AI 辅助工作会产生混合记录。同一条 AI 使用记录可能同时包含组织机密、共同形成的工作产物，以及从业者在工作中发展出的可复用技能和判断。把整条记录简单归为“全部属于组织”或“全部可以随人带走”，都过于粗糙。

这里的**从业者**包括员工及其他为组织或通过组织开展工作的人；这个称呼不决定任何人的法律雇佣身份。

本项目首先追问一个更窄、也更困难的工业问题：

> **当一段工作关系结束时，什么必须留在受保护的保管环境中，什么能力声明可以在其他地方呈现，又由谁来决定？**

> **这不是让个人带走公司的知识，也不是让组织在未经治理的情况下永久复制一个人的判断、风格和能力。**

本项目当前只有一份以原则为先的英文 Worker Knowledge Portability Charter。它未来可能为开放协议、潜在实现和独立治理机制提供参考，但今天不授权任何实现。

![从业者知识可携带性生态](assets/worker-knowledge-portability-ecosystem.zh-CN.png)

[下载中文生态图 PNG](assets/worker-knowledge-portability-ecosystem.zh-CN.png) · [查看中文 SVG](assets/worker-knowledge-portability-ecosystem.zh-CN.svg)

## 离职压力测试

设想一名从业者长期使用 AI 完成工作。相关记录可能混合：

- 受保护的组织或第三方信息；
- 受到合同或法律限制的工作产物；
- 能够支持其可复用技能与判断的证据；
- 来源、限制或权限无法清楚解决的材料。

从业者希望向新的组织呈现经过概括的能力声明，而不转移受保护的来源材料。原工作组织必须保护受到限制的信息。接收方还必须能够区分从业者的自我声明、第三方证明性陈述、技术核验，以及使用方评估（针对特定用途作出的独立判断）。

## 当前原则框架提出什么

- 能力声明、证据项和工作产物是彼此分开的治理对象。
- 保管材料并不自动决定所有权或可携带性。
- 技术核验只检查作者、完整性、技术有效性和状态，不判断陈述是否真实。
- 能力声明可以是自我声明、获得证明性陈述、受到质疑、被撤回或被后续版本替代。
- 证明性陈述与授权可以暂停、撤销、过期或被替代；一个人已经具备的能力本身不能被“撤销”。
- 混合或有争议的证据不能被任何一方单方面移动。

## 四种逐对象处置结果

每个能力声明、证据项或工作产物分别获得一种处置结果；同一案例可以同时包含多种结果：

1. **保留于受保护的保管环境**
2. **获准用于特定用途**
3. **从业者可携带的能力声明**
4. **受限或争议待决**

## 请尝试推翻它

这个项目寻求批评，而不是背书。特别希望看到足以让项目缩小范围或停止的有力论证。

请从以下任一角度提出失败模式：从业者、原工作组织、接收方、法律、安全、人力资源、能力凭证、AI 平台、对抗性使用或治理。

建议的回复格式：

- **视角：**
- **失败模式：**
- **当前原则框架为什么没有处理好：**
- **公开证据或相关项目：**
- **建议：继续 / 缩小范围 / 停止 / 继续调查**

请使用合成或经过安全概括的例子。不要提交个人数据、商业秘密、工作场所机密、私人争议或无权披露的证据。

[进入 Discussion #1：当从业者在 AI 辅助工作后离开时，什么会失败？](https://github.com/yimoburu/worker-knowledge-portability/discussions/1)

## 相关材料

- [英文 Charter v0.2](CHARTER.md)
- [中文术语表](TERMINOLOGY.zh-CN.md)
- [英文术语表](TERMINOLOGY.md)
- [离职压力测试](STRESS-TEST.md)
- [生态说明](ECOSYSTEM.md)
- [相关工作](LANDSCAPE.md)
- [异议登记册](feedback/objection-register.md)

本项目是一份独立的思想起点，不是雇主政策、厂商产品、法律意见、得到背书的标准，也不表示任何实现已经准备就绪。
```

- [ ] **Step 4: Verify terminology and navigation**

```bash
test -f README.zh-CN.md
rg -F 'English | [简体中文](README.zh-CN.md)' README.md
rg -F '[English](README.md) | 简体中文' README.zh-CN.md
rg -F '能力声明' README.zh-CN.md
rg -F '原工作组织' README.zh-CN.md
rg -F '技术核验' README.zh-CN.md
rg -F '使用方评估' README.zh-CN.md
rg -F '这不是让个人带走公司的知识' README.zh-CN.md
rg -F 'assets/worker-knowledge-portability-ecosystem.zh-CN.png' README.zh-CN.md
rg -F 'https://github.com/yimoburu/worker-knowledge-portability/discussions/1' README.zh-CN.md
git diff --check
```

Expected: every `rg` prints exactly one intended match or one intended navigation line; `git diff --check` prints nothing.

- [ ] **Step 5: Commit the guide and navigation**

```bash
git add README.md README.zh-CN.md
git commit -m "docs: add Chinese discussion guide"
```

---

### Task 4: Integrated Prepublication Verification

**Files:**
- Verify: `README.md`
- Verify: `README.zh-CN.md`
- Verify: `TERMINOLOGY.zh-CN.md`
- Verify: `assets/worker-knowledge-portability-ecosystem.zh-CN.svg`
- Verify: `assets/worker-knowledge-portability-ecosystem.zh-CN.png`

**Interfaces:**
- Consumes: All repository deliverables from Tasks 1 through 3.
- Produces: A reviewable local commit set and exact verification evidence for the publication gate.

- [ ] **Step 1: Verify the approved file scope**

```bash
git diff --name-status 399721ad0a4e9c169850eaba8f2fb417d8af1b1e..HEAD
```

Expected: only the approved Chinese files, the single `README.md` navigation change, and approved design/plan documentation appear. No Charter, governance, stress-test, Discussion, code, or schema file changes appear.

- [ ] **Step 2: Scan public Chinese artifacts for prohibited internal framing**

```bash
if rg -n 'NVIDIA|Unified Telemetry|NeMo Relay|CoS|统一遥测|英伟达' \
  README.zh-CN.md TERMINOLOGY.zh-CN.md \
  assets/worker-knowledge-portability-ecosystem.zh-CN.svg; then
  echo 'prohibited internal framing found' >&2
  exit 1
fi
```

Expected: no matches and exit status `0`.

- [ ] **Step 3: Verify XML, PNG dimensions, and geometry again**

```bash
xmllint --noout assets/worker-knowledge-portability-ecosystem.zh-CN.svg
sips -g pixelWidth -g pixelHeight assets/worker-knowledge-portability-ecosystem.zh-CN.png
diff \
  <(rg '^\s*<(rect|path)' assets/worker-knowledge-portability-ecosystem.svg) \
  <(rg '^\s*<(rect|path)' assets/worker-knowledge-portability-ecosystem.zh-CN.svg)
```

Expected: valid XML, `1600` by `1720`, and no geometry diff.

- [ ] **Step 4: Check repository-relative links**

Run this read-only checker:

```bash
python3 - <<'PY'
from pathlib import Path
import re

for name in ('README.md', 'README.zh-CN.md', 'TERMINOLOGY.zh-CN.md'):
    text = Path(name).read_text()
    for target in re.findall(r'\[[^]]+\]\(([^)]+)\)', text):
        if target.startswith(('http://', 'https://', '#')):
            continue
        path = (Path(name).parent / target.split('#', 1)[0]).resolve()
        if not path.exists():
            raise SystemExit(f'{name}: missing relative target {target}')
print('relative-links: ok')
PY
```

Expected: `relative-links: ok`.

- [ ] **Step 5: Check required public URLs**

```bash
for url in \
  'https://github.com/yimoburu/worker-knowledge-portability/tree/399721ad0a4e9c169850eaba8f2fb417d8af1b1e' \
  'https://github.com/yimoburu/worker-knowledge-portability/discussions/1'; do
  curl -fsSL -o /dev/null "$url"
done
```

Expected: both requests exit `0`.

- [ ] **Step 6: Perform final visual review**

Open both English and Chinese PNGs side by side at original resolution. Confirm identical structure, no clipped Chinese glyphs, readable box hierarchy, correct four dispositions, and an unobtrusive baseline footer. Also inspect the Chinese PNG at approximately 390 CSS pixels wide.

- [ ] **Step 7: Present the local package for user approval**

Show the Chinese PNG and link the Chinese README and glossary. Report the exact local `HEAD`, the remote `main` SHA, the file list, and all verification results. Stop before pushing.

---

### Task 5: Publish the Repository Layer

**Files:**
- Publish: the reviewed local commits only

**Interfaces:**
- Consumes: Explicit user approval of the exact local package from Task 4.
- Produces: A verified live GitHub `main` with the Chinese discussion layer.

- [ ] **Step 1: Reconfirm the publication boundary**

Run:

```bash
git status --short --branch
git log --oneline origin/main..HEAD
git diff --check origin/main..HEAD
```

Expected: clean worktree, only reviewed commits ahead of `origin/main`, and no whitespace errors.

- [ ] **Step 2: Push only after explicit user approval**

```bash
git push origin main
```

Expected: push succeeds without force.

- [ ] **Step 3: Verify live state**

```bash
local_sha="$(git rev-parse HEAD)"
remote_sha="$(git ls-remote origin refs/heads/main | awk '{print $1}')"
test "$local_sha" = "$remote_sha"
remote_png="https://raw.githubusercontent.com/yimoburu/worker-knowledge-portability/main/assets/worker-knowledge-portability-ecosystem.zh-CN.png"
curl -fsSL "$remote_png" | shasum -a 256
shasum -a 256 assets/worker-knowledge-portability-ecosystem.zh-CN.png
```

Expected: local and remote SHAs match; remote and local PNG hashes match.

- [ ] **Step 4: Report the published URLs**

Report direct links to `README.zh-CN.md`, `TERMINOLOGY.zh-CN.md`, the Chinese PNG, the Chinese SVG, and Discussion #1. Do not claim that the social launch or validation window has started.
