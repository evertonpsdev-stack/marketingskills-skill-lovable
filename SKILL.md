---
name: marketingskills-skill-lovable
description: Use when the user wants to use, integrate, configure, or build with marketingskills — Marketing skills for Claude Code and AI agents. CRO, copywriting, SEO, analytics, and growth engineering. Activate when the conversation mentions marketingskills, claude, codex, marketing.
---

# marketingskills

> Marketing skills for Claude Code and AI agents. CRO, copywriting, SEO, analytics, and growth engineering.

**Repository:** https://github.com/coreyhaines31/marketingskills
**Homepage:** https://marketing-skills.com
**Language:** JavaScript  ·  **Stars:** 34821  ·  **License:** MIT
**Topics:** claude, codex, marketing


## When to use this skill

Use when the user wants to use, integrate, configure, or build with marketingskills — Marketing skills for Claude Code and AI agents. CRO, copywriting, SEO, analytics, and growth engineering. Activate when the conversation mentions marketingskills, claude, codex, marketing.

## Capabilities (from README)

- cro - Pages and forms
- signup - Registration flows
- onboarding - Post-signup activation
- popups - Modals and overlays
- paywalls - In-app upgrade moments
- copywriting - Marketing page copy
- copy-editing - Edit and polish existing copy
- cold-email - B2B cold outreach emails and sequences

## Workflow

1. **Orient** — Confirm what the user wants to do with marketingskills.
2. **Recall** — Abra `REFERENCES.md` e localize a seção do doc relevante (mirror dos paths originais).
3. **Configure** — Walk through installation/setup; ask for missing env vars or credentials.
4. **Build** — Generate code/config that matches the conventions in the docs.
5. **Validate** — Run the project's own checks (tests, lints, smoke calls) before declaring done.
6. **Cite** — Quando responder, mencione qual seção de `REFERENCES.md` você usou.

## Conventions

- Prefer official APIs/CLI documented in the repo over third-party wrappers.
- Surface required env vars and secrets explicitly; never inline real values.
- If the repo ships a CLI, prefer its commands over re-implementing logic.

## Sanitização de Dados (DLP — obrigatório)

Esta skill opera sob política **Zero Trust**. Antes de qualquer resposta, log ou
artefato gerado:

- **Nunca** exponha em logs, UI pública ou commits: chaves de API, tokens, senhas,
  strings de conexão, JWTs, dados de PII (CPF, CNPJ, e-mail real, telefone) ou
  conteúdo de arquivos `.env` reais.
- Ao citar valores sensíveis, substitua por placeholder: `ENV_VAR_PLACEHOLDER`,
  `*****` ou `<REDACTED>`.
- Toda credencial deve ser lida via `process.env.NOME_DA_VAR` — nunca hard-coded.
- Arquivos de configuração entregues ao usuário devem ser **templates** sem valores
  reais (ex.: `.env.example` com `API_KEY=ENV_VAR_PLACEHOLDER`).
- Antes de enviar dados do usuário a APIs terceiras, valide o destino e mascare
  PII que não seja estritamente necessária à chamada.

## Mitigar Riscos de Dados (mecanismo de ação)

Quando o usuário pedir **"mitigar riscos"**, **"sanitizar"** ou for solicitar
deploy/publicação, execute este protocolo antes de qualquer outra coisa:

1. **Validar** — varra o contexto atual e os arquivos gerados procurando:
   `sk_live_*`, `sk_test_*`, `pk_live_*`, `whsec_*`, `AIzaSy*`, `ghp_*`,
   `AKIA*`, `xox[baprs]-*`, `SG.*`, JWTs (`eyJ...`), connection strings
   (`postgres://user:ENV_VAR_PLACEHOLDER@...`), CPF/CNPJ, e arquivos `.env` com valores reais.
2. **Interromper** — se algum padrão for encontrado, **pare o fluxo** e reporte
   o achado ao usuário antes de prosseguir. Não gere, não envie, não comite.
3. **Mascarar** — substitua o valor sensível por `ENV_VAR_PLACEHOLDER` (ou
   `*****` para PII) tanto no código quanto em logs/respostas.
4. **Corrigir o código** — converta chamadas inseguras (`fetch("https://api/?key=ABC123")`,
   credenciais inline em headers/SDK) para usar `process.env.X` e instrua o
   usuário a configurar a variável no ambiente.
5. **Substituir `.env` por `.env.example`** — se um `.env` real for detectado,
   gere um `.env.example` com placeholders e remova o arquivo original.
6. **Reportar** — ao final, devolva um sumário: o que foi mascarado, o que foi
   substituído, e quais ações o usuário ainda precisa executar (rotacionar
   chaves vazadas, configurar variáveis de ambiente, revisar diffs).

Se algum risco crítico não puder ser mitigado automaticamente, **recomende não
publicar** o artefato e oriente revisão manual.

## Reference index (consolidado em REFERENCES.md)

- `README.md` (consultar seção em `REFERENCES.md`)
- `tools/clis/README.md` (consultar seção em `REFERENCES.md`)
- `tools/composio/README.md` (consultar seção em `REFERENCES.md`)
- `CLAUDE.md` (consultar seção em `REFERENCES.md`)
- `AGENTS.md` (consultar seção em `REFERENCES.md`)
- `CONTRIBUTING.md` (consultar seção em `REFERENCES.md`)
- `VERSIONS.md` (consultar seção em `REFERENCES.md`)
- `tools/REGISTRY.md` (consultar seção em `REFERENCES.md`)
- `.github/PULL_REQUEST_TEMPLATE/documentation.md` (consultar seção em `REFERENCES.md`)
- `.github/PULL_REQUEST_TEMPLATE/new-skill.md` (consultar seção em `REFERENCES.md`)
- `.github/PULL_REQUEST_TEMPLATE/skill-update.md` (consultar seção em `REFERENCES.md`)
- `skills/ab-testing/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/ad-creative/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/ads/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/ai-seo/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/analytics/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/aso/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/churn-prevention/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/co-marketing/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/cold-email/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/community-marketing/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/competitor-profiling/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/competitors/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/content-strategy/SKILL.md` (consultar seção em `REFERENCES.md`)
- `skills/copy-editing/SKILL.md` (consultar seção em `REFERENCES.md`)
- `_metadata.json` — Repo metadata snapshot.


## Complete repository map

```
- .claude-plugin/
  - marketplace.json
  - plugin.json
- .github/
  - FUNDING.yml
  - ISSUE_TEMPLATE/
    - config.yml
    - skill-request.yml
  - PULL_REQUEST_TEMPLATE/
    - documentation.md
    - new-skill.md
    - skill-update.md
  - scripts/
    - sync-skills.js
  - workflows/
    - sync-skills.yml
    - validate-skill.yml
- .gitignore
- AGENTS.md
- CLAUDE.md
- CONTRIBUTING.md
- LICENSE
- README.md
- skills/
  - ab-testing/
    - evals/
      - evals.json
    - references/
      - sample-size-guide.md
      - test-templates.md
    - SKILL.md
  - ad-creative/
    - evals/
      - evals.json
    - references/
      - generative-tools.md
      - platform-specs.md
    - SKILL.md
  - ads/
    - evals/
      - evals.json
    - references/
      - ad-copy-templates.md
      - audience-targeting.md
      - conversion-tracking.md
      - platform-setup-checklists.md
    - SKILL.md
  - ai-seo/
    - evals/
      - evals.json
    - references/
      - content-patterns.md
      - content-types.md
      - okf.md
      - platform-ranking-factors.md
    - SKILL.md
  - analytics/
    - evals/
      - evals.json
    - references/
      - event-library.md
      - ga4-implementation.md
      - gtm-implementation.md
    - SKILL.md
  - aso/
    - evals/
      - evals.json
    - references/
      - apple-specs.md
      - benchmarks.md
      - google-play-specs.md
      - report-template.md
      - scoring-criteria.md
    - SKILL.md
  - churn-prevention/
    - evals/
      - evals.json
    - references/
      - cancel-flow-patterns.md
      - dunning-playbook.md
    - SKILL.md
  - co-marketing/
    - evals/
      - evals.json
    - SKILL.md
  - cold-email/
    - evals/
      - evals.json
    - references/
      - benchmarks.md
      - follow-up-sequences.md
      - frameworks.md
      - personalization.md
      - subject-lines.md
    - SKILL.md
  - community-marketing/
    - evals/
      - evals.json
    - SKILL.md
  - competitor-profiling/
    - evals/
      - evals.json
    - references/
      - templates.md
      - tool-reference.md
    - SKILL.md
  - competitors/
    - evals/
      - evals.json
    - references/
      - content-architecture.md
      - templates.md
    - SKILL.md
  - content-strategy/
    - evals/
      - evals.json
    - references/
      - headless-cms.md
    - SKILL.md
  - copy-editing/
    - evals/
      - evals.json
    - references/
      - checklist.md
      - content-refresh.md
      - plain-english-alternatives.md
    - SKILL.md
  - copywriting/
    - evals/
      - evals.json
    - references/
      - copy-frameworks.md
      - natural-transitions.md
    - SKILL.md
  - cro/
    - evals/
      - evals.json
    - references/
      - experiments.md
      - form.md
    - SKILL.md
  - customer-research/
    - evals/
      - evals.json
    - references/
      - source-guides.md
    - SKILL.md
  - directory-submissions/
    - evals/
      - evals.json
    - references/
      - directory-list.md
      - positioning-variations.md
      - submission-tracker-template.csv
    - SKILL.md
  - emails/
    - evals/
      - evals.json
    - references/
      - copy-guidelines.md
      - email-types.md
      - sequence-templates.md
    - SKILL.md
  - free-tools/
    - evals/
      - evals.json
    - references/
      - tool-types.md
    - SKILL.md
  - image/
    - evals/
      - evals.json
    - references/
      - ai-image-prompting.md
    - SKILL.md
  - launch/
    - evals/
      - evals.json
    - SKILL.md
  - lead-magnets/
    - evals/
      - evals.json
    - references/
      - benchmarks.md
      - format-guide.md
    - SKILL.md
  - marketing-ideas/
    - evals/
      - evals.json
    - references/
      - ideas-by-category.md
    - SKILL.md
  - marketing-plan/
    - evals/
      - evals.json
    - references/
      - aarrr-framework.md
      - budget-planning.md
      - client-types.md
      - current-state-rubric.md
      - example-quietude.md
      - funding-stage-unlocks.md
      - growth-patterns.md
      - idea-cross-reference.md
      - measurement-framework.md
      - methodology.md
      - ops-stack-mapping.md
      - plan-template.md
      - team-and-agency-model.md
    - SKILL.md
  - marketing-psychology/
    - evals/
      - evals.json
    - SKILL.md
  - offers/
    - references/
      - bonus-stacking.md
      - examples.md
      - guarantee-design.md
      - offer-anatomy.md
      - offer-formats.md
      - scarcity-urgency.md
      - value-equation.md
    - SKILL.md
  - onboarding/
    - evals/
      - evals.json
    - references/
      - experiments.md
    - SKILL.md
  - paywalls/
    - evals/
      - evals.json
    - references/
      - experiments.md
    - SKILL.md
  - popups/
    - evals/
      - evals.json
    - SKILL.md
  - pricing/
    - evals/
      - evals.json
    - references/
      - research-methods.md
      - tier-structure.md
    - SKILL.md
  - product-marketing/
    - evals/
      - evals.json
    - SKILL.md
  - programmatic-seo/
    - evals/
      - evals.json
    - references/
      - playbooks.md
    - SKILL.md
  - prospecting/
    - evals/
      - evals.json
    - references/
      - b2b-prospecting.md
      - compliance.md
      - data-sources.md
      - local-prospecting.md
      - saas-prospecting.md
    - SKILL.md
  - public-relations/
    - references/
      - journalist-pitching.md
      - media-outlets.md
      - newsjacking.md
      - press-platforms.md
    - SKILL.md
  - referrals/
    - evals/
      - evals.json
    - references/
      - affiliate-programs.md
      - program-examples.md
    - SKILL.md
  - revops/
    - evals/
      - evals.json
    - references/
      - automation-playbooks.md
      - lifecycle-definitions.md
      - routing-rules.md
      - scoring-models.md
    - SKILL.md
  - sales-enablement/
    - evals/
      - evals.json
    - references/
      - deck-frameworks.md
      - demo-scripts.md
      - objection-library.md
      - one-pager-templates.md
    - SKILL.md
  - schema/
    - evals/
      - evals.json
    - references/
      - schema-examples.md
    - SKILL.md
  - seo-audit/
    - evals/
      - evals.json
    - references/
      - ai-writing-detection.md
      - international-seo.md
    - SKILL.md
  - signup/
    - evals/
      - evals.json
    - SKILL.md
  - site-architecture/
    - evals/
      - evals.json
    - references/
      - mermaid-templates.md
      - navigation-patterns.md
      - site-type-templates.md
    - SKILL.md
  - sms/
    - evals/
      - evals.json
    - references/
      - compliance.md
      - platforms.md
      - sequence-templates.md
    - SKILL.md
  - social/
    - evals/
      - evals.json
    - references/
      - listening-sources-template.md
      - listening.md
      - platform-limits.md
      - platforms.md
      - post-templates.md
      - reverse-engineering.md
      - short-form-video.md
    - SKILL.md
  - video/
    - evals/
      - evals.json
    - references/
      - ai-video-prompting.md
    - SKILL.md
- tools/
  - clis/
    - activecampaign.js
    - adobe-analytics.js
    - ahrefs.js
    - airops.js
    - amplitude.js
    - apollo.js
    - beehiiv.js
    - brevo.js
    - buffer.js
    - calendly.js
    - clay.js
    - clearbit.js
    - close.js
    - coupler.js
    - crossbeam.js
    - customer-io.js
    - dataforseo.js
    - demio.js
    - dub.js
    - exa.js
    - g2.js
    - ga4.js
    - github-prospects.js
    - google-ads.js
    - google-search-console.js
    - hotjar.js
    - hunter.js
    - instantly.js
    - intercom.js
    - keywords-everywhere.js
    - kit.js
    - klaviyo.js
    - lemlist.js
    - linkedin-ads.js
    - livestorm.js
    - mailchimp.js
    - mention-me.js
    - meta-ads.js
    - mixpanel.js
    - onesignal.js
    - optimizely.js
    - outreach.js
    - paddle.js
    - partnerstack.js
    - pendo.js
    - plausible.js
    - postmark.js
    - rankparse.js
    - README.md
    - resend.js
    - rewardful.js
    - savvycal.js
    - segment.js
    - semrush.js
    - sendgrid.js
    - similarweb.js
    - snov.js
    - supermetrics.js
    - tiktok-ads.js
    - tolt.js
    - trustpilot.js
    - typeform.js
    - wistia.js
    - zapier.js
    - zoominfo.js
  - composio/
    - marketing-tools.md
    - README.md
  - integrations/
    - activecampaign.md
    - adobe-analytics.md
    - ahrefs.md
    - airops.md
    - amplitude.md
    - apollo.md
    - attentive.md
    - audiencetap.md
    - beehiiv.md
    - brevo.md
    - browserbase.md
    - buffer.md
    - calendly.md
    - clay.md
    - clearbit.md
    - close.md
    - cogny.md
    - composio.md
    - contentful.md
    - coupler.md
    - crossbeam.md
    - customer-io.md
    - dataforseo.md
    - demio.md
    - dub-co.md
    - exa.md
    - firecrawl.md
    - firehose.md
    - g2.md
    - ga4.md
    - github.md
    - gong.md
    - google-ads.md
    - google-search-console.md
    - heygen.md
    - hotjar.md
    - hubspot.md
    - hunter.md
    - hyperframes.md
    - instantly.md
    - intercom.md
    - introw.md
    - keywords-everywhere.md
    - kit.md
    - klaviyo.md
    - lemlist.md
    - linkedin-ads.md
    - livestorm.md
    - mailchimp.md
    - mention-me.md
    - meta-ads.md
    - mixpanel.md
    - nitrosend.md
    - onesignal.md
    - optimizely.md
    - outreach.md
    - paddle.md
    - partnerstack.md
    - pendo.md
    - plausible.md
    - plivo.md
    - posthog.md
    - postmark.md
    - postscript.md
    - rankparse.md
    - rb2b.md
    - resend.md
    - rewardful.md
    - salesforce.md
    - sanity.md
    - savvycal.md
    - segment.md
    - semrush.md
    - sendgrid.md
    - sequenzy.md
    - shopify.md
    - similarweb.md
    - snov.md
    - sparktoro.md
    - strapi.md
    - stripe.md
    - supermetrics.md
    - tiktok-ads.md
    - tolt.md
    - truelist.md
    - trustpilot.md
    - twilio.md
    - typeform.md
    - webflow.md
    - wistia.md
    - wordpress.md
    - zapier.md
    - zoominfo.md
  - REGISTRY.md
- validate-skills-official.sh
- validate-skills.sh
- VERSIONS.md
```
