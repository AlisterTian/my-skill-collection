<!-- Modified for My Skill Collection on 2026-09-12: local skill refinements and/or portable example paths; original attribution and terms retained. -->

# Default operating stance

The older Python/matplotlib rules in this skill remain valid. The skill also supports R, especially `ggplot2 + patchwork + ComplexHeatmap + ggrepel + svglite/cairo_pdf + ragg`.

## Color policy

Prefer **unified method families across all panels** over maximal hue separation. For dense Nature Machine Intelligence-style figure pages, use the low-saturation `NMI pastel` family described in `references/api.md` and reserve green/red mainly for gains, drops, and other directional cues.

## Stance

- Start by classifying the requested figure into one of four archetypes: `quantitative grid`, `schematic-led composite`, `image plate + quant`, or `asymmetric mixed-modality figure`.
- Prefer one **hero panel** plus subordinate evidence panels over filling the canvas with equal-sized subplots.
- If the user asks for a single chart, still identify its role in the manuscript claim: discovery, mechanism, validation, comparison, robustness, or clinical/biological relevance.
- Keep the background white for plots and diagrams; switch to black only for microscopy / volume-rendering image plates.
- Prefer direct labels over legends when categories are spatially fixed or the legend would force unnecessary eye travel.
- Keep one restrained palette per figure: usually one neutral family, one signal family, and one accent family.
- Treat perceptual separation as necessary but not sufficient: verify that the intended hero series is more salient than baselines after rendering, and do not reuse a sequential light-to-dark scale as unrelated categorical colors.
- Treat statistics, `n`, error-bar definitions, source-data traceability, and image-integrity notes as part of the figure, not as optional caption cleanup.
- When panels show comparable seed/fold/split aggregates, use the same uncertainty definition in every comparable panel or state why a panel is exempt.
- Preserve canonical model capitalization in display labels. Legend entries use display-style initial capitalization; prose follows normal sentence grammar. Never apply blind `.title()` transformations to names such as `XGBoost`, `DeepSeek`, `GPT-5.2`, or `RF`.
- Require a final-size, panel-by-panel visual inspection after automated checks. Source validation cannot prove color hierarchy, label clearance, legend spacing, or complete uncertainty coverage.
- When the user asks for broad `Nature` style rather than ML/NMI-specific style, read `references/nature-2026-observations.md` before choosing layout.
- When the user references `figures4papers` or the older `scientific-figure-making` skill, treat this skill as the successor and open `references/demos.md` for the third-party demo map, copyright boundary, and original reimplementation guidance.

## Private sources and delivery transparency

Keep private source paths, template identifiers, and unpublished provenance out of manuscript text, figure legends, and public artifacts. Use neutral source descriptions there. In the private conversation with the user, provide usable links to requested deliverables. If a skill instruction causes a pause or deviation, link the exact SKILL.md and relevant reference, quote the instruction, and explain its application without exposing unrelated private material.

## When to load this skill

- Python or R figures for **papers, slides, or reports** targeting Nature, Science, Cell, NeurIPS, ICLR, or similar venues.
- Requests involving **grouped bars, trend lines, heatmaps, radar plots, multi-panel grids**, or **PDF/SVG/high-DPI** output.
- Any mention of "Nature style", "publication figure", "paper figure", "SCI figure", "figures4papers", "scientific-figure-making", "R plotting template", or "high-quality scientific plot".
- Requests to improve a figure's logic, aesthetics, panel layout, figure legend, export quality, or journal-readiness.

## When NOT to load

- Plotly, Altair, Bokeh, or other interactive/web-first plotting.
- EDA-only plots without a publication target.
- Primary workflow is 3D, GIS, or non-scientific illustration tooling.
- Illustrator / Figma–first layout.
