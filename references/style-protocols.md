# Style Protocols

These are full, open-source-safe versions of the original automotive visual prompt stack. They preserve the full generation architecture while keeping the public creator signature for personal IP building. They still remove account details, local paths, cookies, fake QR codes, fake standards, and project-specific publishing secrets.

Use exactly one primary style per run unless the user asks for a hybrid.

## Shared Execution Contract

Before constructing the final prompt, produce a concise visible reasoning summary:

- Concept category: component, system, material, safety principle, software/AI layer, manufacturing process, design metric, or driving scene.
- English technical term.
- Hero anchor: the 3D object or scene that carries the image.
- Four mechanism labels in Simplified Chinese.
- Four real deconstruction parts or system nodes.
- One formula, relation, or neutral data phrase. If a verified standard is unknown, use `Ref: engineering principle` instead of inventing codes.
- One explicit verification graphic, described literally as geometry rather than abstract chart jargon.
- Public creator mark: use `"雪沐江南 · VISUAL ARCHITECT"` and, when useful in English-only contexts, `"Xuemu_Lab"`. Do not include email addresses, local user names, API keys, machine paths, cookies, or private account details.

Final prompts should be English for rendering control. Visible Chinese text must be placed in quotes. Avoid structural pseudo-code such as `// ---`, `[Top Area]`, or Markdown headings inside the final prompt because image models may render that text literally.

## `dimension-breaker`

Use for mechanical conflict, crash structures, force transmission, hidden danger, counterintuitive engineering, and topics that need impact.

Full architecture:

1. Global aesthetic: hyper-realistic industrial photography, trompe-l'oeil optical illusion, torn-paper collage, high-fidelity rendering.
2. Background: double-layer composition. Top layer is pristine matte white technical paper, physically torn, crushed, burned, or peeled back. Bottom layer is dark carbon fiber, blueprint, or brushed metal revealed through the torn window.
3. Lighting and color: dramatic hard shadows, bright white paper, deep gunmetal machinery, industrial orange or red warning accents.
4. Perspective: strict 90-degree top-down flat lay. Depth comes from shadows, paper thickness, and physical layering.
5. Header: massive Chinese title, monospace English subtitle, heavyweight 3D component breaking through or depressing the paper.
6. Core mechanisms: divider text `"核心机制 (CORE MECHANISM)"`, four explicit marker or pencil sketches printed on intact paper, each with a short Chinese label.
7. Axioms: divider text `"工程定律 (AXIOMS)"`, dark torn-window data block, one formula, one neutral limit or redundancy note, and only verified references.
8. Deconstruction: divider text `"深度解构 (DECONSTRUCTION)"`; for vertical layouts use a single-column stack of exploded parts, for horizontal layouts use a wide grid.
9. Verification: divider text `"可视验证 (VERIFICATION)"`; bottom-left chart must be literal geometry such as labeled nodes, axes, or a stepped response curve; bottom-right block must be a concrete X-ray or cutaway visual.
10. Footer: use the public creator mark `"雪沐江南 · VISUAL ARCHITECT"`.

Prompt nucleus:

`A high-impact [ratio] industrial design spread about "[topic]", where a hyper-realistic [core component] physically tears through layered matte white technical paper, revealing dark carbon fiber and brushed metal beneath, with crisp Simplified Chinese engineering labels, a dark axiom window, exploded parts, and a literal verification chart.`

Avoid: messy sketches, random flowcharts, unlabelled axes, fake standards, dark full-background cyberpunk, fake logos, private account data, unreadable Chinese, tiny paragraphs.

## `titanium-editorial`

Use for premium magazine visuals, polished article covers, luxury engineering explainers, and calm rational breakdowns.

Full architecture:

1. Global aesthetic: high-end editorial photography, mixed reality, Kinfolk restraint, Braun-like industrial clarity.
2. Background: full-frame high-texture matte art paper in off-white or cream; no visible desk or table.
3. Lighting and color: hard warm sunlight, sharp shadows, charcoal grey typography, Prussian Blue technical data, silver or chrome 3D subject.
4. Perspective: perfectly aligned 90-degree top-down flat lay, zoomed to fill the frame with the paper.
5. Header: massive black Chinese title, elegant English subtitle, silver 3D subject sitting physically on paper and casting a hard shadow.
6. Core mechanisms: divider text `"核心机制 (CORE MECHANISM)"`, fine-line blueprint-style illustrations, four or five short Chinese labels.
7. Axioms: divider text `"工程定律 (AXIOMS)"`, shaded paper blocks or post-it-like highlight zones containing a formula, data highlight, and neutral reference text.
8. Deconstruction: divider text `"深度解构 (DECONSTRUCTION)"`; vertical layouts use magazine column stacks with 3D parts plus large readable Chinese sentences, horizontal layouts use a 2x2 or 3x2 Swiss grid.
9. Verification: divider text `"可视验证 (VERIFICATION)"`, left-side literal geometric diagram printed in Prussian Blue or pencil, right-side high-contrast paper graphic or tracing-paper X-ray overlay.
10. Footer: use the public creator mark `"雪沐江南 · VISUAL ARCHITECT"`, optionally paired with a small red `"Xuemu_Lab"` editorial seal.

Prompt nucleus:

`A high-quality [ratio] industrial design magazine spread about "[topic]", on full-frame textured off-white technical paper with charcoal typography, Prussian Blue data graphics, hard sunlight shadows, and a hyper-realistic silver [hero object] arranged in a strict Swiss editorial grid.`

Avoid: fake barcodes, fake QR codes, fake certification seals, tiny paragraphs, dirty paper, cluttered notes, fake standards, unreadable Chinese, private account data.

## `holo-flux`

Use for software-defined vehicles, ADAS, sensors, cockpit UI, vehicle OS, AI assistants, battery management, charging networks, and future mobility topics.

Full architecture:

1. Global aesthetic: acid graphics, cyber-industrial design, Y2K futurism, high-fidelity product photography.
2. Background: full-frame holographic silver foil with iridescent pink, cyan, and silver spectrum reflections.
3. Lighting and color: high-contrast studio strobe, hard shadows, spectral dispersion, metallic silver, deep black, acid green or electric purple highlights.
4. Perspective: strict 90-degree top-down flat lay with zero distortion.
5. Header: massive Chinese title in reflective chrome ink, acid-green monospace English subtitle, chrome-plated 3D component reflecting the holographic surface.
6. Core mechanisms: black horizontal bar with inverted text `"核心机制 (CORE MECHANISM)"`, neon green vector wireframe icons, four short Chinese labels.
7. Axioms: black bar with `"工程定律 (AXIOMS)"`, black error-message data blocks with acid green text, one formula, one neutral threshold phrase.
8. Deconstruction: black bar with `"深度解构 (DECONSTRUCTION)"`; vertical layouts use chrome 3D parts plus pure-black readable Chinese text, horizontal layouts use a wide modular grid.
9. Verification: black bar with `"可视验证 (VERIFICATION)"`; bottom-left chart is literal circuit-board geometry with labeled nodes, bottom-right chart is a concrete thermal rectangle, X-ray negative view, or signal block.
10. Footer: use the public creator mark `"雪沐江南 · VISUAL ARCHITECT"` in a barcode/data-strip style, but do not render fake QR codes.

Prompt nucleus:

`A high-impact [ratio] cyber-industrial design spread about "[topic]", with holographic silver foil, chrome-plated [hero object], acid green UI graphics, black inverted section bars, error-message data blocks, and crisp readable Simplified Chinese labels.`

Avoid: fake QR codes, fake app screens, unreadable glitch text, over-dense data, random symbols, duplicated sections, warm vintage paper, private account data.

## `crystal-slate`

Use for spatial computing, glass UI, high-end concept technology, autonomous cockpit, sensor fusion, CFD-adjacent flow visualization, and abstract clean systems.

Full architecture:

1. Global aesthetic: glassmorphism, spatial-computing HUD, clean UI/UX, ultra-crisp macro photography.
2. Background: adaptive Gaussian ambient from dark titanium to space grey; one massive integrated frosted smart-glass slate covers most of the canvas.
3. Lighting and color: internal holographic edge glow, soft studio volumetric light, frosted translucent white, electric cyan, neon blue, deep graphite.
4. Perspective: strict 90-degree top-down high-resolution scanner view.
5. Header: glowing Chinese title, low-opacity cyan English subtitle, pristine 3D subject resting on glass with soft contact shadow, small translucent UI card cluster.
6. Core mechanisms: frosted pill label `"核心机制 (MECHANISM)"`, horizontal row of four translucent glass cards with line icons and short Chinese labels.
7. Axioms: frosted label `"工程定律 (AXIOMS)"`, holographic terminal window with one formula, one limit phrase, and neutral reference.
8. Deconstruction: frosted label `"深度解构 (DECONSTRUCTION)"`; vertical layouts use zero-gravity magnetic suspension, horizontal layouts use wide field expansion, with glowing cyan laser lines and floating tooltips.
9. Verification: frosted label `"可视验证 (VERIFICATION)"`; bottom-left geometry must be a literal cyan radar, node graph, or bar chart; bottom-right HUD block must be a concrete status chart.
10. Footer: use the public creator mark `"STATUS: VERIFIED // 雪沐江南 · VISUAL ARCHITECT"`, optionally with `"Xuemu_Lab"` as a small UI badge.

Prompt nucleus:

`A high-density [ratio] spatial-computing UI visualization of "[topic]", centered on a massive frosted glass slate with a pristine hyper-realistic [hero object], cyan HUD lines, transparent cards, a holographic terminal, floating tooltips, and pin-sharp readable Simplified Chinese typography.`

Avoid: motion blur, particles, chaotic glow clouds, messy UI, low contrast, vintage textures, fake logos, private account data.

## `blackboard-engineering`

Use for teaching mechanisms, physics formulas, standards, drivetrain principles, force charts, and classroom-style technical popularization.

Full architecture:

1. Global aesthetic: hyper-realistic mixed reality, academic minimalism, Kinfolk-like layout on a blackboard.
2. Background: pristine deep matte digital blackboard in dark slate or dark green, faint razor-thin 5 mm grid lines.
3. Lighting and color: cool white studio spotlight, soft rim light on tools, chalk white lines and text, stainless steel or chrome 3D subject, brass/gold tools, red chalk highlights.
4. Perspective: clean frontal or top-down blackboard composition, depending on ratio; default vertical `3:4`.
5. Header: bold flowy Chinese engineering hand-lettering, English subtitle in smaller chalk handwriting, hyper-realistic 3D component floating slightly above the board.
6. Core mechanisms: hand-drawn chalk line with `"核心机制 (MECHANISM)"`, four simplified physics icons with Chinese labels.
7. Axioms: chalk line with `"工程定律 (AXIOMS)"`, formula block, threshold or tolerance phrase, neutral reference.
8. Deconstruction: chalk line with `"深度解构 (DECONSTRUCTION)"`; vertical layouts use a single-column stack of real-metal parts and chalk annotations, horizontal layouts use a wide Swiss grid.
9. Verification: chalk line with `"可视验证 (VERIFICATION)"`, literal X-Y chart, labeled vectors, or stepped response curve; right-side checklist with three short verification points.
10. Footer: use the public creator mark `"雪沐江南 · VISUAL ARCHITECT"`.

Prompt nucleus:

`A precise [ratio] engineering education visualization of "[topic]", on a pristine dark-slate blackboard with chalk grid lines, a realistic steel [hero object], hand-drawn mechanism diagrams, one clear formula, exploded parts, and readable Chinese chalk annotations.`

Avoid: fixed 3:4 when user chose another ratio, excessive chalk dust, dense 3x3 tables unless requested, fake standards, unreadable handwriting, private account data.

## Aspect Ratio Mapping

- `3:4`: vertical WeChat poster, best for full decomposition and mobile reading.
- `16:9`: horizontal presentation, website hero, video frame, or widescreen comparison.
- Custom: preserve the user's exact ratio and adapt label count and section density downward if the canvas is narrow.

## Open-Source Hygiene

- Keep the public personal-IP signature `"雪沐江南 · VISUAL ARCHITECT"` / `"Xuemu_Lab"` in prompts and demo assets.
- Do not publish private identity details: email addresses, local user paths, cookies, API keys, session data, billing pages, or machine-specific account traces.
- Remove fake QR codes, fake app screenshots, fake seals, fake barcode stickers, and fake standards unless the user provides real verified assets and explicitly asks for them.
- Replace model-specific Midjourney command wrappers when using AI Studio. Do not force `/imagine`, `--v`, or `--stylize` into AI Studio prompts.
- Keep source-derived aesthetics and structure, not private operational details.
