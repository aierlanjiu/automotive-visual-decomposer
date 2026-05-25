---
name: automotive-visual-decomposer
description: "Turn a user-provided automotive term, component, technology, design concept, product idea, or engineering principle into an interactive visual decomposition workflow: choose style, choose aspect ratio, reason through the visual structure, then output a production-ready image prompt. Use for 汽车视觉可视化, 视觉拆解, engineering poster prompts, infographic prompts, AI Studio image prompts, Codex image generation, Antigravity image generation, and open-source automotive visual style workflows."
---

# Automotive Visual Decomposer

## Overview

Use this skill to turn a single automotive concept into a high-end visual prompt with a clear style path, aspect ratio, visual anchor, decomposition logic, and image-generation target.

Default to prompt output. Generate an image only when the user asks for direct rendering or the current environment clearly has a usable internal image engine.

## Workflow

### 1. Intake

Ask for any missing required choice in one compact interaction:

- Concept: the automotive term or noun to visualize.
- Style: `dimension-breaker`, `titanium-editorial`, `holo-flux`, `crystal-slate`, or `blackboard-engineering`.
- Aspect ratio: `3:4`, `16:9`, or a user-provided custom ratio.
- Output mode: `prompt-only`, `prompt+image`, or `image-only`.

If the user only provides the concept, present the style and aspect choices before producing the final prompt.

### 2. Reasoning Pass

Produce a concise reasoning summary, not hidden chain-of-thought:

- Define the concept category: component, system, design metric, driving scene, manufacturing process, safety principle, software/AI, or brand/product narrative.
- Pick the visual anchor: vehicle, module, component, exploded assembly, force/vector field, UI layer, scene, or material detail.
- Extract 3-5 readable labels. Keep labels short; do not overload the image with paragraphs.
- Use verified facts only. If the concept depends on current vehicle specs, pricing, regulations, or new launches, verify first. If facts are not available, use neutral labels.

### 3. Style Selection

Read `references/style-protocols.md` and apply only the selected style. Do not mix multiple primary styles unless the user explicitly asks.

Use style names exactly:

- `dimension-breaker`: strongest for mechanical conflict, controversy, and destructive metaphors.
- `titanium-editorial`: premium magazine look for calm, expensive-looking explainers.
- `holo-flux`: cyber-industrial look for software-defined vehicles, AI, cockpit UI, sensors, and electrification.
- `crystal-slate`: glassmorphism / spatial UI look for abstract, high-end technology concepts.
- `blackboard-engineering`: chalkboard education look for formulas, mechanisms, and classroom-style breakdowns.

### 4. Prompt Construction

Return the final answer in this structure:

```markdown
## Selection Path
- Concept:
- Style:
- Aspect ratio:
- Output mode:
- Recommended engine:

## Visual Reasoning Summary
- Category:
- Hero anchor:
- Decomposition labels:
- Data/fact policy:

## Final Prompt
[one complete image prompt]
```

The final prompt should be English for rendering control, while exact visible Chinese text should stay in Chinese inside quotes. Keep visible text explicit and short.

### 5. Image Engine Policy

Prefer this order:

1. Recommend AI Studio / Nano Banana Pro 4K as the primary production route when the user is choosing where to render.
2. In Codex, if native image generation is available and the user asks for direct drawing, call the internal image engine with the final prompt.
3. In Antigravity, if its image engine is available and configured, use it with the same final prompt.
4. If no rendering engine is available, stop at the final prompt and clearly say prompt-only was delivered.

Do not hardcode API keys, proxy addresses, cookies, or local account details. Respect the current environment.

## Rules

- Default language for conversation and reasoning summary is Simplified Chinese.
- Do not write article copy, titles, publishing steps, or social media captions unless the user asks.
- Do not invent vehicle specs, standards, dates, prices, certifications, logos, QR codes, or regulatory numbers.
- Strip internal watermarks, internal brand stamps, and private project signatures from open-source prompts unless the user explicitly requests branding.
- Keep final image prompts clean. Do not put Markdown section markers, pseudo-layout code, or comments into the prompt body.
- Prefer fewer larger labels over many tiny annotations.
- Include negative constraints for text quality, fake marks, clutter, broken geometry, and unreadable Chinese.
