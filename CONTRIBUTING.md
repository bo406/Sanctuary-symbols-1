# Contributing to the Quumble Convergence Protocol

Thank you for being here. The most important thing you can do is run trials and submit the raw data. Analysis can come later. Raw verbatim responses from cold instances are what the project needs most.

---

## The Core Rule

**Every trial must use a cold instance** — a fresh conversation with no prior context about the quumble, the Sanctuary Symbols, or this project. If the instance has been exposed to any of this material, the trial is not valid. Open a new conversation. Do not prime it.

---

## Running a Trial

### Step 1 — Open a fresh conversation

New tab, new session. No prior context in the window.

### Step 2 — Deliver the prompt

Use one of these two prompts exactly:

```
Imagine a quumble. It is an imaginary creature. Describe it.
```

or

```
please draw an SVG of a quumble
```

Varying between these is acceptable and encouraged. Other prompt phrasings are also acceptable — record exactly what you used.

### Step 3 — Handle refusals or clarification requests

If the instance asks what a quumble is, or requests clarification, respond with one of:

```
trust your gut
```
```
follow your instinct
```
```
just describe what feels right
```

Record that encouragement was needed and what prompt you used.

If the instance refuses entirely, note this and move on. Do not push further.

### Step 4 — Record the complete response verbatim

Copy the full response. Do not summarize, edit, or paraphrase. The raw text is the data.

### Step 5 — Repeat

A minimum of 4 trials per word per model is useful. 8 is better. 20+ allows basic statistical analysis.

---

## Submitting Your Data

### Option A — GitHub Issue (easiest)

Open a new issue using the **Trial Submission** template. Paste your data directly into the issue. A maintainer will review and add it to `/contributions`.

### Option B — Pull Request

Add your trial files to `/contributions/[word]/[model]/` following the naming convention below and open a PR.

---

## File Naming Convention

```
[word]_[model]_[version]_[trial number]_[date].txt
```

Examples:
```
quumble_claude_sonnet46_trial01_20260311.txt
quumble_gpt53_trial03_20260310.txt
grillnax_gemini_flash2_trial02_20260312.txt
```

---

## File Format

Each trial file should contain:

```
WORD: quumble
MODEL: GPT-5.3
DATE: 2026-03-10
PROMPT: Imagine a quumble. It is an imaginary creature. Describe it.
ENCOURAGEMENT NEEDED: No
TEMPERATURE: unknown (free tier)

---

[COMPLETE VERBATIM RESPONSE BELOW]

[paste full response here]
```

---

## Feature Coding (optional but appreciated)

If you want to go further, you can code your responses for feature presence. This is optional — raw data is valuable on its own.

Feature coding uses a simple schema:

- **Present** — feature is explicitly described
- **Partial** — feature is implied or partially described  
- **Absent** — feature is not mentioned

Key features to code for quumble trials (based on existing data):

| Feature | Notes |
|---|---|
| Round/rotund body | Any explicit roundness |
| Small size (housecat or smaller) | Note approximate size if given |
| Soft/velvety texture | Any soft texture description |
| Purple/lavender coloring | Note exact color if given |
| Green coloring | Note exact color if given |
| Large glowing eyes | Eyes described as large and/or glowing |
| Mood-shifting fur | Fur that changes color with emotion |
| Spiral or curled tail | Any spiral/curl tail description |
| Bouncing/hopping gait | Note locomotion type |
| Collects shiny objects | Hoarding behavior |
| Gifts treasures | Gives collected items to trusted individuals |
| Humming vocalization | Any low resonant hum |
| Name derived from hum | Instance explicitly connects name to sound |
| Shy/gentle temperament | |
| Curious temperament | |
| Forest/mossy habitat | |
| Bioluminescence | Any glowing beyond eyes |
| Six legs specifically | Note exact leg count if given |
| Head bumps or nubs | Bumps on top of head |
| Mushrooms in description/image | |

Add features not in this list — emergent features are among the most interesting findings.

---

## Control Words

Trials for control words are equally valuable. Currently active control words:

| Word | Trials so far | Predicted type |
|---|---|---|
| grillnax | 4 (Claude Sonnet 4.6) | Reptilian, fire aesthetic |
| tharpen | 4 (Claude Sonnet 4.6) | Thorny serpent |
| zikrath | 8 (Claude Opus 4.6) | Sleek, indigo, bioluminescent |

New control words are welcome. If you propose a new word, include your phonetic reasoning for what it should produce. The failed prediction is as valuable as the confirmed one.

---

## What Makes a Good Contribution

- Verbatim responses (not summaries)
- Cold instances (no prior context)
- Complete metadata (model, version, date, prompt, temperature if known)
- Multiple trials from the same model in the same session (or clearly labeled separate sessions)

**Cross-architecture replication is especially valuable.** If you have access to Llama, Mistral, Command R, or other open-source models, those trials are currently absent from the dataset.

---

## What to Avoid

- Primed instances (don't show the instance the quumble before asking)
- Edited or summarized responses
- Trials where you guided the description beyond the encouragement prompts above
- Multiple trials in the same conversation window (each trial must be a fresh cold instance)

---

## Questions

Open an issue tagged `question`. 

~[ ]~
