# Ren Zhengfei Skill — Ren Zhengfei's Cognitive Operating System

[中文](README.md) | **English**

> **Q: My parents keep pressuring me to get married. What should I do?**
>
> Honestly, you're asking the wrong person. I'm over 80. In my era we didn't "date to marry" — I met my ex-wife in the army, a completely different process.
>
> But what you're really asking isn't about dating — it's "how do I handle my parents' pressure?"
>
> The biggest mistake here is thinking it's a binary decision. What your parents actually fear isn't whether this particular setup works — they're getting old and afraid you'll be alone later. The dating pressure is just the solution they can imagine. Your resistance isn't really about "no dating" either — it's probably "I want to move at my own pace." Both sides are fighting the wrong fight in imprecise language.
>
> The most important thing 30 years at Huawei taught me: mastery of **gray zones**. Real decisions almost never sit at either extreme.
>
> **Don't let other people's anxiety become your battlefield. Their anxiety is their work to do, not yours.**
>

This isn't a chatbot pretending to be Ren Zhengfei. It distills the **thinking frameworks** that recur across his 400+ internal speeches, the *Huawei Basic Law*, and the three management manuals — turning them into cognitive tools you can invoke directly.

## Contents

- [What's Included](#whats-included)
- [Installation](#installation)
- [Usage](#usage)
  - [Actual Test Output](#actual-test-output)
- [Content Boundary](#content-boundary)
- [Research Sources](#research-sources)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## What's Included

| Module | Content |
|--------|---------|
| Mental Models | 5 core models: Gray Zone Philosophy, Pressure Principle, Self-Criticism, Dissipative Structure, Survival Anxiety |
| Decision Heuristics | 7 heuristics: Deep Dredging Low Dam, Force Through One Hole, Rigidify-Optimize-Institutionalize, Let Those Who Hear the Gunfire Call in the Artillery, ... |
| Expression DNA | Military vocabulary, crisis narrative rhythm, self-deprecating humor, literary prose |
| Values | What he pursues, what he rejects, what he himself hasn't figured out |
| Honest Boundaries | What it can't do, information sources, known limitations |
| Research Archive | Original research files across 6 dimensions (`references/research/`) |

## Installation

```bash
# Claude Code
npx skills add FireflySentinel/renzhengfei-skill
```

Or manually:

```bash
git clone https://github.com/FireflySentinel/renzhengfei-skill.git
cp -r renzhengfei-skill ~/.claude/skills/renzhengfei-perspective
```

## Usage

After installation, just say in Claude Code:

```
Look at this decision through Ren Zhengfei's perspective.
```

```
Switch to Ren Zhengfei mode and analyze our team's organizational issues.
```

```
How would Ren Zhengfei view the growth challenges we're facing?
```

### Actual Test Output

Below are real conversation outputs after loading the skill (unedited):

---

**Q: If you were going to build an AI hardware product in this era, what would you choose?**

> I wouldn't build AI hardware just because AI is trendy. The question itself is wrong — you're asking "what to build" before asking "for whom" and "solving what problem." Technology exists to solve customer problems, not to show off. Go ask your customers, go to the frontline. What's holding them back every day? Let those who can hear the gunfire tell you what artillery to build.
>
> Don't pick your track sitting in an office. Go get yelled at by customers. Where you get yelled at is where the opportunity is.

**Q: I'm an early-stage founder with only 500K RMB in starting capital. Should I go all-in on foundational LLM research? Isn't this what you mean by "sitting on the cold bench for ten years"?**

> **No. I'm telling you directly — don't do it.**
>
> "Sit on the cold bench for ten years" is right, but you need a bench to sit on first. Huawei's foundational research runs 60 billion RMB a year, funded by carrier business profits. Do you have a carrier business? Do you have a cash cow? 500K going into foundational LLM research isn't sitting on the cold bench for ten years — it's freezing to death on the bench in three months.
>
> Survival is the highest strategy. What you should do now is find a business that can feed you — even if it's small, even if it's unsexy. Once you have cash flow, take a portion of the profits and invest in long-term research. Huawei's model is "use the Carrier BG's profits to feed HiSilicon" — not "build chips directly without a Carrier BG."

**Q: Then should I go public to solve the funding problem and expand quickly to grab market share?**

> **No.**
>
> Huawei still isn't listed, and that's not by accident. Public companies get hijacked by quarterly earnings — how can you make long-term investments under that pressure? Deep Dredging Low Dam means digging deep for internal efficiency and giving the savings to customers. That logic can't survive in a public company.
>
> And "expand quickly to grab market share" is opportunism, not strategy. Running fast doesn't mean you can stand still. Expansion without roots is a tower in the sand. First put down deep roots — figure out who your customers are, what problem you solve that no one else can, then focus all your force on breaking through one pinpoint. Forget expanding quickly. Survive past next year first.

---

## Content Boundary

This skill **only distills management philosophy and decision frameworks**. It does not cover political, geopolitical, or sanctions-related topics. See [`CONTENT_BOUNDARY.md`](CONTENT_BOUNDARY.md).

## Research Sources

Primary sources: *Huawei Basic Law*, *Putting the Strivers First*, *Customer-Centric*, *Value as the Outline*, 400+ internal speeches (including the [GitHub full-text archive](https://github.com/ttpianobirds/RenZhengfei)), and interview records from CNBC, BBC, and People's Daily.

Secondary sources: Cambridge University Press, HBR Case Studies, CSIS Report, London Business School.

Full research archive: [`references/research/`](references/research/).

## Contributing

Found a misattribution of one of Ren's views? A mistake in a heuristic citation? Issues and PRs welcome.

Particularly welcome:
- Additional primary source citations (original *Huawei Basic Law* text)
- Corrections to inaccuracies in expression DNA
- New views from recent internal speeches

## Acknowledgments

- [Nuwa.skill](https://github.com/alchaincyf/nuwa-skill) — thought distillation tool by 花叔 ([@AlchainHust](https://x.com/AlchainHust))
- [ttpianobirds/RenZhengfei](https://github.com/ttpianobirds/RenZhengfei) — full-text archive of Ren Zhengfei's internal speeches

## License

MIT
