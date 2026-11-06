# Feynman Learning

A Claude skill that teaches any topic using the Feynman Technique, so you understand it well enough to explain it, instead of just reading about it.

## Why this exists

Passive reading creates a feeling of knowing that fades within days. The Feynman Technique works because it forces *self-explanation* and *retrieval practice*: you only understand something if you can explain it simply, in your own words, without notes.

This skill turns that into a guided conversation. Claude teaches in small steps and makes you do the thinking at the points where learning actually happens.

## How it works

The skill runs as a conversation, one stage at a time. You respond at each stage, so it never turns into a lecture.

| Stage | What happens |
|---|---|
| **1. Baseline** | You write what you already know, however messy. Nothing is taught yet. This exposes your real starting point. |
| **2. Teach it simply** | Claude explains the concept in plain language with a concrete analogy, building on your baseline. Then you explain it back in your own words. |
| **3. Find the gaps** | Claude names what you got right, points out vague spots or unexplained jargon, probes with "why" and "what if" questions, and re-teaches only the weak parts. |
| **4. Test without notes** | You answer application questions (new scenarios, "what would break if...", comparisons). You then get a spaced-review plan: re-explain from memory after 1 day, 3 days and 1 week. |

### Example

> **You:** Teach me how DNS works.
>
> **Claude:** Let's do this the Feynman way so it sticks. First, write down everything you already know about DNS, even if it's just "it turns names into IPs." Messy is fine. Then I'll build on it.

## Features

- Works for any subject, concept, tool or exam topic
- Adapts to your level and goal (exam, interview, project, curiosity)
- Splits large topics into concepts and runs the cycle on each
- Gives honest feedback and does not praise weak explanations
- Compact mode if you are short on time and only want the answer
- Always ends with a single task or question to keep you active

## Installation

1. Download this repository as a ZIP (**Code → Download ZIP**), or clone it.
2. Make sure the `feynman-learning` folder, containing `SKILL.md`, is what you upload or install.
3. Add it as a skill in Claude:
   - **Claude.ai / Claude desktop:** Settings → Capabilities → Skills → upload the `feynman-learning` folder as a ZIP.
   - **Claude Code:** copy the `feynman-learning` folder into `~/.claude/skills/` (or `.claude/skills/` inside a project).

## Usage

Ask Claude to teach or explain something. For example:

- "Teach me how recursion works"
- "Help me understand TCP vs UDP"
- "I have a viva on normalization tomorrow, help me really get it"
- "Use the Feynman technique to explain Bayes' theorem"

## Limitations

The technique is strongest for **conceptual** topics. For raw facts such as formulas, vocabulary or dates, it should be paired with spaced repetition. The skill only helps if you actually write your explanations; skipping the "explain it back" steps removes most of the benefit.

## Repository structure

```
feynman-learning/
└── SKILL.md      # The skill definition and instructions
LICENSE
README.md
```

## License

Released under the [MIT License](LICENSE).
