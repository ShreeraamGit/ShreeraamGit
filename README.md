# Shreeraam Alagarsamy Sethuraj

**AI Product Engineer — Paris, France**

I design and ship production AI systems on the web: generative image pipelines,
LLM-powered tooling, and the infrastructure that keeps them reliable and affordable.
2+ years of freelance delivery on Upwork; currently building AI-driven commerce.

### What I build

- **Production generative-AI pipelines** — batch image generation with Gemini,
  orchestrated on Inngest workers, with cost budgets, perceptual-hash dedup,
  and face-similarity quality gates. Running in production, not a demo.
- **Self-hosted AI code review platform** — deployed and operate Kodus on an
  Oracle Cloud ARM VM: 7-container Docker stack (NestJS API, review worker,
  RabbitMQ, Postgres, MongoDB) behind Nginx/SSL, reviewing every PR via a
  GitHub App with a custom merge gate that blocks on critical/high findings.
  ~$0/month infrastructure.
- **The full stack around the AI** — Next.js 16 / React 19 apps, Supabase,
  Stripe payments, CI/CD — because a model call is 5% of shipping an AI product.

### Selected work

**[Eesha Silks](https://www.eeshasilks.com)** — production e-commerce platform with an AI product-photography pipeline
- Multi-provider image generation (Gemini + OpenAI) behind a provider factory, with structured prompt engineering (garment geometry, shot curation, framing constraints)
- Batch jobs on a dedicated Inngest worker (Render) to escape serverless time limits; admin ops console to dispatch/reap/redispatch jobs
- Cost control as a first-class feature: daily spend budgets, duplicate detection via perceptual hashing, face-similarity scoring for output QA
- Around it: hardened Stripe checkout (server-side pricing, anti-tampering), WCAG 2.1 AA compliance (234 → 0 violations), 15 CI/CD workflows

**[kodus-ai](https://github.com/ShreeraamGit/kodus-ai)** — self-hosted AI code review platform (Kodus on Oracle Cloud Free tier): RabbitMQ-queued review pipeline, per-stage audit trail, AST graph context, cost-capped LLM (deepseek via OpenCode Zen), custom CI merge gate that blocks merges on critical/high findings. Reviews every PR on a production e-commerce repo.

### Stack

**AI:** Gemini API · OpenAI API · prompt engineering · Inngest · image-similarity scoring
**Core:** TypeScript · Next.js · React · Node.js · Supabase/Postgres · Stripe
**Infra/Ops:** Docker · RabbitMQ · Oracle Cloud (ARM64) · Nginx · GitHub Actions · Vercel · Render · Playwright · Vitest

### Contact

📫 shreeraaam@outlook.com
