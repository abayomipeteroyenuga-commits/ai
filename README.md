# Ethan AI Lab v2.0 — Professional AI Experimentation PWA

Suggested domain: `ailab.ethandigitalacademy.org`

## What v2 adds
- Professional Playground with system/user prompts, variables, reusable constraints and model profiles
- Prompt library with version history, rollback/load workflow and local prompt optimization
- Side-by-side A/B prompt comparison and recorded pairwise reviews
- Dataset manager with CSV, JSON and JSONL local import
- Evaluation studio with reusable cases, batch experiments, composite local scoring and experiment history
- JSON Schema studio and candidate-output validation
- Function/tool builder with typed parameter schemas
- Agent Studio with selectable tools, autonomy levels, guardrails, readiness scoring and saved blueprints
- AI app/workflow project canvas with user problem, inputs, outputs, success metrics, risks and build blueprint
- Lab notebook for observations, hypotheses, decisions and research notes
- Secure-backend connector contract for real AI providers without exposing API keys in the browser
- Workspace export/import, dark/light theme, responsive UI, installable PWA and offline shell

## Security architecture
Do **not** put OpenAI, Gemini, Anthropic or other provider API keys inside this frontend or localStorage. Configure a server/serverless endpoint such as `/api/ai` and keep provider credentials there. Ethan AI Lab sends a structured request to that endpoint only when live mode is enabled.

## Deployment
Upload these files to the repository root and deploy as a static site on Vercel, Netlify, Cloudflare Pages or another HTTPS host. HTTPS is required for normal PWA installation/service-worker behavior.

## Standalone behavior
Without a backend the app remains fully useful for prompt design, versioning, datasets, local evaluation exercises, schema/tool design, agent planning, project work, notes and portfolio evidence. Live AI text generation is intentionally not faked.
