# Style Protocols

Use exactly one primary style per run unless the user asks for a hybrid. These protocols are open-source-safe distillations of the original automotive visual prompt stack.

## `dimension-breaker`

Use for mechanical conflict, crash structures, force transmission, controversy, hidden danger, counterintuitive engineering, and topics that need impact.

- Look: matte technical paper physically torn by heavy machinery, dark carbon fiber or brushed metal revealed underneath, hard shadows, warning accents.
- Composition: strict top-down flat lay. The 3D component breaks through, crushes, tears, burns, or depresses the paper.
- Text policy: big Chinese title, 3-4 mechanism sketches, one formula/data block, 3-4 exploded parts, one verification chart.
- Prompt nucleus: "A high-impact [ratio] industrial design spread about \"[topic]\", where a hyper-realistic [core component] violently interacts with layered white technical paper, revealing dark carbon fiber and mechanical voids beneath, with crisp Chinese engineering labels and a structured verification panel."
- Avoid: messy sketches, random flowcharts, unlabelled axes, fake standards, dark full-background cyberpunk.

## `titanium-editorial`

Use for premium magazine visuals, polished article covers, luxury engineering explainers, and calm rational breakdowns.

- Look: off-white premium paper, Prussian Blue technical ink, charcoal typography, silver or chrome 3D subject, hard sunlight shadows.
- Composition: full-frame paper background, no visible desktop. Top-down editorial flat lay with a clean Swiss grid.
- Text policy: title, English subtitle, core mechanism sketches, axioms block, 3-4 deconstruction labels, visual verification panel.
- Prompt nucleus: "A high-end [ratio] industrial design magazine spread about \"[topic]\", on full-frame textured off-white technical paper with Prussian Blue data graphics, charcoal typography, and a hyper-realistic silver [hero object] casting crisp hard shadows."
- Avoid: fake barcodes, fake seals, tiny paragraphs, dirty paper, cluttered notes, illegible Chinese.

## `holo-flux`

Use for software-defined vehicles, ADAS, sensors, cockpit UI, vehicle OS, AI assistants, battery management, charging networks, and future mobility topics.

- Look: holographic silver foil, acid green and electric purple highlights, chrome 3D parts, cyber-industrial UI, high-contrast typography.
- Composition: strict top-down flat lay. Use black bars, neon vector wireframes, error-message data blocks, and chrome exploded parts.
- Text policy: one massive Chinese title, one English technical subtitle, 4 mechanism icons, formula/data block, 3-4 labels.
- Prompt nucleus: "A high-impact [ratio] cyber-industrial design spread about \"[topic]\", with holographic silver foil, chrome-plated [hero object], acid green UI graphics, black inverted section bars, and crisp readable Chinese labels."
- Avoid: fake QR codes, unreadable glitch text, over-dense data, random symbols, duplicated sections, warm vintage paper.

## `crystal-slate`

Use for spatial computing, glass UI, high-end concept technology, autonomous cockpit, sensor fusion, CFD-adjacent flow visualization, and abstract clean systems.

- Look: large frosted glass slate, deep titanium-to-space-grey ambient background, cyan edge glow, transparent UI cards, pristine 3D object.
- Composition: the glass slate covers most of the canvas. Use zero-gravity exploded parts or horizontal field expansion depending on ratio.
- Text policy: ultra-clean title, small English subtitle, 4 glass cards, one holographic terminal formula, 3-4 floating tooltips.
- Prompt nucleus: "A high-density [ratio] spatial-computing UI visualization of \"[topic]\", centered on a massive frosted glass slate with a pristine hyper-realistic [hero object], cyan HUD lines, transparent cards, and pin-sharp readable Chinese typography."
- Avoid: motion blur, particles, chaotic glow clouds, messy UI, low contrast, vintage textures.

## `blackboard-engineering`

Use for teaching mechanisms, physics formulas, standards, drivetrain principles, force charts, and classroom-style technical popularization.

- Look: deep matte dark-slate blackboard, white chalk schematics, chrome or steel 3D component, red chalk highlights, precise grid.
- Composition: title and hero object on top, mechanism icons and equation block in the middle, exploded parts and verification chart below.
- Text policy: chalk-style Chinese must stay readable. Use 3-4 labels and one formula. Do not force dense 3x3 tables unless the user asks.
- Prompt nucleus: "A precise [ratio] engineering education visualization of \"[topic]\", on a clean dark-slate blackboard with chalk grid lines, a realistic steel [hero object], hand-drawn mechanism diagrams, one clear formula, and readable Chinese chalk annotations."
- Avoid: fixed 3:4 if user chose another ratio, proprietary stamps, excessive chalk dust, tiny tables, fake standards.

## Aspect Ratio Mapping

- `3:4`: vertical WeChat poster, best for full decomposition and mobile reading.
- `16:9`: horizontal presentation, website hero, video frame, or widescreen comparison.
- Custom: preserve the user's exact ratio and adapt layout density downward if the canvas is narrow.

## Open-Source Hygiene

- Replace internal footers, brand stamps, private signatures, and project names with neutral wording such as "VISUAL ARCHITECT", unless the user requests branding.
- Replace model-specific command syntax only when the target renderer needs it. Do not force Midjourney suffixes into AI Studio prompts.
- Keep source-derived aesthetics, not private operational details.
