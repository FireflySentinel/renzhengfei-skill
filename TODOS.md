# TODOS

## Native Chinese review before v1.0

**What:** Get a native Chinese speaker to review the final SKILL.md before publishing v1.0.

**Why:** The skill's expression DNA and decision heuristics will be in Chinese. A non-native review pass can produce technically correct but tonally awkward Chinese that sounds unnatural to the 即刻/Bilibili audience. Credibility of a skill distilling a Chinese figure depends on sounding authentic in Chinese.

**Pros:** Catches awkward phrasing, overly formal register, or expressions that sound AI-generated. Builds trust with the primary audience.

**Cons:** Requires finding a trusted builder contact willing to spend ~30 min reviewing. Coordination overhead.

**Context:** The primary audience is Chinese tech builders. The skill is in Chinese-first. The expression DNA section in particular encodes Ren's voice — if it sounds like translated English, the skill loses authenticity. A single native speaker pass before v1.0 publish is sufficient; this isn't a formal translation review.

**Depends on:** v1.0 SKILL.md completion (SOURCING.md all boxes checked)

**Where to start:** Find a native speaker in your builder network (即刻 contacts, WeChat). Share the SKILL.md, ask them to flag anything that sounds unnatural or unlike how Chinese engineers actually talk about these concepts.

## Verify 女娲.skill output quality for Ren Zhengfei

**What:** Install 女娲.skill and run it on 任正非 before committing to Approach C. If the output is garbage, switch to Approach B early.

**Why:** The entire hybrid approach (Approach C) depends on 女娲.skill producing a usable scaffold for Ren Zhengfei. This has never been tested. The outside voice in the CEO review flagged this as an unverified load-bearing dependency. A 20-minute test de-risks the entire plan.

**Pros:** Know immediately whether the auto-generate path works. If it doesn't, you save a full review/cleanup cycle by switching to manual writing (Approach B) before investing time.

**Cons:** None. This is pure de-risking.

**Context:** Run `npx skills add alchaincyf/nuwa-skill` then `/nuwa 任正非 Ren Zhengfei`. Review the output for: (1) format correctness, (2) content quality, (3) political content contamination. If output is usable, proceed with Approach C. If not, switch to Approach B (manual write using SKILL.md format spec).

**Effort:** S (human: ~20min / CC: ~20min)

**Priority:** P1 — should be the very first implementation step

**Depends on:** Nothing

## Create CONTENT_BOUNDARY.md

**What:** Create a checklist of topics to scan for and remove from SKILL.md before publishing, plus topics that are IN scope.

**Why:** 任正非 is uniquely positioned at the intersection of tech, geopolitics, and national security. 女娲.skill will pull from interviews where he discusses US sanctions, the Entity List, and China's tech independence. Without a specific checklist, a reviewer might miss subtle political references. This was identified as the plan's main risk in the CEO review.

**Pros:** Makes the content review gate repeatable and explicit. Serves as a template for future Eastern Governance OS skills (Deng Xiaoping, Lee Kuan Yew).

**Cons:** Requires upfront thought about what counts as politically sensitive vs legitimate management philosophy.

**Context:** REMOVE topics: US Entity List/sanctions, US-China tech war, Huawei-government/CCP/PLA relationship, national security positioning, specific geopolitical adversaries, 5G security debate, chip self-sufficiency as geopolitical strategy, quotes framing Huawei as national duty. KEEP topics: management philosophy, organizational design, decision-making frameworks (灰度哲学, 蓝军机制), corporate values (以奋斗者为本), R&D investment philosophy, HR philosophy, business strategy (international expansion as market strategy).

**Effort:** S (human: ~30min / CC: ~5min)

**Priority:** P1 — blocks v0.1 publish (must exist before content review step)

**Depends on:** Nothing

## Expand acceptance test ground truth check

**What:** Check at least 3 claims across different SKILL.md sections against actual primary texts, not just 1.

**Why:** The outside voice in the CEO review flagged that checking only 1 claim is weak. A skill full of plausible-sounding fabrications could pass a single ground truth check. Checking 3 claims across different sections (one mental model, one decision heuristic, one expression DNA phrase) provides much better coverage.

**Pros:** Catches AI hallucinations across the SKILL.md, not just in one lucky spot. Quick to do.

**Cons:** Requires 华为基本法 or 任正非文集 text to be accessible for comparison. Adds ~20 minutes to the acceptance test.

**Context:** Pick one verifiable claim from each of: (1) a mental model definition, (2) a decision heuristic, (3) an expression DNA phrase or anti-pattern. Compare each against the actual primary text. PASS: all 3 match in substance. FAIL on any: investigate whether the section is fabricated vs misattributed.

**Effort:** S (human: ~30min / CC: ~10min)

**Priority:** P2 — improves v0.1 quality gate but not a blocker

**Depends on:** 华为基本法 text being accessible

## Check copyright status of quoting 华为基本法

**What:** Quick research on the IP/copyright status of directly quoting 华为基本法 passages in an open-source GitHub repo.

**Why:** The outside voice in the CEO review raised this. v0.1 (auto-generated) doesn't directly quote primary texts, but v1.0 (source-grounded) will include direct citations. 华为基本法 is widely quoted across hundreds of publications, but formal copyright status is unclear.

**Pros:** Good legal hygiene for v1.0. Avoids potential takedown issues if Huawei IP team objects.

**Cons:** Likely a non-issue given how widely the text is quoted and mirrored. Low risk of wasted research time.

**Context:** Check: (1) Is 华为基本法 under copyright? (2) Is fair use/fair dealing applicable for excerpts in an educational/analytical context? (3) Are existing skills in the ecosystem (steve-jobs-skill, etc.) quoting copyrighted material? If quoting is risky, summarize/paraphrase instead of direct quotes for v1.0.

**Effort:** S (human: ~15min research)

**Priority:** P3 — not a blocker, good hygiene for v1.0 phase

**Depends on:** v1.0 sourcing phase starting
