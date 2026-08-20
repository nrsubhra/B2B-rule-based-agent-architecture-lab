# B2B Agent Architecture Lab

Standalone static web platform for a controlled B2B multi-agent procurement experiment.

## What users can do

- Edit or add synthetic vendors.
- Set six vendor dimensions: Technical/IT, Finance/Economic Value, Risk/Security, Legal/Compliance, Operations/Implementation, Relationship/Service.
- Add a critical diagnostic fact and penalty to any vendor.
- Edit the firm's organizational objective weights.
- Compare Single AI, Pipeline, Parallel, Shared Memory, and Supervisor architectures.
- Manipulate centralized vs fragmented information.
- Optionally explore goal conflict and specialization as secondary-study factors.
- Run repeated rule-based apparatus-validation simulations.
- Inspect architecture diagrams and information-flow traces.
- Export trial-level CSV.
- Export/import the entire scenario as JSON.

## Methodological terminology

The app uses **design-implied benchmark**, not "normative optimum." The benchmark is the vendor that maximizes the organizational utility function explicitly specified by the experimenter, using the complete vendor record. It is an internal-validity benchmark, not a universal claim about real-world procurement.

## Recommended dissertation sequence

1. Apparatus validation using the current rule-based layer.
2. Main Study 1: Architecture × Information Distribution.
3. Treat vendor scenario as a replicated/block/random factor.
4. Study 2: add goal conflict.
5. Study 3: specialist vs redundant-generalist agents.
6. Study 4: human oversight / human-seeded systems.

## Future LLM version

Use LangGraph for orchestration and LangSmith for observability, while storing research data independently. Preserve fact IDs and require structured outputs. Human-code a sample of traces for reliability. Include fact-removal counterfactuals.

## Run locally

Double-click `index.html`.

## Host publicly

### GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html`.
3. Go to Settings → Pages.
4. Choose "Deploy from a branch" and select `main` / root.

### Netlify
Drag this folder into Netlify's static-site deployment interface.

### Important
The public static version intentionally does not embed an Anthropic/OpenAI API key. A live LLM version should call a server-side API endpoint so credentials remain private and model/version metadata can be logged.
