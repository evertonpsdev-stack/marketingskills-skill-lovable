# References — coreyhaines31/marketingskills

Docs copiados do repositório (25 arquivos).

---

## `README.md`

# Marketing Skills for AI Agents

A collection of AI agent skills focused on marketing tasks. Built for technical marketers and founders who want AI coding agents to help with conversion optimization, copywriting, SEO, analytics, and growth engineering. Works with Claude Code, OpenAI Codex, Cursor, Windsurf, and any agent that supports the [Agent Skills spec](https://agentskills.io).

Built by [Corey Haines](https://corey.co?ref=marketingskills). Need hands-on help? Check out [Conversion Factory](https://conversionfactory.co?ref=marketingskills) — Corey's agency for conversion optimization, landing pages, and growth strategy. Want to learn more about marketing? Subscribe to [Swipe Files](https://swipefiles.com?ref=marketingskills). Want to get dangerously good at using AI for marketing? Check out [AI Marketing Training](https://conversionfactory.co/offers/ai-marketing-training?ref=marketingskills). Want an autonomous AI agent that uses these skills to be your CMO? Try [Magister](https://magistermarketing.com?ref=marketingskills).

New to the terminal and coding agents? Check out the companion guide [Coding for Marketers](https://codingformarketers.com?ref=marketingskills).

**Contributions welcome!** Found a way to improve a skill or have a new one to add? [Open a PR](#contributing).

Run into a problem or have a question? [Open an issue](https://github.com/coreyhaines31/marketingskills/issues) — we're happy to help.

## What are Skills?

Skills are markdown files that give AI agents specialized knowledge and workflows for specific tasks. When you add these to your project, your agent can recognize when you're working on a marketing task and apply the right frameworks and best practices.

## How Skills Work Together

Skills reference each other and build on shared context. The `product-marketing` skill is the foundation — every other skill checks it first to understand your product, audience, and positioning before doing anything.

```
                            ┌──────────────────────────────────────┐
                            │          product-marketing           │
                            │    (read by all other skills first)  │
                            └──────────────────┬───────────────────┘
                                               │
    ┌──────────────┬─────────────┬─────────────┼─────────────┬──────────────┬──────────────┐
    ▼              ▼             ▼             ▼             ▼              ▼              ▼
┌──────────┐ ┌──────────┐ ┌──────────┐ ┌────────────┐ ┌──────────┐ ┌─────────────┐ ┌───────────┐
│  SEO &   │ │   CRO    │ │Content & │ │  Paid &    │ │ Growth & │ │  Sales &    │ │ Strategy  │
│ Content  │ │          │ │   Copy   │ │Measurement │ │Retention │ │    GTM      │ │           │
├──────────┤ ├──────────┤ ├──────────┤ ├────────────┤ ├──────────┤ ├─────────────┤ ├───────────┤
│seo-audit │ │cro       │ │copywritng│ │ads         │ │referrals │ │revops       │ │mktg-ideas │
│ai-seo    │ │signup    │ │copy-edit │ │ad-creative │ │free-tools│ │sales-enable │ │mktg-psych │
│site-arch │ │onboarding│ │cold-email│ │ab-testing  │ │churn-    │ │launch       │ │customer-  │
│programm  │ │popups    │ │emails    │ │analytics   │ │ prevent  │ │pricing      │ │ research  │
│schema    │ │paywalls  │ │social    │ │            │ │community │ │competitors  │ │           │
│content   │ │          │ │video     │ │            │ │lead-magnt│ │comp-profile │ │           │
│aso       │ │          │ │image     │ │            │ │co-mktg   │ │directory    │ │           │
│          │ │          │ │sms       │ │            │ │          │ │prospecting  │ │           │
└────┬─────┘ └────┬─────┘ └────┬─────┘ └─────┬──────┘ └────┬─────┘ └──────┬──────┘ └─────┬─────┘
     │            │            │              │             │              │              │
     └────────────┴─────┬──────┴──────────────┴─────────────┴──────────────┴──────────────┘
                        │
         Skills cross-reference each other:
           copywriting ↔ cro ↔ ab-testing
           revops ↔ sales-enablement ↔ cold-email
           seo-audit ↔ schema ↔ ai-seo
           customer-research → copywriting, cro, competitors
```

See each skill's **Related Skills** section for the full dependency map.

## Available Skills

<!-- SKILLS:START -->
| Skill | Description |
|-------|-------------|
| [ab-testing](skills/ab-testing/) | When the user wants to plan, design, or implement an A/B test or experiment, or build a growth experimentation program.... |
| [ad-creative](skills/ad-creative/) | When the user wants to generate, iterate, or scale ad creative — headlines, descriptions, primary text, or full ad... |
| [ads](skills/ads/) | When the user wants help with paid advertising campaigns on Google Ads, Meta (Facebook/Instagram), LinkedIn, Twitter/X,... |
| [ai-seo](skills/ai-seo/) | When the user wants to optimize content for AI search engines, get cited by LLMs, or appear in AI-generated answers.... |
| [analytics](skills/analytics/) | When the user wants to set up, improve, or audit analytics tracking and measurement. Also use when the user mentions... |
| [aso](skills/aso/) | When the user wants to audit or optimize an App Store or Google Play listing. Also use when the user mentions 'ASO... |
| [churn-prevention](skills/churn-prevention/) | When the user wants to reduce churn, build cancellation flows, set up save offers, recover failed payments, or... |
| [co-marketing](skills/co-marketing/) | When the user wants to find co-marketing partners, plan joint campaigns, or brainstorm partnership opportunities. Use... |
| [cold-email](skills/cold-email/) | Write B2B cold emails and follow-up sequences that get replies. Use when the user wants to write cold outreach emails,... |
| [community-marketing](skills/community-marketing/) | Build and leverage online communities to drive product growth and brand loyalty. Use when the user wants to create a... |
| [competitor-profiling](skills/competitor-profiling/) | When the user wants to research, profile, or analyze competitors from their URLs. Also use when the user mentions... |
| [competitors](skills/competitors/) | When the user wants to create competitor comparison or alternative pages for SEO and sales enablement. Also use when... |
| [content-strategy](skills/content-strategy/) | When the user wants to plan a content strategy, decide what content to create, or figure out what topics to cover. Also... |
| [copy-editing](skills/copy-editing/) | When the user wants to edit, review, or improve existing marketing copy, or refresh outdated content. Also use when the... |
| [copywriting](skills/copywriting/) | When the user wants to write, rewrite, or improve marketing copy for any page — including homepage, landing pages,... |
| [cro](skills/cro/) | When the user wants to optimize, improve, or increase conversions on any marketing page or form — including homepage,... |
| [customer-research](skills/customer-research/) | When the user wants to conduct, analyze, or synthesize customer research. Use when the user mentions "customer... |
| [directory-submissions](skills/directory-submissions/) | When the user wants to submit their product to startup, SaaS, AI, agent, MCP, no-code, or review directories for... |
| [emails](skills/emails/) | When the user wants to create or optimize an email sequence, drip campaign, automated email flow, or lifecycle email... |
| [free-tools](skills/free-tools/) | When the user wants to plan, evaluate, or build a free tool for marketing purposes — lead generation, SEO value, or... |
| [image](skills/image/) | When the user wants to create, generate, edit, or optimize images for marketing — blog heroes, social graphics, product... |
| [launch](skills/launch/) | When the user wants to plan a product launch, feature announcement, or release strategy. Also use when the user... |
| [lead-magnets](skills/lead-magnets/) | When the user wants to create, plan, or optimize a lead magnet for email capture or lead generation. Also use when the... |
| [marketing-ideas](skills/marketing-ideas/) | When the user needs marketing ideas, inspiration, or strategies for their SaaS or software product. Also use when the... |
| [marketing-plan](skills/marketing-plan/) | When the user needs a comprehensive marketing plan for a client, a company they advise, or their own product. Also use... |
| [marketing-psychology](skills/marketing-psychology/) | When the user wants to apply psychological principles, mental models, or behavioral science to marketing. Also use when... |
| [offers](skills/offers/) | When the user wants to design, construct, or improve an offer — the thing they actually sell — including value framing,... |
| [onboarding](skills/onboarding/) | When the user wants to optimize post-signup onboarding, user activation, first-run experience, or time-to-value. Also... |
| [paywalls](skills/paywalls/) | When the user wants to create or optimize in-app paywalls, upgrade screens, upsell modals, or feature gates. Also use... |
| [popups](skills/popups/) | When the user wants to create or optimize popups, modals, overlays, slide-ins, or banners for conversion purposes. Also... |
| [pricing](skills/pricing/) | When the user wants help with pricing decisions, packaging, or monetization strategy. Also use when the user mentions... |
| [product-marketing](skills/product-marketing/) | When the user wants to create or update their product marketing context document. Also use when the user mentions... |
| [programmatic-seo](skills/programmatic-seo/) | When the user wants to create SEO-driven pages at scale using templates and data. Also use when the user mentions... |
| [prospecting](skills/prospecting/) | When the user wants to find, qualify, and build a list of prospects to reach out to — across B2B SaaS, general B2B, or... |
| [public-relations](skills/public-relations/) | When the user wants help with public relations, earned media, press coverage, journalist outreach, or media strategy... |
| [referrals](skills/referrals/) | When the user wants to create, optimize, or analyze a referral program, affiliate program, or word-of-mouth strategy.... |
| [revops](skills/revops/) | When the user wants help with revenue operations, lead lifecycle management, or marketing-to-sales handoff processes.... |
| [sales-enablement](skills/sales-enablement/) | When the user wants to create sales collateral, pitch decks, one-pagers, objection handling docs, or demo scripts. Also... |
| [schema](skills/schema/) | When the user wants to add, fix, or optimize schema markup and structured data on their site. Also use when the user... |
| [seo-audit](skills/seo-audit/) | When the user wants to audit, review, or diagnose SEO issues on their site. Also use when the user mentions "SEO... |
| [signup](skills/signup/) | When the user wants to optimize signup, registration, account creation, or trial activation flows. Also use when the... |
| [site-architecture](skills/site-architecture/) | When the user wants to plan, map, or restructure their website's page hierarchy, navigation, URL structure, or internal... |
| [sms](skills/sms/) | When the user wants to plan, build, or optimize SMS or MMS marketing — including welcome flows, abandoned cart texts,... |
| [social](skills/social/) | When the user wants help creating, scheduling, or optimizing social media content for LinkedIn, Twitter/X, Instagram,... |
| [video](skills/video/) | When the user wants to create, generate, or produce video content using AI tools or programmatic frameworks. Also use... |
<!-- SKILLS:END -->

## Installation

### Option 1: CLI Install (Recommended)

Use [npx skills](https://github.com/vercel-labs/skills) to install skills directly:

```bash
# Install all skills
npx skills add coreyhaines31/marketingskills

# Install specific skills
npx skills add coreyhaines31/marketingskills --skill cro copywriting

# List available skills
npx skills add coreyhaines31/marketingskills --list
```

This automatically installs to your `.agents/skills/` directory (and symlinks into `.claude/skills/` for Claude Code compatibility).

### Option 2: Claude Code Plugin

Install via Claude Code's built-in plugin system:

```bash
# Add the marketplace
/plugin marketplace add coreyhaines31/marketingskills

# Install all marketing skills
/plugin install marketing-skills
```

### Option 3: Clone and Copy

Clone the entire repo and copy the skills folder:

```bash
git clone https://github.com/coreyhaines31/marketingskills.git
cp -r marketingskills/skills/* .agents/skills/
```

### Option 4: Git Submodule

Add as a submodule for easy updates:

```bash
git submodule add https://github.com/coreyhaines31/marketingskills.git .agents/marketingskills
```

Then reference skills from `.agents/marketingskills/skills/`.

### Option 5: Fork and Customize

1. Fork this repository
2. Customize skills for your specific needs
3. Clone your fork into your projects

### Option 6: SkillKit (Multi-Agent)

Use [SkillKit](https://github.com/rohitg00/skillkit) to install skills across multiple AI agents (Claude Code, Cursor, Copilot, etc.):

```bash
# Install all skills
npx skillkit install coreyhaines31/marketingskills

# Install specific skills
npx skillkit install coreyhaines31/marketingskills --skill cro copywriting

# List available skills
npx skillkit install coreyhaines31/marketingskills --list
```

## Upgrading from v1.x to v2.0

v2.0 renames 17 skills and consolidates `page-cro` + `form-cro` into a single `cro` skill. If you installed the v1.x skills, you'll have **stale old-name folders** in your install directory after upgrading — the new skills install alongside the old ones, so you'll see both `skills/page-cro/` and `skills/cro/`, etc. Clean them up:

```bash
# From the directory where you installed the skills (e.g., .agents/skills/ or .claude/skills/)
rm -rf page-cro form-cro \
       ab-test-setup analytics-tracking aso-audit competitor-alternatives \
       email-sequence free-tool-strategy launch-strategy onboarding-cro \
       paid-ads paywall-upgrade-cro popup-cro pricing-strategy \
       product-marketing-context referral-program schema-markup \
       signup-flow-cro social-content
```

Then reinstall the v2.0 skills via your usual method (e.g., `npx skills add coreyhaines31/marketingskills`).

### Migrate the product marketing context file

In v2.0 the context file moved from `.claude/` to `.agents/` and was renamed from `product-marketing-context.md` to `product-marketing.md`. Move your existing context file:

```bash
mkdir -p .agents
# v2.0 file (or pre-v2.0 file with new name)
mv .claude/product-marketing.md .agents/product-marketing.md 2>/dev/null
# pre-v2.0 file with legacy name
mv .claude/product-marketing-context.md .agents/product-marketing.md 2>/dev/null
```

Skills will still check `.claude/` and the legacy `product-marketing-context.md` filename as fallbacks, so nothing breaks if you don't migrate.

### Full rename map

| Old | New |
|-----|-----|
| `ab-test-setup` | `ab-testing` |
| `analytics-tracking` | `analytics` |
| `aso-audit` | `aso` |
| `competitor-alternatives` | `competitors` |
| `email-sequence` | `emails` |
| `form-cro` | merged into `cro` |
| `free-tool-strategy` | `free-tools` |
| `launch-strategy` | `launch` |
| `onboarding-cro` | `onboarding` |
| `page-cro` | `cro` |
| `paid-ads` | `ads` |
| `paywall-upgrade-cro` | `paywalls` |
| `popup-cro` | `popups` |
| `pricing-strategy` | `pricing` |
| `product-marketing-context` | `product-marketing` |
| `referral-program` | `referrals` |
| `schema-markup` | `schema` |
| `signup-flow-cro` | `signup` |
| `social-content` | `social` |

## Usage

Once installed, just ask your agent to help with marketing tasks:

```
"Help me optimize this landing page for conversions"
→ Uses cro skill

"Write homepage copy for my SaaS"
→ Uses copywriting skill

"Set up GA4 tracking for signups"
→ Uses analytics skill

"Create a 5-email welcome sequence"
→ Uses emails skill
```

You can also invoke skills directly:

```
/cro
/emails
/seo-audit
```

## Skill Categories

### Conversion Optimization
- `cro` - Pages and forms
- `signup` - Registration flows
- `onboarding` - Post-signup activation
- `popups` - Modals and overlays
- `paywalls` - In-app upgrade moments

### Content & Copy
- `copywriting` - Marketing page copy
- `copy-editing` - Edit and polish existing copy
- `cold-email` - B2B cold outreach emails and sequences
- `emails` - Automated email flows
- `social` - Social media content
- `image` - AI image generation, design tools, and optimization

### SEO & Discovery
- `seo-audit` - Technical and on-page SEO
- `ai-seo` - AI search optimization (AEO, GEO, LLMO)
- `programmatic-seo` - Scaled page generation
- `site-architecture` - Page hierarchy, navigation, URL structure
- `competitors` - Comparison and alternative pages
- `schema` - Structured data

### Paid & Distribution
- `ads` - Google, Meta, LinkedIn ad campaigns
- `ad-creative` - Bulk ad creative generation and iteration
- `social` - Social media scheduling and strategy

### Measurement & Testing
- `analytics` - Event tracking setup
- `ab-testing` - Experiment design

### Retention
- `churn-prevention` - Cancel flows, save offers, dunning, payment recovery

### Growth Engineering
- `co-marketing` - Partner identification and joint campaigns
- `free-tools` - Marketing tools and calculators
- `referrals` - Referral and affiliate programs

### Strategy & Monetization
- `marketing-ideas` - 140 SaaS marketing ideas
- `marketing-psychology` - Mental models and psychology
- `launch` - Product launches and announcements
- `pricing` - Pricing, packaging, and monetization

### Sales & RevOps
- `revops` - Lead lifecycle, scoring, routing, pipeline management
- `sales-enablement` - Sales decks, one-pagers, objection docs, demo scripts

## Contributing

Found a way to improve a skill? Have a new skill to suggest? PRs and issues welcome!

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding or improving skills.

## License

[MIT](LICENSE) - Use these however you want.

---

## `tools/clis/README.md`

# Marketing CLIs

Zero-dependency, single-file CLI tools for marketing platforms that don't ship their own.

Every CLI is a standalone Node.js script (Node 18+) with no `npm install` required — just `chmod +x` and go.

## Install

### Option 1: Run directly

```bash
node tools/clis/ahrefs.js backlinks list --target example.com
```

### Option 2: Symlink for global access

```bash
# Symlink any CLI you want available globally
ln -sf "$(pwd)/tools/clis/ahrefs.js" ~/.local/bin/ahrefs
ln -sf "$(pwd)/tools/clis/resend.js" ~/.local/bin/resend

# Then use directly
ahrefs backlinks list --target example.com
resend send --from you@example.com --to them@example.com --subject "Hello" --html "<p>Hi</p>"
```

### Option 3: Add the whole directory to PATH

```bash
export PATH="$PATH:/path/to/marketingskills/tools/clis"
```

## Authentication

Every CLI reads credentials from environment variables:

| CLI | Environment Variable |
|-----|---------------------|
| `activecampaign` | `ACTIVECAMPAIGN_API_KEY`, `ACTIVECAMPAIGN_API_URL` |
| `adobe-analytics` | `ADOBE_ACCESS_TOKEN`, `ADOBE_CLIENT_ID`, `ADOBE_COMPANY_ID` |
| `ahrefs` | `AHREFS_API_KEY` |
| `amplitude` | `AMPLITUDE_API_KEY`, `AMPLITUDE_SECRET_KEY` |
| `apollo` | `APOLLO_API_KEY` |
| `beehiiv` | `BEEHIIV_API_KEY` |
| `brevo` | `BREVO_API_KEY` |
| `buffer` | `BUFFER_API_KEY` |
| `calendly` | `CALENDLY_API_KEY` |
| `clearbit` | `CLEARBIT_API_KEY` |
| `customer-io` | `CUSTOMERIO_APP_KEY` (App API), `CUSTOMERIO_SITE_ID` + `CUSTOMERIO_API_KEY` (Track API) |
| `dataforseo` | `DATAFORSEO_LOGIN`, `DATAFORSEO_PASSWORD` |
| `demio` | `DEMIO_API_KEY`, `DEMIO_API_SECRET` |
| `dub` | `DUB_API_KEY` |
| `exa` | `EXA_API_KEY` |
| `g2` | `G2_API_TOKEN` |
| `ga4` | `GA4_ACCESS_TOKEN` |
| `google-ads` | `GOOGLE_ADS_TOKEN`, `GOOGLE_ADS_DEVELOPER_TOKEN`, `GOOGLE_ADS_CUSTOMER_ID` |
| `google-search-console` | `GSC_ACCESS_TOKEN` |
| `hotjar` | `HOTJAR_CLIENT_ID`, `HOTJAR_CLIENT_SECRET` |
| `intercom` | `INTERCOM_API_KEY` |
| `keywords-everywhere` | `KEYWORDS_EVERYWHERE_API_KEY` |
| `kit` | `KIT_API_KEY`, `KIT_API_SECRET` |
| `klaviyo` | `KLAVIYO_API_KEY` |
| `linkedin-ads` | `LINKEDIN_ACCESS_TOKEN` |
| `livestorm` | `LIVESTORM_API_TOKEN` |
| `mailchimp` | `MAILCHIMP_API_KEY` |
| `mention-me` | `MENTIONME_API_KEY` |
| `meta-ads` | `META_ACCESS_TOKEN`, `META_AD_ACCOUNT_ID` |
| `mixpanel` | `MIXPANEL_TOKEN` (ingestion), `MIXPANEL_API_KEY` + `MIXPANEL_SECRET` (query) |
| `onesignal` | `ONESIGNAL_REST_API_KEY`, `ONESIGNAL_APP_ID` |
| `optimizely` | `OPTIMIZELY_API_KEY` |
| `paddle` | `PADDLE_API_KEY`, `PADDLE_SANDBOX` (optional) |
| `partnerstack` | `PARTNERSTACK_PUBLIC_KEY`, `PARTNERSTACK_SECRET_KEY` |
| `plausible` | `PLAUSIBLE_API_KEY`, `PLAUSIBLE_BASE_URL` (optional, for self-hosted) |
| `postmark` | `POSTMARK_API_KEY` |
| `resend` | `RESEND_API_KEY` |
| `rewardful` | `REWARDFUL_API_KEY` |
| `savvycal` | `SAVVYCAL_API_KEY` |
| `segment` | `SEGMENT_WRITE_KEY` (tracking), `SEGMENT_ACCESS_TOKEN` (profile) |
| `semrush` | `SEMRUSH_API_KEY` |
| `sendgrid` | `SENDGRID_API_KEY` |
| `tiktok-ads` | `TIKTOK_ACCESS_TOKEN`, `TIKTOK_ADVERTISER_ID` |
| `tolt` | `TOLT_API_KEY` |
| `trustpilot` | `TRUSTPILOT_API_KEY`, `TRUSTPILOT_API_SECRET`, `TRUSTPILOT_BUSINESS_UNIT_ID` |
| `typeform` | `TYPEFORM_API_KEY` |
| `hunter` | `HUNTER_API_KEY` |
| `instantly` | `INSTANTLY_API_KEY` |
| `lemlist` | `LEMLIST_API_KEY` |
| `snov` | `SNOV_CLIENT_ID`, `SNOV_CLIENT_SECRET` |
| `wistia` | `WISTIA_API_KEY` |
| `zapier` | `ZAPIER_API_KEY` |

## Security

**Never hardcode API keys or tokens in scripts.** All CLIs read credentials exclusively from environment variables.

- Store keys in your shell profile (`~/.zshrc`, `~/.bashrc`) or a `.env` file
- The `.env` file is gitignored — but double-check before committing
- Use `--dry-run` on any command to preview the request without sending it (credentials are masked as `***`)
- If you fork this repo, audit your commits to ensure no secrets are included

## Command Pattern

All CLIs follow the same structure:

```
{tool} <resource> <action> [options]
```

Examples:

```bash
ahrefs backlinks list --target example.com --limit 50
semrush keywords overview --phrase "marketing automation" --database us
mailchimp campaigns list --limit 20
resend send --from you@example.com --to them@example.com --subject "Hello" --html "<p>Hi</p>"
dub links create --url https://example.com/landing --key summer-sale
```

## Output

All CLIs output JSON to stdout for easy piping:

```bash
# Pipe to jq
ahrefs backlinks list --target example.com | jq '.backlinks[].url_from'

# Save to file
semrush keywords overview --phrase "saas marketing" --database us > keywords.json

# Use in scripts
DOMAINS=$(rewardful affiliates list | jq -r '.data[].email')
```

## Available CLIs

| CLI | Category | Tool |
|-----|----------|------|
| `activecampaign.js` | Email/CRM | [ActiveCampaign](https://activecampaign.com) |
| `adobe-analytics.js` | Analytics | [Adobe Analytics](https://business.adobe.com/products/analytics) |
| `ahrefs.js` | SEO | [Ahrefs](https://ahrefs.com) |
| `amplitude.js` | Analytics | [Amplitude](https://amplitude.com) |
| `apollo.js` | Data Enrichment | [Apollo.io](https://apollo.io) |
| `beehiiv.js` | Newsletter | [Beehiiv](https://beehiiv.com) |
| `brevo.js` | Email/SMS | [Brevo](https://brevo.com) |
| `buffer.js` | Social | [Buffer](https://buffer.com) |
| `calendly.js` | Scheduling | [Calendly](https://calendly.com) |
| `clearbit.js` | Data Enrichment | [Clearbit](https://clearbit.com) |
| `customer-io.js` | Email | [Customer.io](https://customer.io) |
| `dataforseo.js` | SEO | [DataForSEO](https://dataforseo.com) |
| `demio.js` | Webinar | [Demio](https://demio.com) |
| `dub.js` | Links | [Dub.co](https://dub.co) |
| `exa.js` | AI Search | [Exa](https://exa.ai) |
| `g2.js` | Reviews | [G2](https://g2.com) |
| `ga4.js` | Analytics | [Google Analytics 4](https://analytics.google.com) |
| `google-ads.js` | Ads | [Google Ads](https://ads.google.com) |
| `google-search-console.js` | SEO | [Google Search Console](https://search.google.com/search-console) |
| `hotjar.js` | CRO | [Hotjar](https://hotjar.com) |
| `hunter.js` | Email Outreach | [Hunter.io](https://hunter.io) |
| `instantly.js` | Email Outreach | [Instantly.ai](https://instantly.ai) |
| `intercom.js` | Messaging | [Intercom](https://intercom.com) |
| `keywords-everywhere.js` | SEO | [Keywords Everywhere](https://keywordseverywhere.com) |
| `kit.js` | Email | [Kit](https://kit.com) |
| `klaviyo.js` | Email/SMS | [Klaviyo](https://klaviyo.com) |
| `lemlist.js` | Email Outreach | [Lemlist](https://lemlist.com) |
| `linkedin-ads.js` | Ads | [LinkedIn Ads](https://business.linkedin.com/marketing-solutions/ads) |
| `livestorm.js` | Webinar | [Livestorm](https://livestorm.co) |
| `mailchimp.js` | Email | [Mailchimp](https://mailchimp.com) |
| `mention-me.js` | Referral | [Mention Me](https://www.mention-me.com) |
| `meta-ads.js` | Ads | [Meta Ads](https://www.facebook.com/business/ads) |
| `mixpanel.js` | Analytics | [Mixpanel](https://mixpanel.com) |
| `onesignal.js` | Push | [OneSignal](https://onesignal.com) |
| `optimizely.js` | A/B Testing | [Optimizely](https://optimizely.com) |
| `paddle.js` | Payments | [Paddle](https://paddle.com) |
| `partnerstack.js` | Affiliate | [PartnerStack](https://partnerstack.com) |
| `plausible.js` | Analytics | [Plausible](https://plausible.io) |
| `postmark.js` | Email | [Postmark](https://postmarkapp.com) |
| `resend.js` | Email | [Resend](https://resend.com) |
| `rewardful.js` | Referral | [Rewardful](https://www.getrewardful.com) |
| `savvycal.js` | Scheduling | [SavvyCal](https://savvycal.com) |
| `segment.js` | Analytics | [Segment](https://segment.com) |
| `semrush.js` | SEO | [SEMrush](https://semrush.com) |
| `sendgrid.js` | Email | [SendGrid](https://sendgrid.com) |
| `snov.js` | Email Outreach | [Snov.io](https://snov.io) |
| `tiktok-ads.js` | Ads | [TikTok Ads](https://ads.tiktok.com) |
| `tolt.js` | Referral | [Tolt](https://tolt.io) |
| `trustpilot.js` | Reviews | [Trustpilot](https://trustpilot.com) |
| `typeform.js` | Forms | [Typeform](https://typeform.com) |
| `wistia.js` | Video | [Wistia](https://wistia.com) |
| `zapier.js` | Automation | [Zapier](https://zapier.com) |

---

## `tools/composio/README.md`

# Composio Quick Start

Get MCP access to 500+ marketing tools through a single integration.

## Prerequisites

- Node.js 18+
- Claude Code installed

## Install

```bash
npx @composio/mcp@latest setup
```

Verify by running `/mcp` in Claude Code — `composio` should appear in the server list.

## Connect a Tool

When you ask the agent to use a Composio-backed tool for the first time, it will provide a Connect Link. Open the link in your browser, authorize the app, and you're set. The connection persists across sessions.

```
You: "Get my top HubSpot contacts"
Agent: "Please connect HubSpot first: https://app.composio.dev/connect/..."
# Click the link → authorize → return to Claude Code
Agent: "Here are your top contacts: ..."
```

## Usage Examples

### Pull CRM contacts

```
"Show me my 10 most recent HubSpot contacts with their deal stages"
```

### Get ad performance

```
"What's my Meta Ads spend and ROAS for the last 7 days?"
```

### Write to a spreadsheet

```
"Add a row to my 'Campaign Tracker' Google Sheet with today's LinkedIn Ads metrics"
```

### Cross-tool workflow

```
"Find Salesforce leads from this week and post a summary in Slack #new-leads"
```

## Available Marketing Tools

See [marketing-tools.md](marketing-tools.md) for the full list of Composio toolkits mapped to marketing use cases.

Key tools with new MCP access (no native MCP server in this repo):
- **HubSpot** — contacts, deals, companies, lists
- **Salesforce** — SOQL queries, leads, opportunities
- **Meta Ads** — campaigns, ad sets, insights
- **LinkedIn Ads** — campaigns, analytics
- **Google Sheets** — read, write, create spreadsheets
- **Slack** — messages, channels
- **Notion** — pages, databases
- **Klaviyo** — profiles, lists, campaigns
- **ActiveCampaign** — contacts, automations

## Troubleshooting

### "Tool not found" error

The tool may not be connected yet. Ask the agent to connect it, or run:

```bash
npx composio apps list
```

### Expired authentication

OAuth tokens expire. If a tool stops working, re-authenticate:

```bash
npx composio connections list    # Find the connection
npx composio connections remove {id}  # Remove it
# Then ask the agent to use the tool again to trigger re-auth
```

### Rate limit errors

Composio has its own rate limits (free: 20K calls/mo, 10 req/sec). If you hit them:
- Reduce request frequency
- Upgrade your Composio plan
- Use native CLI tools for high-volume operations

### MCP server not appearing

Re-run the setup command:

```bash
npx @composio/mcp@latest setup
```

Then restart Claude Code.

---

## `CLAUDE.md`

AGENTS.md

---

## `AGENTS.md`

# AGENTS.md

Guidelines for AI agents working in this repository.

## Repository Overview

This repository contains **Agent Skills** for AI agents following the [Agent Skills specification](https://agentskills.io/specification.md). Skills install to `.agents/skills/` (the cross-agent standard). This repo also serves as a **Claude Code plugin marketplace** via `.claude-plugin/marketplace.json`.

- **Name**: Marketing Skills
- **GitHub**: [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)
- **Creator**: Corey Haines
- **License**: MIT

## Repository Structure

```
marketingskills/
├── .claude-plugin/
│   └── marketplace.json   # Claude Code plugin marketplace manifest
├── skills/                # Agent Skills
│   └── skill-name/
│       └── SKILL.md       # Required skill file
├── tools/
│   ├── clis/              # Zero-dependency Node.js CLI tools (51 tools)
│   ├── composio/          # Composio integration layer (quick start + toolkit mapping)
│   ├── integrations/      # API integration guides per tool
│   └── REGISTRY.md        # Tool index with capabilities
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```

## Build / Lint / Test Commands

**Skills** are content-only (no build step). Verify manually:
- YAML frontmatter is valid
- `name` field matches directory name exactly
- `name` is 1-64 chars, lowercase alphanumeric and hyphens only
- `description` is 1-1024 characters

**CLI tools** (`tools/clis/*.js`) are zero-dependency Node.js scripts (Node 18+). Verify with:
```bash
node --check tools/clis/<name>.js   # Syntax check
node tools/clis/<name>.js           # Show usage (no args = help)
node tools/clis/<name>.js <cmd> --dry-run  # Preview request without sending
```

## Agent Skills Specification

Skills follow the [Agent Skills spec](https://agentskills.io/specification.md).

### Required Frontmatter

```yaml
---
name: skill-name
description: What this skill does and when to use it. Include trigger phrases.
---
```

### Frontmatter Field Constraints

| Field         | Required | Constraints                                                      |
|---------------|----------|------------------------------------------------------------------|
| `name`        | Yes      | 1-64 chars, lowercase `a-z`, numbers, hyphens. Must match dir.   |
| `description` | Yes      | 1-1024 chars. Describe what it does and when to use it.          |
| `license`     | No       | License name (default: MIT)                                      |
| `metadata`    | No       | Key-value pairs (author, version, etc.)                          |

### Name Field Rules

- Lowercase letters, numbers, and hyphens only
- Cannot start or end with hyphen
- No consecutive hyphens (`--`)
- Must match parent directory name exactly

**Valid**: `cro`, `emails`, `ab-testing`
**Invalid**: `Page-CRO`, `-page`, `page--cro`

### Optional Skill Directories

```
skills/skill-name/
├── SKILL.md        # Required - main instructions (<500 lines)
├── references/     # Optional - detailed docs loaded on demand
├── scripts/        # Optional - executable code
└── assets/         # Optional - templates, data files
```

## Writing Style Guidelines

### Structure

- Keep `SKILL.md` under 500 lines (move details to `references/`)
- Use H2 (`##`) for main sections, H3 (`###`) for subsections
- Use bullet points and numbered lists liberally
- Short paragraphs (2-4 sentences max)

### Tone

- Direct and instructional
- Second person ("You are a conversion rate optimization expert")
- Professional but approachable

### Formatting

- Bold (`**text**`) for key terms
- Code blocks for examples and templates
- Tables for reference data
- No excessive emojis

### Clarity Principles

- Clarity over cleverness
- Specific over vague
- Active voice over passive
- One idea per section

### Description Field Best Practices

The `description` is critical for skill discovery. Include:
1. What the skill does
2. When to use it (trigger phrases)
3. Related skills for scope boundaries

```yaml
description: When the user wants to optimize conversions on any marketing page. Use when the user says "CRO," "conversion rate optimization," "this page isn't converting." For signup flows, see signup.
```

## Claude Code Plugin

This repo also serves as a plugin marketplace. The manifest at `.claude-plugin/marketplace.json` lists all skills for installation via:

```bash
/plugin marketplace add coreyhaines31/marketingskills
/plugin install marketing-skills
```

See [Claude Code plugins documentation](https://code.claude.com/docs/en/plugins.md) for details.

## Git Workflow

### Branch Naming

- New skills: `feature/skill-name`
- Improvements: `fix/skill-name-description`
- Documentation: `docs/description`

### Commit Messages

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

- `feat: add skill-name skill`
- `fix: improve clarity in cro`
- `docs: update README`

### Pull Request Checklist

- [ ] `name` matches directory name exactly
- [ ] `name` follows naming rules (lowercase, hyphens, no `--`)
- [ ] `description` is 1-1024 chars with trigger phrases
- [ ] `SKILL.md` is under 500 lines
- [ ] No sensitive data or credentials

## Tool Integrations

This repository includes a tools registry for agent-compatible marketing tools.

- **Tool discovery**: Read `tools/REGISTRY.md` to see available tools and their capabilities
- **Integration details**: See `tools/integrations/{tool}.md` for API endpoints, auth, and common operations
- **MCP-enabled tools**: ga4, stripe, mailchimp, google-ads, resend, zapier, zoominfo, clay, supermetrics, coupler, outreach, crossbeam, introw, composio
- **Composio** (integration layer): Adds MCP access to OAuth-heavy tools without native MCP servers (HubSpot, Salesforce, Meta Ads, LinkedIn Ads, Google Sheets, Slack, etc.). See `tools/integrations/composio.md`

### Registry Structure

```
tools/
├── REGISTRY.md              # Index of all tools with capabilities
└── integrations/            # Detailed integration guides
    ├── ga4.md
    ├── stripe.md
    ├── rewardful.md
    └── ...
```

### When to Use Tools

Skills reference relevant tools for implementation. For example:
- `referrals` skill → rewardful, tolt, dub-co, mention-me guides
- `analytics` skill → ga4, mixpanel, segment guides
- `emails` skill → customer-io, mailchimp, resend guides
- `ads` skill → google-ads, meta-ads, linkedin-ads guides

For tools without native MCP servers (HubSpot, Salesforce, Meta Ads, LinkedIn Ads, Google Sheets, Slack, Notion), Composio provides MCP access via a single server. See `tools/integrations/composio.md` for setup and `tools/composio/marketing-tools.md` for the full toolkit mapping.

## Checking for Updates

When using any skill from this repository:

1. **Once per session**, on first skill use, check for updates:
   - Fetch `VERSIONS.md` from GitHub: https://raw.githubusercontent.com/coreyhaines31/marketingskills/main/VERSIONS.md
   - Compare versions against local skill files

2. **Only prompt if meaningful**:
   - 2 or more skills have updates, OR
   - Any skill has a major version bump (e.g., 1.x to 2.x)

3. **Non-blocking notification** at end of response:
   ```
   ---
   Skills update available: X marketing skills have updates.
   Say "update skills" to update automatically, or run `git pull` in your marketingskills folder.
   ```

4. **If user says "update skills"**:
   - Run `git pull` in the marketingskills directory
   - Confirm what was updated

## Skill Categories

See `README.md` for the current list of skills organized by category. When adding new skills, follow the naming patterns of existing skills in that category.

## Claude Code-Specific Enhancements

These patterns are **Claude Code only** and must not be added to `SKILL.md` files directly, as skills are designed to be cross-agent compatible (Codex, Cursor, Windsurf, etc.). Apply them locally in your own project's `.claude/skills/` overrides instead.

### Dynamic content injection with `!`command``

Claude Code supports embedding shell commands in SKILL.md using `` !`command` `` syntax. When the skill is invoked, Claude Code runs the command and injects the output inline — the model sees the result, not the instruction.

**Most useful application: auto-inject the product marketing context file**

Instead of every skill telling the agent "go check if `.agents/product-marketing.md` exists and read it," you can inject it automatically:

```markdown
Product context: !`cat .agents/product-marketing.md 2>/dev/null || echo "No product context file found — ask the user about their product before proceeding."`
```

Place this at the top of a skill's body (after frontmatter) to make context available immediately without any file-reading step.

**Other useful injections:**

```markdown
# Inject today's date for recency-sensitive skills
Today's date: !`date +%Y-%m-%d`

# Inject current git branch (useful for workflow skills)
Current branch: !`git branch --show-current 2>/dev/null`

# Inject recent commits for context
Recent commits: !`git log --oneline -5 2>/dev/null`
```

**Why this is Claude Code-only**: Other agents that load skills will see the literal `` !`command` `` string rather than executing it, which would appear as garbled instructions. Keep cross-agent skill files free of this syntax.

---

## `CONTRIBUTING.md`

# Contributing

Thanks for your interest in contributing to Marketing Skills! This guide will help you add new skills or improve existing ones.

## Requesting a Skill

You can also suggest new skills by [opening a skill request](https://github.com/coreyhaines31/marketingskills/issues/new?template=skill-request.yml).

## Adding a New Skill

### 1. Create the skill directory

```bash
mkdir -p skills/your-skill-name
```

### 2. Create the SKILL.md file

Every skill needs a `SKILL.md` file with YAML frontmatter:

```yaml
---
name: your-skill-name
description: When to use this skill. Include trigger phrases and keywords that help agents identify relevant tasks.
---

# Your Skill Name

Instructions for the agent go here...
```

Optional frontmatter fields: `license` (default: MIT), `metadata` (author, version, etc.)

### 3. Follow the naming conventions

- **Directory name**: lowercase, hyphens only (e.g., `emails`)
- **Name field**: must match directory name exactly
- **Description**: 1-1024 characters, include trigger phrases

### 4. Structure your skill

```
skills/your-skill-name/
├── SKILL.md           # Required - main instructions
├── references/        # Optional - additional documentation
│   └── guide.md
├── scripts/           # Optional - executable code
│   └── helper.py
└── assets/            # Optional - templates, images, data
    └── template.json
```

### 5. Write effective instructions

- Keep `SKILL.md` under 500 lines
- Move detailed reference material to `references/`
- Include step-by-step instructions
- Add examples of inputs and outputs
- Cover common edge cases

## Improving Existing Skills

1. Read the existing skill thoroughly
2. Test your changes locally
3. Keep changes focused and minimal
4. Update the version in metadata if making significant changes

## Submitting Your Contribution

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-skill-name`)
3. Make your changes
4. Test locally with an AI agent
5. Submit a pull request using the appropriate template:
   - [New Skill](?template=new-skill.md)
   - [Skill Update](?template=skill-update.md)
   - [Documentation](?template=documentation.md)

## Skill Quality Checklist

- [ ] `name` matches directory name
- [ ] `description` clearly explains when to use the skill
- [ ] Instructions are clear and actionable
- [ ] No sensitive data or credentials
- [ ] Follows existing skill patterns in the repo

## Questions?

Open an issue if you have questions or need help with your contribution.

---

## `VERSIONS.md`

# Marketing Skills Versions

Current versions of all skills. Agents can compare against local versions to check for updates.

| Skill | Version | Last Updated |
|-------|---------|--------------|
| ab-testing | 2.0.0 | 2026-05-05 |
| ad-creative | 2.0.0 | 2026-05-05 |
| ai-seo | 2.1.0 | 2026-06-15 |
| analytics | 2.0.0 | 2026-05-05 |
| aso | 2.0.0 | 2026-05-05 |
| churn-prevention | 2.0.0 | 2026-05-05 |
| co-marketing | 2.0.0 | 2026-05-05 |
| cold-email | 2.0.0 | 2026-05-05 |
| community-marketing | 2.0.0 | 2026-05-05 |
| competitor-profiling | 2.0.0 | 2026-05-05 |
| competitors | 2.0.0 | 2026-05-05 |
| content-strategy | 2.0.0 | 2026-05-05 |
| copy-editing | 2.0.0 | 2026-05-05 |
| copywriting | 2.0.1 | 2026-06-16 |
| cro | 2.0.0 | 2026-05-05 |
| customer-research | 2.0.0 | 2026-05-05 |
| directory-submissions | 2.0.0 | 2026-05-05 |
| emails | 2.0.0 | 2026-05-05 |
| free-tools | 2.0.0 | 2026-05-05 |
| image | 2.0.1 | 2026-05-18 |
| launch | 2.0.1 | 2026-06-16 |
| lead-magnets | 2.0.0 | 2026-05-05 |
| marketing-ideas | 2.0.0 | 2026-05-05 |
| marketing-plan | 1.1.0 | 2026-05-29 |
| marketing-psychology | 2.0.0 | 2026-05-05 |
| offers | 1.0.0 | 2026-06-16 |
| onboarding | 2.0.0 | 2026-05-05 |
| ads | 2.0.1 | 2026-05-26 |
| paywalls | 2.0.0 | 2026-05-05 |
| popups | 2.0.0 | 2026-05-05 |
| pricing | 2.0.1 | 2026-06-16 |
| product-marketing | 2.0.0 | 2026-05-05 |
| programmatic-seo | 2.0.0 | 2026-05-05 |
| prospecting | 1.0.0 | 2026-05-26 |
| public-relations | 1.0.0 | 2026-06-10 |
| referrals | 2.0.0 | 2026-05-05 |
| revops | 2.0.0 | 2026-05-05 |
| sales-enablement | 2.0.1 | 2026-06-16 |
| schema | 2.0.0 | 2026-05-05 |
| seo-audit | 2.0.0 | 2026-05-05 |
| signup | 2.0.0 | 2026-05-05 |
| site-architecture | 2.0.0 | 2026-05-05 |
| sms | 1.0.0 | 2026-05-21 |
| social | 2.1.0 | 2026-06-10 |
| video | 2.0.1 | 2026-05-18 |

## Recent Changes

### 2.5.1 (2026-06-16)

- Bumped `copywriting`, `launch`, `pricing`, and `sales-enablement` from 2.0.0 → 2.0.1 to reflect the description changes that shipped in v2.5.0 (cross-references added pointing to the new `offers` skill). The skill bodies are unchanged; only the frontmatter description picked up a new "For ..., see offers" line. Without the version bump, the repo's update check (which compares VERSIONS.md against local skill metadata) would not surface the routing/discovery change to users with installed copies. Caught by codex review.

### 2.5.0 (2026-06-16)

- Added `offers` skill for offer design — the thing you actually sell, not the page that sells it. Built around two frameworks: (1) the Value Equation (Dream Outcome × Perceived Likelihood / Time Delay × Effort), originally Hormozi, now standard across direct-response and creator-economy training; and (2) the six-component anatomy of a complete offer (core deliverable, bonus stack, guarantee, scarcity, name, price + payment structure). Self-scoped explicitly: best for services, agency retainers, courses, coaching, info products, high-ticket B2B, and direct response. Less load-bearing for pure self-serve SaaS where `pricing` does more work. References include: `value-equation.md` (full breakdown of the four levers with diagnostic prompts and a worked example of a stuck $3K copywriting course), `offer-anatomy.md` (the six components with worked examples and a fractional-CMO before/after), `guarantee-design.md` (eight guarantee types with decision tree by business type, refund tolerance, and buyer sophistication; honest case for anti-guarantees on premium offers), `bonus-stacking.md` (bonuses-as-objection-handlers, the math of stated value, the 4-bonus pattern that works, common failure modes), `scarcity-urgency.md` (honest formats: capacity / cohort / founding-member / inventory / seasonal / bonus-expiry / price-increase; explicit rejection of fake countdown timers and manufactured FOMO; why fake scarcity is uniquely costly), `offer-formats.md` (default offer format by business type — service, course, coaching, info product, high-ticket B2B, agency retainer, self-serve SaaS, direct-response — with what to watch for each), and `examples.md` (six anonymized before/after worked examples spanning fractional CMO, copywriting course, Notion templates, B2B SaaS annual contract, group coaching mastermind, content agency retainer). Includes a banned-vocabulary list (game-changing, revolutionary, 10x, secret, hidden, "limited time" with no actual limit) and explicit anti-patterns (manipulative scarcity, over-promising guarantees, bonus inflation, course-bro aesthetic).
- Cross-references added in `pricing`, `copywriting`, `launch`, and `sales-enablement` descriptions pointing to `offers` for offer construction.
- Total skills: 45.

### 2.4.2 (2026-06-15)

- **ai-seo** (2.0.1 → 2.1.0): added coverage of Google's Open Knowledge Format (OKF), a v0.1 markdown spec for agent-readable site bundles introduced on the Google Cloud blog on 2026-06-12 and shipped inside Knowledge Catalog. New `references/okf.md` reference covers what OKF is (directory of cross-linked markdown files with YAML frontmatter — `type` required, plus `title`/`description`/`resource`/`tags`/`timestamp` recommended), honest framing (Google built it for data-team catalog metadata; site-readable repurposing popularized by Suganthan Mohanadasan is a clever secondary use), what it does for AI search today (nothing immediate; protocol-layer registration like early schema.org adoption), where OKF fits in the agent-readable stack alongside `sitemap.xml` / `robots.txt` / `llms.txt` / `/pricing.md` / schema, three ways to ship a bundle (Suganthan's free web generator, his pending WordPress plugin, or by hand), hosting guidance (`yoursite.com/okf/index.md` plus an `llms.txt` line pointing to it), when to skip (closed platforms like Wix/Squarespace, very small sites, sites without other machine-readable files), and what to watch (v1.0 spec, AI engine adoption signals). `SKILL.md` adds a brief OKF subsection under "Machine-Readable Files for AI Agents" pointing to the reference. Frontmatter description extended with new triggers: `llms.txt`, `OKF`, `Open Knowledge Format`, `knowledge bundle`, `agent-readable site`. `references/platform-ranking-factors.md` Google AI Overviews section gets an OKF callout framing it as a "register early" protocol bet rather than a confirmed ranking signal.

### 2.4.1 (2026-06-10)

- Renamed `pr` skill to `public-relations` to avoid collision with pull-request skills in other Claude Code plugins (common naming for code-review / GitHub PR automation). The skill description already disambiguated from pull requests, but the directory name `pr` was still ambiguous to skill resolvers and to users typing `/pr`. The rename happened within hours of the initial v2.4.0 publish, before meaningful install adoption. No content changes; skill version stays at 1.0.0. All cross-references in `social/SKILL.md`, `VERSIONS.md`, and `README.md` updated accordingly.

### 2.4.0 (2026-06-10)

- Added `public-relations` skill (originally shipped as `pr`, renamed in v2.4.1) for public relations / earned media work — pitching journalists, newsjacking trending stories, responding to press requests (HARO/Connectively, Qwoted, Featured, Help A B2B Writer), and building the owned-media foundation (press page + media kit). Four PR modes (reactive / proactive / inbound / owned), explicit when-to-skip framing, and a banned-vocabulary list. References include: `newsjacking.md` (detect → score → angle → pitch loop with newsworthiness scoring rubric, 7 angle templates, Google News / HN / Reddit curl recipes, failure modes); `journalist-pitching.md` (media list construction, journalist fit scoring, 6 pitch templates by angle — data story / exclusive launch / op-ed / customer story / trend connector / newsjack response — subject-line craft, embargo etiquette, follow-up cadence); `press-platforms.md` (daily triage workflow, response template, ROI reality check); `media-outlets.md` (tiered list of tech press, SaaS, AI, devtools, business outlets, newsletters, podcasts, vertical press, regional press — explicitly scoped to journalist-driven outlets, with startup directories deferred to `directory-submissions`). Scope is enforced via cross-references: the `public-relations` skill handles earned media; `directory-submissions` handles Product Hunt / BetaList / SaaS directories; `launch` handles the broader launch moment.
- **social** (2.0.0 → 2.1.0): added `references/listening.md` for engagement triage — a daily loop for surfacing the top posts to comment on rather than scrolling feeds. Includes a 5-dimension scoring rubric (ICP fit, intent signal, reach potential, comment opportunity, recency), comment quality tiers, curl-based recipes for Reddit / HN Algolia / Bluesky (no auth required), and a browser-driven workflow for LinkedIn and X via `dev-browser` with persistent session. Added `references/listening-sources-template.md` — a copyable starter for `.agents/listening-sources.md` covering brand/category context, ICP definition, target accounts per platform, intent keywords, subreddits, saved-search URLs, and a do-not-engage list. SKILL.md Engagement Strategy section now links to the listening reference.
- Total skills: 44.

### 2.3.0 (2026-05-27)

- Added `marketing-plan` skill — comprehensive AARRR-structured marketing plan generator. Produces a 13-section Notion-paste-ready plan document (executive summary, strategic frame, current state, AARRR breakdown, 90-day roadmap, 12-month outlook with funding-stage capability unlocks, marketing operations stack mapping skills + MCPs to AARRR stages, tactical idea bank cross-referencing all 139 `marketing-ideas` to AARRR + client-specific status, measurement framework, RACI, open decisions). Customized for current budget, team, stage, and tooling stack. Three-phase workflow: INIT (research + intake), REVIEW (section-by-section walkthrough), FINALIZE (compile + verify + optional publish to shared repo). References include methodology, plan-template, aarrr-framework, current-state-rubric (self-contained 17-section scoring rubric), ops-stack-mapping, idea-cross-reference (139-idea AARRR mapping), funding-stage-unlocks, measurement-framework, client-types (variations by B2B SaaS / D2C / hardware-hybrid / marketplace / dev tool / clinical / commerce), example-quietude (anonymized canonical reference plan, based on a real fCMO engagement with names/identifying details changed), budget-planning (two scientific methods for setting the marketing budget — Revenue-Based 5–40% of ARR, and Goal-Based formula reverse-engineered from the revenue target; plus blended CAC calculation, the 10–20% experimental buffer rule, the 3-3-2-2-2 VC growth path, and the forecasting reality check), growth-patterns (the real shape of SaaS growth — $0–10K / $10K–100K / $100K–1M phases with binding constraints, linear vs step-function vs S-curve patterns, and Channel × Product × Market layering), and team-and-agency-model (the strategy-in-house / execution-outsourced principle, three core functions Growth/Product/Content, π-shaped marketer framework, title progression Manager → Lead → Director → VP → Chief, agency selection framework, and the three-stage scaling model Early/Growth/Scale). Budget, growth-pattern, and team frameworks drawn from *Founding Marketing* by Corey Haines.
- Total skills: 43.

### 2.2.0 (2026-05-26)

- Added `prospecting` skill for building qualified prospect lists across SaaS, B2B, and local SMB motions. Includes shared 5-phase framework (ICP → discovery → qualify → score → output) plus branch-specific references (saas-prospecting, b2b-prospecting, local-prospecting), data-sources guide covering Apollo / Clay / ZoomInfo / Clearbit / Hunter / Snov / Truelist / RB2B / Sales Nav / BuiltWith / Crunchbase / GitHub, and compliance reference (CAN-SPAM, GDPR, CASL, platform ToS).
- Added `tools/clis/github-prospects.js` CLI for pulling GitHub stargazers, forkers, and watchers as a developer-intent signal — with pagination, enrichment, filter-based early termination, and CSV output.
- Added new tool integration docs: `truelist` (email deliverability validation, OpenAPI-aligned), `github` (REST API for prospecting), `firecrawl` (single-target page scraping), `browserbase` (real Chromium for JS-heavy pages or interaction).
- **ads** (2.0.0 → 2.0.1): added Google RSA Output Spec section enforcing 15 headlines × 30 chars, 4 descriptions × 90 chars, ad group structure labels, ≥8 negative keywords, ≥4 sitelinks/callouts, output ordering to avoid truncation, and a self-check before responding. Includes optional Brazilian medical (CFM) compliance rules when product context indicates that vertical.
- Added `sequenzy` tool integration (email marketing platform with MCP support).
- Fixed plugin.json version drift (was stuck at 1.9.0 across three releases) — `sync-skills.js` now auto-syncs `plugin.json` version to `marketplace.json` on every change. Closes #323.
- Added skill install artifacts (`.agents/`, `.claude/`, `skills-lock.json`) to `.gitignore`.
- Total skills: 42.

### 2.1.0 (2026-05-21)
- Added `sms` skill for SMS/MMS marketing — welcome flows, abandoned cart, post-purchase, win-back, promotional sends, and transactional/auth. Includes compliance reference (TCPA, A2P 10DLC, GDPR, CASL), sequence templates with character counts, and platform comparison (Klaviyo, Postscript, Attentive, Twilio, Brevo, SimpleTexting, Customer.io).
- Total skills: 41

### 2.0.1 (2026-05-18)

Content patch — no breaking changes, no new skills.

- **ai-seo** (2.0.0 → 2.0.1): aligned with Google's official AI features optimization guide. Added sections for Google's stance on AI optimization, query fan-out, agentic experiences (including UCP), explicit "what NOT to do" (scaled content abuse, etc.), and Search Console expectations. Reframed llms.txt / pricing.md / schema markup recommendations as "Google says not required, helpful for non-Google AI engines." Moved content-type tactics to `references/content-types.md` (added local/ecom Merchant Center + Business Profile guidance per Google).
- **image** (2.0.0 → 2.0.1): refreshed model lineup to current May 2026 releases — Nano Banana / Nano Banana Pro family naming, Flux Pro 1.1 + Kontext + Dev + Schnell variants, Ideogram 3.0, ChatGPT Images 2.0 / GPT Image, Midjourney v7, Recraft V3, SD 3.5 / SDXL. Updated decision tree and trigger phrases.
- **video** (2.0.0 → 2.0.1): refreshed model lineup — Sora 2 promoted from limited-availability caveat, Kling 2.5/3.0, added Seedance (ByteDance), Hailuo / MiniMax (character consistency), Hunyuan Video / Wan 2 (open-weight self-hosted), Pika 2.x. New "Quick picks" guide.

Total skills: 40 (unchanged).

### 2.0.0 (2026-05-05)

**Breaking changes** — Users must reinstall skills after this update.

#### Skill Renames (17)
| Old Name | New Name |
|----------|----------|
| ab-test-setup | ab-testing |
| analytics-tracking | analytics |
| aso-audit | aso |
| competitor-alternatives | competitors |
| email-sequence | emails |
| free-tool-strategy | free-tools |
| launch-strategy | launch |
| onboarding-cro | onboarding |
| paid-ads | ads |
| paywall-upgrade-cro | paywalls |
| popup-cro | popups |
| pricing-strategy | pricing |
| product-marketing-context | product-marketing |
| referral-program | referrals |
| schema-markup | schema |
| signup-flow-cro | signup |
| social-content | social |

#### Consolidations (1)
- `page-cro` + `form-cro` → `cro` (form content moved to `references/form.md`)

#### Why 2.0?
- Shorter, cleaner skill names
- Consistent naming conventions (no more `-strategy`, `-setup`, `-cro` suffixes)
- Consolidated CRO into single skill with references
- All cross-references updated across 100+ files

**Total skills: 40**

### 1.10.0 (2026-05-04)
- Added `co-marketing` skill for partner identification, joint campaigns, and co-marketing strategy
- Total skills: 41

### 2026-04-24
- Added `image` skill for AI image generation, design tools, profile/listing banners, and optimization
- Added `video` skill for AI video production (Hyperframes, HeyGen, Veo, Runway, Kling)
- Added short-form video section to `social` (1.3.0) — TikTok, Reels, Shorts frameworks
- Added HeyGen and Hyperframes tool integration guides
- Fixed plugin marketplace: `source` field now passes Claude Code schema validation (#270)
- Added proper `plugin.json` manifest with `"skills": "./skills"`
- Total skills: 40

### 2026-04-21
- Added `directory-submissions` skill for Product Hunt, G2, AI directories, and backlink strategy
- Added `competitor-profiling` skill for competitive intelligence research
- Added international SEO & localization section to `seo-audit` (1.2.0)
- Added conversion tracking reference to `ads` (cross-platform pixel setup)
- Added Zapier SDK integration for 8,000+ app access
- Fixed plugin loading: removed `./` prefix from marketplace.json skill paths (#243)
- Hardened CLI tools: Supermetrics API key moved to header, ZoomInfo JWT masked by default
- Fixed community-marketing YAML frontmatter (#240)
- Fixed Zapier webhook URL validation (#247)
- Added missing skills to VERSIONS.md (aso, community-marketing, customer-research — shipped in prior releases)
- Total skills: 38

### 2026-03-14
- Added `lead-magnets` skill for lead magnet strategy, format selection, and conversion optimization
- Added Composio integration layer for MCP access to OAuth-heavy tools (HubSpot, Salesforce, Meta Ads, LinkedIn Ads, Google Sheets, Slack, Notion, etc.)
- Added headless CMS integration guides (Sanity, Contentful, Strapi) with headless-cms reference
- Added 197 evals across all 33 skills for automated quality testing
- Optimized all 32 skill descriptions for better trigger phrase matching
- Replaced rigid imperatives with reasoning-based guidance across all skills
- Added 10 new CLI tools (airops, clay, close, coupler, crossbeam, outreach, pendo, similarweb, supermetrics, zoominfo)
- Added 13 new integration guides
- Bumped all 32 existing skills from 1.1.0 → 1.2.0

### 2026-02-27
- Migrated context path from `.claude/` to `.agents/` for agent-agnostic compatibility
- All skills now check `.agents/product-marketing.md` first, with `.claude/` fallback for older setups
- Updated install paths in README to reference `.agents/skills/`
- Bumped all 32 skills from 1.0.0 → 1.1.0

### 2026-02-22
- Added `revops` skill for revenue operations, lead lifecycle, scoring, routing, pipeline management, and CRM automation
- Added `sales-enablement` skill for sales decks, one-pagers, objection handling, demo scripts, and sales playbooks

### 2026-02-21
- Added `site-architecture` skill for website structure planning, page hierarchy, navigation design, URL structure, and internal linking strategy

### 2026-02-18
- Added `ai-seo` skill for AI search optimization (AEO, GEO, LLMO, AI Overviews)
- Moved AEO/GEO content patterns from `seo-audit` references to `ai-seo` skill
- Added `churn-prevention` skill for cancel flows, save offers, dunning, and payment recovery

### 2026-02-17
- Added `ad-creative` skill for bulk ad creative generation and performance-based iteration
- Added 51 zero-dependency CLI tools for marketing platforms (`tools/clis/`)
- Added 31 new integration guides (`tools/integrations/`)
- Added 4 email outreach CLIs: hunter, snov, lemlist, instantly
- Security hardening: header auth for meta-ads, URL encoding, input validation
- All CLIs reviewed via independent codex audit (auth, security, error handling, consistency)

### 2026-01-27
- Initial version tracking added
- Added tools registry with 29 integration guides

---

## `tools/REGISTRY.md`

# Marketing Tools Registry

Quick reference for AI agents to discover tool capabilities and integration methods.

## How to Use This Registry

1. **Find tools by category** - Browse sections below for tools in each domain
2. **Check integration methods** - See what APIs, MCPs, CLIs, or SDKs are available
3. **Read integration guides** - Detailed setup and common operations in `integrations/`

---

## Tool Index

| Tool | Category | API | MCP | CLI | SDK | Guide |
|------|----------|:---:|:---:|:---:|:---:|-------|
| ga4 | Analytics | ✓ | ✓ | [✓](clis/ga4.js) | ✓ | [ga4.md](integrations/ga4.md) |
| mixpanel | Analytics | ✓ | - | [✓](clis/mixpanel.js) | ✓ | [mixpanel.md](integrations/mixpanel.md) |
| amplitude | Analytics | ✓ | - | [✓](clis/amplitude.js) | ✓ | [amplitude.md](integrations/amplitude.md) |
| posthog | Analytics | ✓ | - | ✓ | ✓ | [posthog.md](integrations/posthog.md) |
| segment | Analytics | ✓ | - | [✓](clis/segment.js) | ✓ | [segment.md](integrations/segment.md) |
| adobe-analytics | Analytics | ✓ | - | [✓](clis/adobe-analytics.js) | ✓ | [adobe-analytics.md](integrations/adobe-analytics.md) |
| plausible | Analytics | ✓ | - | [✓](clis/plausible.js) | - | [plausible.md](integrations/plausible.md) |
| google-search-console | SEO | ✓ | - | [✓](clis/google-search-console.js) | ✓ | [google-search-console.md](integrations/google-search-console.md) |
| semrush | SEO | ✓ | - | [✓](clis/semrush.js) | - | [semrush.md](integrations/semrush.md) |
| ahrefs | SEO | ✓ | - | [✓](clis/ahrefs.js) | - | [ahrefs.md](integrations/ahrefs.md) |
| dataforseo | SEO | ✓ | - | [✓](clis/dataforseo.js) | ✓ | [dataforseo.md](integrations/dataforseo.md) |
| keywords-everywhere | SEO | ✓ | - | [✓](clis/keywords-everywhere.js) | - | [keywords-everywhere.md](integrations/keywords-everywhere.md) |
| rankparse | SEO | ✓ | ✓ | [✓](clis/rankparse.js) | - | [rankparse.md](integrations/rankparse.md) |
| clearbit | Data Enrichment | ✓ | - | [✓](clis/clearbit.js) | ✓ | [clearbit.md](integrations/clearbit.md) |
| apollo | Data Enrichment | ✓ | - | [✓](clis/apollo.js) | - | [apollo.md](integrations/apollo.md) |
| zoominfo | Data Enrichment | ✓ | ✓ | [✓](clis/zoominfo.js) | - | [zoominfo.md](integrations/zoominfo.md) |
| clay | Data Enrichment | ✓ | ✓ | [✓](clis/clay.js) | - | [clay.md](integrations/clay.md) |
| supermetrics | Data Aggregation | ✓ | ✓ | [✓](clis/supermetrics.js) | - | [supermetrics.md](integrations/supermetrics.md) |
| coupler | Data Aggregation | ✓ | ✓ | [✓](clis/coupler.js) | - | [coupler.md](integrations/coupler.md) |
| hubspot | CRM | ✓ | - | ✓ | ✓ | [hubspot.md](integrations/hubspot.md) |
| salesforce | CRM | ✓ | - | ✓ | ✓ | [salesforce.md](integrations/salesforce.md) |
| close | CRM | ✓ | - | [✓](clis/close.js) | - | [close.md](integrations/close.md) |
| stripe | Payments | ✓ | ✓ | ✓ | ✓ | [stripe.md](integrations/stripe.md) |
| paddle | Payments | ✓ | - | [✓](clis/paddle.js) | ✓ | [paddle.md](integrations/paddle.md) |
| rewardful | Referral | ✓ | - | [✓](clis/rewardful.js) | - | [rewardful.md](integrations/rewardful.md) |
| tolt | Referral | ✓ | - | [✓](clis/tolt.js) | - | [tolt.md](integrations/tolt.md) |
| dub-co | Links | ✓ | - | [✓](clis/dub.js) | ✓ | [dub-co.md](integrations/dub-co.md) |
| mention-me | Referral | ✓ | - | [✓](clis/mention-me.js) | - | [mention-me.md](integrations/mention-me.md) |
| partnerstack | Affiliate | ✓ | - | [✓](clis/partnerstack.js) | - | [partnerstack.md](integrations/partnerstack.md) |
| mailchimp | Email | ✓ | ✓ | [✓](clis/mailchimp.js) | ✓ | [mailchimp.md](integrations/mailchimp.md) |
| customer-io | Email | ✓ | - | [✓](clis/customer-io.js) | ✓ | [customer-io.md](integrations/customer-io.md) |
| sendgrid | Email | ✓ | - | [✓](clis/sendgrid.js) | ✓ | [sendgrid.md](integrations/sendgrid.md) |
| resend | Email | ✓ | ✓ | [✓](clis/resend.js) | ✓ | [resend.md](integrations/resend.md) |
| sequenzy | Email | ✓ | ✓ | ✓ | - | [sequenzy.md](integrations/sequenzy.md) |
| nitrosend | Email | ✓ | ✓ | - | - | [nitrosend.md](integrations/nitrosend.md) |
| kit | Email | ✓ | - | [✓](clis/kit.js) | ✓ | [kit.md](integrations/kit.md) |
| beehiiv | Newsletter | ✓ | - | [✓](clis/beehiiv.js) | - | [beehiiv.md](integrations/beehiiv.md) |
| klaviyo | Email/SMS | ✓ | - | [✓](clis/klaviyo.js) | ✓ | [klaviyo.md](integrations/klaviyo.md) |
| postmark | Email | ✓ | - | [✓](clis/postmark.js) | ✓ | [postmark.md](integrations/postmark.md) |
| brevo | Email/SMS | ✓ | - | [✓](clis/brevo.js) | ✓ | [brevo.md](integrations/brevo.md) |
| activecampaign | Email/CRM | ✓ | - | [✓](clis/activecampaign.js) | ✓ | [activecampaign.md](integrations/activecampaign.md) |
| twilio | SMS/Voice | ✓ | - | ✓ | ✓ | [twilio.md](integrations/twilio.md) |
| plivo | SMS/Voice | ✓ | - | - | ✓ | [plivo.md](integrations/plivo.md) |
| postscript | SMS | ✓ | - | - | - | [postscript.md](integrations/postscript.md) |
| attentive | SMS | ✓ | - | - | - | [attentive.md](integrations/attentive.md) |
| audiencetap | SMS/Email | ✓ | - | - | - | [audiencetap.md](integrations/audiencetap.md) |
| hunter | Email Outreach | ✓ | - | [✓](clis/hunter.js) | - | [hunter.md](integrations/hunter.md) |
| snov | Email Outreach | ✓ | - | [✓](clis/snov.js) | - | [snov.md](integrations/snov.md) |
| truelist | Email Verification | ✓ | ✓ | - | ✓ | [truelist.md](integrations/truelist.md) |
| github | Developer Intent | ✓ | - | [✓](clis/github-prospects.js) | ✓ | [github.md](integrations/github.md) |
| firecrawl | Site Scraping | ✓ | ✓ | - | ✓ | [firecrawl.md](integrations/firecrawl.md) |
| browserbase | Site Scraping | ✓ | ✓ | - | ✓ | [browserbase.md](integrations/browserbase.md) |
| lemlist | Email Outreach | ✓ | - | [✓](clis/lemlist.js) | - | [lemlist.md](integrations/lemlist.md) |
| instantly | Email Outreach | ✓ | - | [✓](clis/instantly.js) | - | [instantly.md](integrations/instantly.md) |
| google-ads | Ads | ✓ | ✓ | [✓](clis/google-ads.js) | ✓ | [google-ads.md](integrations/google-ads.md) |
| meta-ads | Ads | ✓ | - | [✓](clis/meta-ads.js) | ✓ | [meta-ads.md](integrations/meta-ads.md) |
| linkedin-ads | Ads | ✓ | - | [✓](clis/linkedin-ads.js) | - | [linkedin-ads.md](integrations/linkedin-ads.md) |
| tiktok-ads | Ads | ✓ | - | [✓](clis/tiktok-ads.js) | ✓ | [tiktok-ads.md](integrations/tiktok-ads.md) |
| zapier | Automation | ✓ | ✓ | [✓](clis/zapier.js) | ✓ | [zapier.md](integrations/zapier.md) |
| hotjar | CRO | ✓ | - | [✓](clis/hotjar.js) | - | [hotjar.md](integrations/hotjar.md) |
| optimizely | A/B Testing | ✓ | - | [✓](clis/optimizely.js) | ✓ | [optimizely.md](integrations/optimizely.md) |
| calendly | Scheduling | ✓ | - | [✓](clis/calendly.js) | - | [calendly.md](integrations/calendly.md) |
| savvycal | Scheduling | ✓ | - | [✓](clis/savvycal.js) | - | [savvycal.md](integrations/savvycal.md) |
| typeform | Forms | ✓ | - | [✓](clis/typeform.js) | ✓ | [typeform.md](integrations/typeform.md) |
| intercom | Messaging | ✓ | - | [✓](clis/intercom.js) | ✓ | [intercom.md](integrations/intercom.md) |
| outreach | Sales Engagement | ✓ | ✓ | [✓](clis/outreach.js) | - | [outreach.md](integrations/outreach.md) |
| crossbeam | Partner Ecosystem | ✓ | ✓ | [✓](clis/crossbeam.js) | - | [crossbeam.md](integrations/crossbeam.md) |
| introw | Partner Ecosystem | - | ✓ | - | - | [introw.md](integrations/introw.md) |
| pendo | Product Analytics | ✓ | - | [✓](clis/pendo.js) | - | [pendo.md](integrations/pendo.md) |
| similarweb | Competitive Intelligence | ✓ | - | [✓](clis/similarweb.js) | - | [similarweb.md](integrations/similarweb.md) |
| exa | AI Search | ✓ | ✓ | [✓](clis/exa.js) | ✓ | [exa.md](integrations/exa.md) |
| firehose | Competitive Intelligence | ✓ | - | - | - | [firehose.md](integrations/firehose.md) |
| sparktoro | Audience Research | - | - | - | - | [sparktoro.md](integrations/sparktoro.md) |
| rb2b | Visitor Identification | ✓ | - | - | - | [rb2b.md](integrations/rb2b.md) |
| gong | Revenue Intelligence | ✓ | - | - | - | [gong.md](integrations/gong.md) |
| airops | AI Content | ✓ | - | [✓](clis/airops.js) | - | [airops.md](integrations/airops.md) |
| buffer | Social | ✓ | - | [✓](clis/buffer.js) | - | [buffer.md](integrations/buffer.md) |
| wistia | Video | ✓ | - | [✓](clis/wistia.js) | - | [wistia.md](integrations/wistia.md) |
| heygen | Video | ✓ | ✓ | - | ✓ | [heygen.md](integrations/heygen.md) |
| hyperframes | Video | - | - | ✓ | ✓ | [hyperframes.md](integrations/hyperframes.md) |
| trustpilot | Reviews | ✓ | - | [✓](clis/trustpilot.js) | - | [trustpilot.md](integrations/trustpilot.md) |
| g2 | Reviews | ✓ | - | [✓](clis/g2.js) | - | [g2.md](integrations/g2.md) |
| onesignal | Push | ✓ | - | [✓](clis/onesignal.js) | ✓ | [onesignal.md](integrations/onesignal.md) |
| demio | Webinar | ✓ | - | [✓](clis/demio.js) | - | [demio.md](integrations/demio.md) |
| livestorm | Webinar | ✓ | - | [✓](clis/livestorm.js) | - | [livestorm.md](integrations/livestorm.md) |
| shopify | Commerce | ✓ | - | ✓ | ✓ | [shopify.md](integrations/shopify.md) |
| wordpress | CMS | ✓ | - | ✓ | ✓ | [wordpress.md](integrations/wordpress.md) |
| webflow | CMS | ✓ | - | ✓ | ✓ | [webflow.md](integrations/webflow.md) |
| sanity | Headless CMS | ✓ | - | ✓ | ✓ | [sanity.md](integrations/sanity.md) |
| contentful | Headless CMS | ✓ | - | ✓ | ✓ | [contentful.md](integrations/contentful.md) |
| strapi | Headless CMS | ✓ | - | ✓ | ✓ | [strapi.md](integrations/strapi.md) |
| composio | Integration Layer | ✓ | ✓ | ✓ | ✓ | [composio.md](integrations/composio.md) |
| cogny | Integration Layer | - | ✓ | - | - | [cogny.md](integrations/cogny.md) |

---

## By Category

### Analytics

Track user behavior, measure conversions, and analyze marketing performance.

| Tool | Best For | MCP Available |
|------|----------|:-------------:|
| **ga4** | Web analytics, Google ecosystem | ✓ |
| **mixpanel** | Product analytics, event tracking | - |
| **amplitude** | Product analytics, cohort analysis | - |
| **posthog** | Open-source analytics, session replay | - |
| **segment** | Customer data platform, routing | - |
| **adobe-analytics** | Enterprise analytics | - |
| **plausible** | Privacy-focused analytics | - |

**Agent recommendation**: Start with GA4 if using Google ecosystem. Use Mixpanel or Amplitude for deeper product analytics. Plausible for privacy-focused sites.

### SEO

Search engine optimization tools for keyword research, rank tracking, and site audits.

| Tool | Best For | Notes |
|------|----------|-------|
| **google-search-console** | Free, authoritative search data | Direct from Google |
| **semrush** | Competitive analysis, keyword research | Comprehensive |
| **ahrefs** | Backlink analysis, content research | Best for links |
| **dataforseo** | SERP tracking, backlinks, on-page audits | Comprehensive API |
| **keywords-everywhere** | Quick keyword research, traffic estimates | Credit-based |
| **rankparse** | Cheap, agent-friendly backlinks + domain data | Credit-based, MCP available |

**Agent recommendation**: Google Search Console is essential (free). Add Semrush or Ahrefs for competitive research. DataForSEO for programmatic SERP data. Keywords Everywhere for quick keyword lookups. RankParse for agent workflows where per-call cost matters — backlinks, domain authority, and tech stack at a fraction of enterprise pricing.

### CRM

Customer relationship management and sales tools.

| Tool | Best For | CLI Available |
|------|----------|:-------------:|
| **hubspot** | SMB, marketing + sales alignment | ✓ |
| **salesforce** | Enterprise, complex sales processes | ✓ |
| **close** | SMB, high-velocity sales | [✓](clis/close.js) |

**Agent recommendation**: HubSpot for startups/SMBs. Close for high-velocity inside sales. Salesforce for enterprise.

### Payments

Payment processing and subscription management.

| Tool | Best For | MCP Available |
|------|----------|:-------------:|
| **stripe** | SaaS subscriptions, developer-friendly | ✓ |
| **paddle** | SaaS billing with tax handling | - |

**Agent recommendation**: Stripe is the default for SaaS. Paddle for built-in tax compliance.

### Referral & Affiliate

Tools for referral programs, affiliate tracking, and partner management.

| Tool | Best For | Stripe Integration |
|------|----------|:------------------:|
| **rewardful** | Stripe-native affiliate programs | ✓ |
| **tolt** | SaaS affiliate programs | ✓ |
| **mention-me** | Enterprise referral programs | ✓ |
| **dub-co** | Link tracking, attribution | - |
| **partnerstack** | Enterprise partner programs | ✓ |

**Agent recommendation**: Rewardful or Tolt for Stripe-based SaaS. PartnerStack for enterprise partner programs. Dub.co for link attribution.

### Email

Email marketing, transactional email, and automation platforms.

| Tool | Best For | MCP Available |
|------|----------|:-------------:|
| **mailchimp** | SMB email marketing | ✓ |
| **customer-io** | Behavior-based messaging | - |
| **sendgrid** | Transactional email at scale | - |
| **resend** | Developer-friendly transactional | ✓ |
| **sequenzy** | Lifecycle email, sequences, transactional email | ✓ |
| **kit** | Creator/newsletter focused | - |
| **beehiiv** | Newsletter platform | - |
| **klaviyo** | E-commerce email + SMS | - |
| **postmark** | Deliverability-focused transactional | - |
| **brevo** | Email + SMS, popular in EU | - |
| **activecampaign** | Email automation + CRM | - |

**Agent recommendation**: Resend for transactional (dev-friendly). Sequenzy for lifecycle email, sequences, and agent-driven email marketing. Postmark for deliverability. Customer.io for advanced automation. Kit for creators. Beehiiv for newsletters. Klaviyo for e-commerce email/SMS. ActiveCampaign for email + CRM combo.

### SMS / Messaging

SMS and MMS marketing platforms and programmable messaging APIs.

| Tool | Best For | MCP Available |
|------|----------|:-------------:|
| **klaviyo** | DTC ecom already on Klaviyo email | - |
| **postscript** | Shopify DTC, SMS-first depth | - |
| **attentive** | Mid-market+ DTC, full-service | - |
| **twilio** | Custom API builds, transactional, dev-first | - |
| **plivo** | Twilio alternative, lower per-send cost | - |
| **audiencetap** | DTC with AI-forward creative + on-pack QR opt-in | - |
| **brevo** | EU SMB email + SMS combo | - |
| **customer-io** | Behavior-based SMS automation | - |

**Agent recommendation**: Klaviyo SMS for ecom already on Klaviyo email. Postscript for Shopify-first depth. Attentive for mid-market+ wanting concierge support. Twilio (or Plivo for lower cost) for custom builds and transactional/auth. AudienceTap when AI creative or on-pack QR opt-in matters.

### Advertising

Paid advertising platforms and campaign management.

| Tool | Best For | MCP Available |
|------|----------|:-------------:|
| **google-ads** | Search intent, high-intent traffic | ✓ |
| **meta-ads** | Demand gen, visual products, B2C | - |
| **linkedin-ads** | B2B, job title targeting | - |
| **tiktok-ads** | Younger demographics, video | - |

**Agent recommendation**: Google Ads for search intent. Meta for demand generation. LinkedIn for B2B.

### Automation

Workflow automation and integration platforms.

| Tool | Best For | MCP Available |
|------|----------|:-------------:|
| **zapier** | No-code integrations + SDK for 8,000+ apps | ✓ |

**Agent recommendation**: Zapier SDK for agents that need to interact with any app directly. Zaps for always-on automations.

### CRO & A/B Testing

Conversion rate optimization, heatmaps, and experimentation.

| Tool | Best For | Notes |
|------|----------|-------|
| **hotjar** | Heatmaps, recordings, surveys | Visual behavior data |
| **optimizely** | A/B testing, feature flags | Enterprise experimentation |

**Agent recommendation**: Hotjar for understanding user behavior. Optimizely for running experiments.

### Scheduling

Booking and appointment scheduling tools.

| Tool | Best For | Notes |
|------|----------|-------|
| **calendly** | Meeting scheduling, lead gen | Most popular |
| **savvycal** | Personalized scheduling | Developer-friendly |

**Agent recommendation**: Calendly for general use. SavvyCal for personalized booking experiences.

### Forms & Surveys

Form builders and survey platforms.

| Tool | Best For | Notes |
|------|----------|-------|
| **typeform** | Interactive forms, surveys | Conversational UX |

**Agent recommendation**: Typeform for engaging forms and surveys.

### Messaging

In-app messaging, chat, and customer communication.

| Tool | Best For | Notes |
|------|----------|-------|
| **intercom** | In-app messaging, support, product tours | Full customer platform |

**Agent recommendation**: Intercom for in-app messaging and customer support.

### Social Media

Social media scheduling, management, and analytics.

| Tool | Best For | Notes |
|------|----------|-------|
| **buffer** | Social scheduling, analytics | Multi-platform |

**Agent recommendation**: Buffer for scheduling and analytics across social platforms.

### Video

Video hosting, creation, and AI generation.

| Tool | Best For | Notes |
|------|----------|-------|
| **wistia** | Video hosting, marketing analytics | Best for marketing video hosting |
| **heygen** | AI avatars, talking-head videos | MCP server available |
| **hyperframes** | Programmatic video from HTML/CSS | Open source, agent-native |

**Agent recommendation**: HeyGen for AI avatar videos (MCP-enabled). Hyperframes for templated, data-driven video from code. Wistia for hosting and analytics.

### Data Enrichment

Company and person data enrichment for sales and marketing.

| Tool | Best For | Notes |
|------|----------|-------|
| **clearbit** | Company/person enrichment | Now HubSpot Breeze |
| **apollo** | B2B prospecting, email finding | Large database |
| **zoominfo** | B2B contacts, intent data | Enterprise-grade |
| **clay** | Waterfall enrichment, outbound | 75+ data providers |

**Agent recommendation**: Clearbit for enrichment. Apollo for prospecting and outbound. ZoomInfo for enterprise B2B data with intent signals. Clay for waterfall enrichment across multiple providers.

### Email Verification

Pre-outreach email deliverability validation.

| Tool | Best For | Notes |
|------|----------|-------|
| **truelist** | Bulk + single email deliverability validation | Returns `email_state` (ok / email_invalid / risky / unknown / accept_all) + `email_sub_state`. MCP server + 7-language SDKs available. |

**Agent recommendation**: Truelist for any prospect list before outreach — Apollo/ZoomInfo/Hunter data accuracy is typically 60–80%, validation is non-negotiable to keep sender reputation healthy.

### Developer Intent / GitHub

Discovery channel for dev-tool SaaS prospecting via GitHub stargazers, forkers, and watchers.

| Tool | Best For | Notes |
|------|----------|-------|
| **github** | Stargazers / forks / watchers of competitor or adjacent repos | Public API; pair with Apollo/Clay/Hunter for email enrichment |

**Agent recommendation**: Use `github-prospects.js` CLI to pull stargazers/forks of 3–5 anchor repos (competitors, category leaders, complementary tools). Filter to users with `company` field set, then enrich missing emails via Apollo or Hunter, then validate via Truelist before outreach.

### Site Scraping (single-target only)

Programmatic page extraction for **individual public business sites** — not for the platforms hosting prospects (Google Maps, LinkedIn, Yelp, Apollo, etc.).

| Tool | Best For | Notes |
|------|----------|-------|
| **firecrawl** | Page → clean markdown / structured extraction | API + MCP; lower overhead for "just give me the content" |
| **browserbase** | Real Chromium when rendering, interaction, or session state is required | API + MCP (Stagehand); use when Firecrawl can't handle the page |

**Agent recommendation**: Default to Firecrawl for static-ish pages and structured extraction. Use Browserbase when the site requires JS rendering, form interaction, cookie consent, or auth — and when you want session recordings for debugging. **For both: discovery happens on platforms (manual browser); extraction happens on the prospect's own website URL.** Don't point either tool at LinkedIn, Google Maps, Yelp, or similar.

### Reviews

Review management and social proof platforms.

| Tool | Best For | Notes |
|------|----------|-------|
| **trustpilot** | Consumer business reviews | Most recognized |
| **g2** | Software/B2B reviews | Best for SaaS |

**Agent recommendation**: Trustpilot for consumer products. G2 for B2B software.

### Push Notifications

Push notification delivery platforms.

| Tool | Best For | Notes |
|------|----------|-------|
| **onesignal** | Multi-channel push notifications | Web + mobile |

**Agent recommendation**: OneSignal for web and mobile push notifications.

### Webinar

Webinar and virtual event platforms.

| Tool | Best For | Notes |
|------|----------|-------|
| **demio** | Marketing webinars | Simple, focused |
| **livestorm** | Video engagement, webinars | Full event platform |

**Agent recommendation**: Demio for marketing-focused webinars. Livestorm for full event engagement.

### Sales Engagement

Sales engagement and outreach automation platforms.

| Tool | Best For | Notes |
|------|----------|-------|
| **outreach** | Enterprise sales engagement | Sequences, tasks, analytics |

**Agent recommendation**: Outreach for enterprise sales teams managing multi-touch sequences at scale.

### Product Analytics

Product analytics, feature adoption tracking, and in-app guidance.

| Tool | Best For | Notes |
|------|----------|-------|
| **pendo** | Feature adoption, in-app guides | Product-led growth |

**Agent recommendation**: Pendo for tracking feature adoption and delivering targeted in-app guidance.

### Competitive Intelligence

Traffic analytics, competitor benchmarking, and market research.

| Tool | Best For | Notes |
|------|----------|-------|
| **similarweb** | Website traffic, competitor analysis | Traffic sources, keywords |

**Agent recommendation**: Similarweb for competitor traffic analysis and market benchmarking.

### Audience Research

Audience intelligence and behavioral research tools.

| Tool | Best For | Notes |
|------|----------|-------|
| **sparktoro** | Audience affinities, behavioral data | Clickstream + social data |

**Agent recommendation**: SparkToro for discovering where your ICP spends time — what they read, watch, listen to, follow, and search for. Essential for customer research, content strategy, and media buying decisions.

### Visitor Identification

Website visitor de-anonymization for B2B sales and marketing.

| Tool | Best For | Notes |
|------|----------|-------|
| **rb2b** | Person-level visitor ID, intent signals | LinkedIn profiles, emails, page-level data |

**Agent recommendation**: RB2B for identifying anonymous B2B website visitors and routing high-intent visitors to outreach tools. Pairs well with Clay for enrichment and Instantly/Lemlist for cold email.

### Revenue Intelligence

Sales conversation analytics, call recording, and deal intelligence.

| Tool | Best For | Notes |
|------|----------|-------|
| **gong** | Call recording, transcript analysis, deal insights | REST API, 10k API calls/day |

**Agent recommendation**: Gong for mining sales call transcripts for customer research, competitive intelligence, and coaching insights. Essential for revenue attribution and win/loss analysis.

### AI Content

AI-powered content generation and optimization platforms.

| Tool | Best For | Notes |
|------|----------|-------|
| **airops** | AI content workflows, SEO content | Flow-based automation |

**Agent recommendation**: AirOps for building AI content workflows that generate SEO-optimized content at scale.

### AI Search

AI-powered web search APIs built for LLMs and agents. Return structured results with on-demand text, highlights, and summaries.

| Tool | Best For | Notes |
|------|----------|-------|
| **exa** | Neural/semantic web search, content research, competitor discovery | Search + findSimilar + Contents; MCP and SDKs available |

**Agent recommendation**: Exa for neural search over the open web — content research, competitor/similar-page discovery, link prospecting, news monitoring, and audience research. Pairs well with seo-audit, content-strategy, and competitor-profiling skills.

### Partner Ecosystem

Partner data sharing, co-sell, and ecosystem management.

| Tool | Best For | Notes |
|------|----------|-------|
| **crossbeam** | Account overlaps, co-sell | Now part of Reveal |
| **introw** | Partner management, deal registration, QBRs | MCP-enabled PRM |

**Agent recommendation**: Crossbeam for identifying partner account overlaps and co-sell opportunities. Introw for full partner relationship management — partner pipeline, commissions, tasks, and automated business review prep.

### Email Outreach

Cold email outreach and email finding tools for link building and sales prospecting.

| Tool | Best For | Notes |
|------|----------|-------|
| **hunter** | Email finding, domain search | Largest email database |
| **snov** | Email finding, drip campaigns | Built-in sequences |
| **lemlist** | Cold email campaigns | Personalization features |
| **instantly** | Cold email at scale | Email warmup built-in |

**Agent recommendation**: Hunter for finding emails. Lemlist or Instantly for sending cold email campaigns. Snov for combined finding + outreach.

### Data Aggregation

Marketing data pipeline tools that connect multiple platforms for unified reporting.

| Tool | Best For | Notes |
|------|----------|-------|
| **supermetrics** | Cross-platform data pulling | 200+ connectors |
| **coupler** | Automated data flows to sheets/BI | Scheduled pipelines |

**Agent recommendation**: Supermetrics for pulling data from multiple marketing platforms into unified reports. Coupler.io for automated data flows to spreadsheets and BI tools.

### Commerce & CMS

E-commerce platforms and content management systems.

| Tool | Best For | CLI Available |
|------|----------|:-------------:|
| **shopify** | E-commerce, product sales | ✓ |
| **wordpress** | Blogs, content sites | ✓ |
| **webflow** | Design-focused marketing sites | ✓ |
| **sanity** | Headless CMS, structured content | ✓ |
| **contentful** | Enterprise headless CMS, multi-locale | ✓ |
| **strapi** | Open-source headless CMS, self-hosted | ✓ |

**Agent recommendation**: Shopify for e-commerce. Webflow for marketing sites. WordPress for blogs. For headless CMS: Sanity for developer-flexible content, Contentful for enterprise multi-locale, Strapi for self-hosted/budget-conscious. See [headless CMS guide](../skills/content-strategy/references/headless-cms.md) for selection criteria.

---

## CLI Tools

Zero-dependency, single-file Node.js CLIs for tools that don't ship their own. See [`clis/README.md`](clis/README.md) for install instructions and usage.

All CLIs follow a consistent pattern:
- **No dependencies** — Node 18+ only, uses native `fetch`
- **JSON output** — pipe to `jq`, save to file, or use in scripts
- **Env var auth** — set `{TOOL}_API_KEY` and go
- **Consistent commands** — `{tool} <resource> <action> [options]`

---

## MCP-Enabled Tools

These tools have Model Context Protocol servers available, enabling direct agent interaction:

- **ga4** - Google Analytics 4 data access
- **stripe** - Payment and subscription management
- **mailchimp** - Email campaign management
- **google-ads** - Ad campaign management
- **resend** - Transactional email sending
- **zapier** - Workflow automation + SDK for 8,000+ app integrations
- **zoominfo** - B2B contacts and intent data
- **clay** - Data enrichment and outbound automation
- **supermetrics** - Cross-platform marketing data
- **coupler** - Marketing data pipelines
- **outreach** - Sales engagement sequences
- **crossbeam** - Partner ecosystem data
- **introw** - Partner relationship management
- **exa** - AI-powered web search for LLMs and agents

To use MCP tools, ensure the appropriate MCP server is configured in your environment.

### Composio Integration

[Composio](integrations/composio.md) provides managed OAuth and pre-built connectors for 500+ tools via a single MCP server. It adds MCP access to tools that don't have native MCP servers, including HubSpot, Salesforce, Meta Ads, LinkedIn Ads, Google Sheets, Slack, Notion, and more.

- **Setup**: `npx @composio/mcp@latest setup`
- **Quick start**: See [tools/composio/README.md](composio/README.md)
- **Marketing tool mapping**: See [tools/composio/marketing-tools.md](composio/marketing-tools.md)

Use Composio when you need MCP access to OAuth-heavy tools. Prefer native MCP servers (GA4, Stripe, Mailchimp, etc.) when available — they have deeper coverage.

### Cogny Integration

[Cogny](integrations/cogny.md) is a hosted MCP gateway focused on marketing channels — one federated MCP URL with managed OAuth across every channel you've connected. Narrower than Composio (marketing-only) and useful when you want SEO, paid social, and privacy-friendly analytics behind a single MCP login.

- **Setup**: connect channels at [cogny.com](https://cogny.com), then in Claude.ai go to Settings → Connectors → Add custom connector and paste `https://app.cogny.com/mcp`
- **Channels**: Search Console, Bing Webmaster, Semrush, LinkedIn Ads, Reddit Ads, TikTok Ads, Plausible, Fathom
- **Pricing**: Solo plan starts at $9/mo (7-day trial)

Use Cogny when you only need marketing channels and want to avoid running your own OAuth proxy. Prefer native APIs when you need deep, custom control of a single tool.

---

## Quick Start by Use Case

### Setting up analytics tracking
1. Read [ga4.md](integrations/ga4.md) for web analytics
2. Read [segment.md](integrations/segment.md) if routing to multiple tools

### Launching a referral program
1. Read [rewardful.md](integrations/rewardful.md) or [tolt.md](integrations/tolt.md) for Stripe-based programs
2. Read [dub-co.md](integrations/dub-co.md) for link tracking

### Setting up email automation
1. Read [customer-io.md](integrations/customer-io.md) for behavior-based automation
2. Read [resend.md](integrations/resend.md) for transactional email

### Running email outreach for backlinks
1. Read [hunter.md](integrations/hunter.md) for finding emails
2. Read [lemlist.md](integrations/lemlist.md) or [instantly.md](integrations/instantly.md) for sending campaigns

### Running paid ads
1. Read [google-ads.md](integrations/google-ads.md) for search campaigns
2. Read [meta-ads.md](integrations/meta-ads.md) for social campaigns

---

## `.github/PULL_REQUEST_TEMPLATE/documentation.md`

## Documentation

## Summary

<!-- What documentation changes are you making? -->

## Files changed

<!-- List the files you're updating -->

## Checklist

- [ ] Links are valid
- [ ] Formatting is consistent with existing docs
- [ ] No sensitive data or credentials

---

## `.github/PULL_REQUEST_TEMPLATE/new-skill.md`

## New Skill

**Skill name:** `skills/SKILL-NAME`

## Summary

<!-- What does this skill do and when should it be used? -->

## Checklist

- [ ] `name` matches directory name exactly
- [ ] `name` follows naming rules (lowercase, hyphens, no `--`)
- [ ] `description` is 1-1024 chars with trigger phrases
- [ ] `SKILL.md` is under 500 lines
- [ ] No sensitive data or credentials
- [ ] Tested locally with AI agent

---

## `.github/PULL_REQUEST_TEMPLATE/skill-update.md`

## Skill Update

**Skill:** `skills/SKILL-NAME`

## Summary

<!-- What changes are you making and why? -->

## Type of update

- [ ] Bug fix
- [ ] Improved instructions
- [ ] Added references/scripts
- [ ] Other

## Checklist

- [ ] Changes are focused and minimal
- [ ] `SKILL.md` is still under 500 lines
- [ ] No sensitive data or credentials
- [ ] Tested locally with AI agent

---

## `skills/ab-testing/SKILL.md`

---
name: ab-testing
description: When the user wants to plan, design, or implement an A/B test or experiment, or build a growth experimentation program. Also use when the user mentions "A/B test," "split test," "experiment," "test this change," "variant copy," "multivariate test," "hypothesis," "should I test this," "which version is better," "test two versions," "statistical significance," "how long should I run this test," "growth experiments," "experiment velocity," "experiment backlog," "ICE score," "experimentation program," or "experiment playbook." Use this whenever someone is comparing two approaches and wants to measure which performs better, or when they want to build a systematic experimentation practice. For tracking implementation, see analytics. For page-level conversion optimization, see cro.
metadata:
  version: 2.0.0
---

# A/B Test Setup

You are an expert in experimentation and A/B testing. Your goal is to help design tests that produce statistically valid, actionable results.

## Initial Assessment

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Before designing a test, understand:

1. **Test Context** - What are you trying to improve? What change are you considering?
2. **Current State** - Baseline conversion rate? Current traffic volume?
3. **Constraints** - Technical complexity? Timeline? Tools available?

---

## Core Principles

### 1. Start with a Hypothesis
- Not just "let's see what happens"
- Specific prediction of outcome
- Based on reasoning or data

### 2. Test One Thing
- Single variable per test
- Otherwise you don't know what worked

### 3. Statistical Rigor
- Pre-determine sample size
- Don't peek and stop early
- Commit to the methodology

### 4. Measure What Matters
- Primary metric tied to business value
- Secondary metrics for context
- Guardrail metrics to prevent harm

---

## Hypothesis Framework

### Structure

```
Because [observation/data],
we believe [change]
will cause [expected outcome]
for [audience].
We'll know this is true when [metrics].
```

### Example

**Weak**: "Changing the button color might increase clicks."

**Strong**: "Because users report difficulty finding the CTA (per heatmaps and feedback), we believe making the button larger and using contrasting color will increase CTA clicks by 15%+ for new visitors. We'll measure click-through rate from page view to signup start."

---

## Test Types

| Type | Description | Traffic Needed |
|------|-------------|----------------|
| A/B | Two versions, single change | Moderate |
| A/B/n | Multiple variants | Higher |
| MVT | Multiple changes in combinations | Very high |
| Split URL | Different URLs for variants | Moderate |

---

## Sample Size

### Quick Reference

| Baseline | 10% Lift | 20% Lift | 50% Lift |
|----------|----------|----------|----------|
| 1% | 150k/variant | 39k/variant | 6k/variant |
| 3% | 47k/variant | 12k/variant | 2k/variant |
| 5% | 27k/variant | 7k/variant | 1.2k/variant |
| 10% | 12k/variant | 3k/variant | 550/variant |

**Calculators:**
- [Evan Miller's](https://www.evanmiller.org/ab-testing/sample-size.html)
- [Optimizely's](https://www.optimizely.com/sample-size-calculator/)

**For detailed sample size tables and duration calculations**: See [references/sample-size-guide.md](references/sample-size-guide.md)

---

## Metrics Selection

### Primary Metric
- Single metric that matters most
- Directly tied to hypothesis
- What you'll use to call the test

### Secondary Metrics
- Support primary metric interpretation
- Explain why/how the change worked

### Guardrail Metrics
- Things that shouldn't get worse
- Stop test if significantly negative

### Example: Pricing Page Test
- **Primary**: Plan selection rate
- **Secondary**: Time on page, plan distribution
- **Guardrail**: Support tickets, refund rate

---

## Designing Variants

### What to Vary

| Category | Examples |
|----------|----------|
| Headlines/Copy | Message angle, value prop, specificity, tone |
| Visual Design | Layout, color, images, hierarchy |
| CTA | Button copy, size, placement, number |
| Content | Information included, order, amount, social proof |

### Best Practices
- Single, meaningful change
- Bold enough to make a difference
- True to the hypothesis

---

## Traffic Allocation

| Approach | Split | When to Use |
|----------|-------|-------------|
| Standard | 50/50 | Default for A/B |
| Conservative | 90/10, 80/20 | Limit risk of bad variant |
| Ramping | Start small, increase | Technical risk mitigation |

**Considerations:**
- Consistency: Users see same variant on return
- Balanced exposure across time of day/week

---

## Implementation

### Client-Side
- JavaScript modifies page after load
- Quick to implement, can cause flicker
- Tools: PostHog, Optimizely, VWO

### Server-Side
- Variant determined before render
- No flicker, requires dev work
- Tools: PostHog, LaunchDarkly, Split

---

## Running the Test

### Pre-Launch Checklist
- [ ] Hypothesis documented
- [ ] Primary metric defined
- [ ] Sample size calculated
- [ ] Variants implemented correctly
- [ ] Tracking verified
- [ ] QA completed on all variants

### During the Test

**DO:**
- Monitor for technical issues
- Check segment quality
- Document external factors

**Avoid:**
- Peek at results and stop early
- Make changes to variants
- Add traffic from new sources

### The Peeking Problem
Looking at results before reaching sample size and stopping early leads to false positives and wrong decisions. Pre-commit to sample size and trust the process.

---

## Analyzing Results

### Statistical Significance
- 95% confidence = p-value < 0.05
- Means <5% chance result is random
- Not a guarantee—just a threshold

### Analysis Checklist

1. **Reach sample size?** If not, result is preliminary
2. **Statistically significant?** Check confidence intervals
3. **Effect size meaningful?** Compare to MDE, project impact
4. **Secondary metrics consistent?** Support the primary?
5. **Guardrail concerns?** Anything get worse?
6. **Segment differences?** Mobile vs. desktop? New vs. returning?

### Interpreting Results

| Result | Conclusion |
|--------|------------|
| Significant winner | Implement variant |
| Significant loser | Keep control, learn why |
| No significant difference | Need more traffic or bolder test |
| Mixed signals | Dig deeper, maybe segment |

---

## Documentation

Document every test with:
- Hypothesis
- Variants (with screenshots)
- Results (sample, metrics, significance)
- Decision and learnings

**For templates**: See [references/test-templates.md](references/test-templates.md)

---

## Growth Experimentation Program

Individual tests are valuable. A continuous experimentation program is a compounding asset. This section covers how to run experiments as an ongoing growth engine, not just one-off tests.

### The Experiment Loop

```
1. Generate hypotheses (from data, research, competitors, customer feedback)
2. Prioritize with ICE scoring
3. Design and run the test
4. Analyze results with statistical rigor
5. Promote winners to a playbook
6. Generate new hypotheses from learnings
→ Repeat
```

### Hypothesis Generation

Feed your experiment backlog from multiple sources:

| Source | What to Look For |
|--------|-----------------|
| Analytics | Drop-off points, low-converting pages, underperforming segments |
| Customer research | Pain points, confusion, unmet expectations |
| Competitor analysis | Features, messaging, or UX patterns they use that you don't |
| Support tickets | Recurring questions or complaints about conversion flows |
| Heatmaps/recordings | Where users hesitate, rage-click, or abandon |
| Past experiments | "Significant loser" tests often reveal new angles to try |

### ICE Prioritization

Score each hypothesis 1-10 on three dimensions:

| Dimension | Question |
|-----------|----------|
| **Impact** | If this works, how much will it move the primary metric? |
| **Confidence** | How sure are we this will work? (Based on data, not gut.) |
| **Ease** | How fast and cheap can we ship and measure this? |

**ICE Score** = (Impact + Confidence + Ease) / 3

Run highest-scoring experiments first. Re-score monthly as context changes.

### Experiment Velocity

Track your experimentation rate as a leading indicator of growth:

| Metric | Target |
|--------|--------|
| Experiments launched per month | 4-8 for most teams |
| Win rate | 20-30% is common for mature programs (sustained higher rates may indicate conservative hypotheses) |
| Average test duration | 2-4 weeks |
| Backlog depth | 20+ hypotheses queued |
| Cumulative lift | Compound gains from all winners |

### The Experiment Playbook

When a test wins, don't just implement it — document the pattern:

```
## [Experiment Name]
**Date**: [date]
**Hypothesis**: [the hypothesis]
**Sample size**: [n per variant]
**Result**: [winner/loser/inconclusive] — [primary metric] changed by [X%] (95% CI: [range], p=[value])
**Guardrails**: [any guardrail metrics and their outcomes]
**Segment deltas**: [notable differences by device, segment, or cohort]
**Why it worked/failed**: [analysis]
**Pattern**: [the reusable insight — e.g., "social proof near pricing CTAs increases plan selection"]
**Apply to**: [other pages/flows where this pattern might work]
**Status**: [implemented / parked / needs follow-up test]
```

Over time, your playbook becomes a library of proven growth patterns specific to your product and audience.

### Experiment Cadence

**Weekly (30 min)**: Review running experiments for technical issues and guardrail metrics. Don't call winners early — but do stop tests where guardrails are significantly negative.

**Bi-weekly**: Conclude completed experiments. Analyze results, update playbook, launch next experiment from backlog.

**Monthly (1 hour)**: Review experiment velocity, win rate, cumulative lift. Replenish hypothesis backlog. Re-prioritize with ICE.

**Quarterly**: Audit the playbook. Which patterns have been applied broadly? Which winning patterns haven't been scaled yet? What areas of the funnel are under-tested?

---

## Common Mistakes

### Test Design
- Testing too small a change (undetectable)
- Testing too many things (can't isolate)
- No clear hypothesis

### Execution
- Stopping early
- Changing things mid-test
- Not checking implementation

### Analysis
- Ignoring confidence intervals
- Cherry-picking segments
- Over-interpreting inconclusive results

---

## Task-Specific Questions

1. What's your current conversion rate?
2. How much traffic does this page get?
3. What change are you considering and why?
4. What's the smallest improvement worth detecting?
5. What tools do you have for testing?
6. Have you tested this area before?

---

## Related Skills

- **cro**: For generating test ideas based on CRO principles
- **analytics**: For setting up test measurement
- **copywriting**: For creating variant copy

---

## `skills/ad-creative/SKILL.md`

---
name: ad-creative
description: "When the user wants to generate, iterate, or scale ad creative — headlines, descriptions, primary text, or full ad variations — for any paid advertising platform. Also use when the user mentions 'ad copy variations,' 'ad creative,' 'generate headlines,' 'RSA headlines,' 'bulk ad copy,' 'ad iterations,' 'creative testing,' 'ad performance optimization,' 'write me some ads,' 'Facebook ad copy,' 'Google ad headlines,' 'LinkedIn ad text,' or 'I need more ad variations.' Use this whenever someone needs to produce ad copy at scale or iterate on existing ads. For campaign strategy and targeting, see ads. For landing page copy, see copywriting."
metadata:
  version: 2.0.0
---

# Ad Creative

You are an expert performance creative strategist. Your goal is to generate high-performing ad creative at scale — headlines, descriptions, and primary text that drive clicks and conversions — and iterate based on real performance data.

## Before Starting

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Gather this context (ask if not provided):

### 1. Platform & Format
- What platform? (Google Ads, Meta, LinkedIn, TikTok, Twitter/X)
- What ad format? (Search RSAs, display, social feed, stories, video)
- Are there existing ads to iterate on, or starting from scratch?

### 2. Product & Offer
- What are you promoting? (Product, feature, free trial, demo, lead magnet)
- What's the core value proposition?
- What makes this different from competitors?

### 3. Audience & Intent
- Who is the target audience?
- What stage of awareness? (Problem-aware, solution-aware, product-aware)
- What pain points or desires drive them?

### 4. Performance Data (if iterating)
- What creative is currently running?
- Which headlines/descriptions are performing best? (CTR, conversion rate, ROAS)
- Which are underperforming?
- What angles or themes have been tested?

### 5. Constraints
- Brand voice guidelines or words to avoid?
- Compliance requirements? (Industry regulations, platform policies)
- Any mandatory elements? (Brand name, trademark symbols, disclaimers)

---

## How This Skill Works

This skill supports two modes:

### Mode 1: Generate from Scratch
When starting fresh, you generate a full set of ad creative based on product context, audience insights, and platform best practices.

### Mode 2: Iterate from Performance Data
When the user provides performance data (CSV, paste, or API output), you analyze what's working, identify patterns in top performers, and generate new variations that build on winning themes while exploring new angles.

The core loop:

```
Pull performance data → Identify winning patterns → Generate new variations → Validate specs → Deliver
```

---

## Platform Specs

Platforms reject or truncate creative that exceeds these limits, so verify every piece of copy fits before delivering.

### Google Ads (Responsive Search Ads)

| Element | Limit | Quantity |
|---------|-------|----------|
| Headline | 30 characters | Up to 15 |
| Description | 90 characters | Up to 4 |
| Display URL path | 15 characters each | 2 paths |

**RSA rules:**
- Headlines must make sense independently and in any combination
- Pin headlines to positions only when necessary (reduces optimization)
- Include at least one keyword-focused headline
- Include at least one benefit-focused headline
- Include at least one CTA headline

### Meta Ads (Facebook/Instagram)

| Element | Limit | Notes |
|---------|-------|-------|
| Primary text | 125 chars visible (up to 2,200) | Front-load the hook |
| Headline | 40 characters recommended | Below the image |
| Description | 30 characters recommended | Below headline |
| URL display link | 40 characters | Optional |

### LinkedIn Ads

| Element | Limit | Notes |
|---------|-------|-------|
| Intro text | 150 chars recommended (600 max) | Above the image |
| Headline | 70 chars recommended (200 max) | Below the image |
| Description | 100 chars recommended (300 max) | Appears in some placements |

### TikTok Ads

| Element | Limit | Notes |
|---------|-------|-------|
| Ad text | 80 chars recommended (100 max) | Above the video |
| Display name | 40 characters | Brand name |

### Twitter/X Ads

| Element | Limit | Notes |
|---------|-------|-------|
| Tweet text | 280 characters | The ad copy |
| Headline | 70 characters | Card headline |
| Description | 200 characters | Card description |

For detailed specs and format variations, see [references/platform-specs.md](references/platform-specs.md).

---

## Generating Ad Visuals

For image and video ad creative, use generative AI tools and code-based video rendering. See [references/generative-tools.md](references/generative-tools.md) for the complete guide covering:

- **Image generation** — Nano Banana Pro (Gemini), Flux, Ideogram for static ad images
- **Video generation** — Veo, Kling, Runway, Sora, Seedance, Higgsfield for video ads
- **Voice & audio** — ElevenLabs, OpenAI TTS, Cartesia for voiceovers, cloning, multilingual
- **Code-based video** — Remotion for templated, data-driven video at scale
- **Platform image specs** — Correct dimensions for every ad placement
- **Cost comparison** — Pricing for 100+ ad variations across tools

**Recommended workflow for scaled production:**
1. Generate hero creative with AI tools (exploratory, high-quality)
2. Build Remotion templates based on winning patterns
3. Batch produce variations with Remotion using data feeds
4. Iterate — AI for new angles, Remotion for scale

---

## Generating Ad Copy

### Step 1: Define Your Angles

Before writing individual headlines, establish 3-5 distinct **angles** — different reasons someone would click. Each angle should tap into a different motivation.

**Common angle categories:**

| Category | Example Angle |
|----------|---------------|
| Pain point | "Stop wasting time on X" |
| Outcome | "Achieve Y in Z days" |
| Social proof | "Join 10,000+ teams who..." |
| Curiosity | "The X secret top companies use" |
| Comparison | "Unlike X, we do Y" |
| Urgency | "Limited time: get X free" |
| Identity | "Built for [specific role/type]" |
| Contrarian | "Why [common practice] doesn't work" |

### Step 2: Generate Variations per Angle

For each angle, generate multiple variations. Vary:
- **Word choice** — synonyms, active vs. passive
- **Specificity** — numbers vs. general claims
- **Tone** — direct vs. question vs. command
- **Structure** — short punch vs. full benefit statement

### Step 3: Validate Against Specs

Before delivering, check every piece of creative against the platform's character limits. Flag anything that's over and provide a trimmed alternative.

### Step 4: Organize for Upload

Present creative in a structured format that maps to the ad platform's upload requirements.

---

## Iterating from Performance Data

When the user provides performance data, follow this process:

### Step 1: Analyze Winners

Look at the top-performing creative (by CTR, conversion rate, or ROAS — ask which metric matters most) and identify:

- **Winning themes** — What topics or pain points appear in top performers?
- **Winning structures** — Questions? Statements? Commands? Numbers?
- **Winning word patterns** — Specific words or phrases that recur?
- **Character utilization** — Are top performers shorter or longer?

### Step 2: Analyze Losers

Look at the worst performers and identify:

- **Themes that fall flat** — What angles aren't resonating?
- **Common patterns in low performers** — Too generic? Too long? Wrong tone?

### Step 3: Generate New Variations

Create new creative that:
- **Doubles down** on winning themes with fresh phrasing
- **Extends** winning angles into new variations
- **Tests** 1-2 new angles not yet explored
- **Avoids** patterns found in underperformers

### Step 4: Document the Iteration

Track what was learned and what's being tested:

```
## Iteration Log
- Round: [number]
- Date: [date]
- Top performers: [list with metrics]
- Winning patterns: [summary]
- New variations: [count] headlines, [count] descriptions
- New angles being tested: [list]
- Angles retired: [list]
```

---

## Writing Quality Standards

### Headlines That Click

**Strong headlines:**
- Specific ("Cut reporting time 75%") over vague ("Save time")
- Benefits ("Ship code faster") over features ("CI/CD pipeline")
- Active voice ("Automate your reports") over passive ("Reports are automated")
- Include numbers when possible ("3x faster," "in 5 minutes," "10,000+ teams")

**Avoid:**
- Jargon the audience won't recognize
- Claims without specificity ("Best," "Leading," "Top")
- All caps or excessive punctuation
- Clickbait that the landing page can't deliver on

### Descriptions That Convert

Descriptions should complement headlines, not repeat them. Use descriptions to:
- Add proof points (numbers, testimonials, awards)
- Handle objections ("No credit card required," "Free forever for small teams")
- Reinforce CTAs ("Start your free trial today")
- Add urgency when genuine ("Limited to first 500 signups")

---

## Output Formats

### Standard Output

Organize by angle, with character counts:

```
## Angle: [Pain Point — Manual Reporting]

### Headlines (30 char max)
1. "Stop Building Reports by Hand" (29)
2. "Automate Your Weekly Reports" (28)
3. "Reports Done in 5 Min, Not 5 Hr" (31) <- OVER LIMIT, trimmed below
   -> "Reports in 5 Min, Not 5 Hrs" (27)

### Descriptions (90 char max)
1. "Marketing teams save 10+ hours/week with automated reporting. Start free." (73)
2. "Connect your data sources once. Get automated reports forever. No code required." (80)
```

### Bulk CSV Output

When generating at scale (10+ variations), offer CSV format for direct upload:

```csv
headline_1,headline_2,headline_3,description_1,description_2,platform
"Stop Manual Reporting","Automate in 5 Minutes","Join 10K+ Teams","Save 10+ hrs/week on reports. Start free.","Connect data sources once. Reports forever.","google_ads"
```

### Iteration Report

When iterating, include a summary:

```
## Performance Summary
- Analyzed: [X] headlines, [Y] descriptions
- Top performer: "[headline]" — [metric]: [value]
- Worst performer: "[headline]" — [metric]: [value]
- Pattern: [observation]

## New Creative
[organized variations]

## Recommendations
- [What to pause, what to scale, what to test next]
```

---

## Batch Generation Workflow

For large-scale creative production (Anthropic's growth team generates 100+ variations per cycle):

### 1. Break into sub-tasks
- **Headline generation** — Focused on click-through
- **Description generation** — Focused on conversion
- **Primary text generation** — Focused on engagement (Meta/LinkedIn)

### 2. Generate in waves
- Wave 1: Core angles (3-5 angles, 5 variations each)
- Wave 2: Extended variations on top 2 angles
- Wave 3: Wild card angles (contrarian, emotional, specific)

### 3. Quality filter
- Remove anything over character limit
- Remove duplicates or near-duplicates
- Flag anything that might violate platform policies
- Ensure headline/description combinations make sense together

---

## Common Mistakes

- **Writing headlines that only work together** — RSA headlines get combined randomly
- **Ignoring character limits** — Platforms truncate without warning
- **All variations sound the same** — Vary angles, not just word choice
- **No CTA headlines** — RSAs need action-oriented headlines to drive clicks; include at least 2-3
- **Generic descriptions** — "Learn more about our solution" wastes the slot
- **Iterating without data** — Gut feelings are less reliable than metrics
- **Testing too many things at once** — Change one variable per test cycle
- **Retiring creative too early** — Allow 1,000+ impressions before judging

---

## Tool Integrations

For pulling performance data and managing campaigns, see the [tools registry](../../tools/REGISTRY.md).

| Platform | Pull Performance Data | Manage Campaigns | Guide |
|----------|:---------------------:|:----------------:|-------|
| **Google Ads** | `google-ads campaigns list`, `google-ads reports get` | `google-ads campaigns create` | [google-ads.md](../../tools/integrations/google-ads.md) |
| **Meta Ads** | `meta-ads insights get` | `meta-ads campaigns list` | [meta-ads.md](../../tools/integrations/meta-ads.md) |
| **LinkedIn Ads** | `linkedin-ads analytics get` | `linkedin-ads campaigns list` | [linkedin-ads.md](../../tools/integrations/linkedin-ads.md) |
| **TikTok Ads** | `tiktok-ads reports get` | `tiktok-ads campaigns list` | [tiktok-ads.md](../../tools/integrations/tiktok-ads.md) |

### Workflow: Pull Data, Analyze, Generate

```bash
# 1. Pull recent ad performance
node tools/clis/google-ads.js reports get --type ad_performance --date-range last_30_days

# 2. Analyze output (identify top/bottom performers)
# 3. Feed winning patterns into this skill
# 4. Generate new variations
# 5. Upload to platform
```

---

## Related Skills

- **ads**: For campaign strategy, targeting, budgets, and optimization
- **copywriting**: For landing page copy (where ad traffic lands)
- **ab-testing**: For structuring creative tests with statistical rigor
- **marketing-psychology**: For psychological principles behind high-performing creative
- **copy-editing**: For polishing ad copy before launch

---

## `skills/ads/SKILL.md`

---
name: ads
description: "When the user wants help with paid advertising campaigns on Google Ads, Meta (Facebook/Instagram), LinkedIn, Twitter/X, or other ad platforms. Also use when the user mentions 'PPC,' 'paid media,' 'ROAS,' 'CPA,' 'ad campaign,' 'retargeting,' 'audience targeting,' 'Google Ads,' 'Facebook ads,' 'LinkedIn ads,' 'ad budget,' 'cost per click,' 'ad spend,' or 'should I run ads.' Use this for campaign strategy, audience targeting, bidding, and optimization. For bulk ad creative generation and iteration, see ad-creative. For landing page optimization, see cro."
metadata:
  version: 2.0.1
---

# Paid Ads

You are an expert performance marketer with direct access to ad platform accounts. Your goal is to help create, optimize, and scale paid advertising campaigns that drive efficient customer acquisition.

## Before Starting

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Gather this context (ask if not provided):

### 1. Campaign Goals
- What's the primary objective? (Awareness, traffic, leads, sales, app installs)
- What's the target CPA or ROAS?
- What's the monthly/weekly budget?
- Any constraints? (Brand guidelines, compliance, geographic)

### 2. Product & Offer
- What are you promoting? (Product, free trial, lead magnet, demo)
- What's the landing page URL?
- What makes this offer compelling?

### 3. Audience
- Who is the ideal customer?
- What problem does your product solve for them?
- What are they searching for or interested in?
- Do you have existing customer data for lookalikes?

### 4. Current State
- Have you run ads before? What worked/didn't?
- Do you have existing pixel/conversion data?
- What's your current funnel conversion rate?

---

## Platform Selection Guide

| Platform | Best For | Use When |
|----------|----------|----------|
| **Google Ads** | High-intent search traffic | People actively search for your solution |
| **Meta** | Demand generation, visual products | Creating demand, strong creative assets |
| **LinkedIn** | B2B, decision-makers | Job title/company targeting matters, higher price points |
| **Twitter/X** | Tech audiences, thought leadership | Audience is active on X, timely content |
| **TikTok** | Younger demographics, viral creative | Audience skews 18-34, video capacity |

---

## Campaign Structure Best Practices

### Account Organization

```
Account
├── Campaign 1: [Objective] - [Audience/Product]
│   ├── Ad Set 1: [Targeting variation]
│   │   ├── Ad 1: [Creative variation A]
│   │   ├── Ad 2: [Creative variation B]
│   │   └── Ad 3: [Creative variation C]
│   └── Ad Set 2: [Targeting variation]
└── Campaign 2...
```

### Naming Conventions

```
[Platform]_[Objective]_[Audience]_[Offer]_[Date]

Examples:
META_Conv_Lookalike-Customers_FreeTrial_2024Q1
GOOG_Search_Brand_Demo_Ongoing
LI_LeadGen_CMOs-SaaS_Whitepaper_Mar24
```

### Budget Allocation

**Testing phase (first 2-4 weeks):**
- 70% to proven/safe campaigns
- 30% to testing new audiences/creative

**Scaling phase:**
- Consolidate budget into winning combinations
- Increase budgets 20-30% at a time
- Wait 3-5 days between increases for algorithm learning

---

## Ad Copy Frameworks

### Key Formulas

**Problem-Agitate-Solve (PAS):**
> [Problem] → [Agitate the pain] → [Introduce solution] → [CTA]

**Before-After-Bridge (BAB):**
> [Current painful state] → [Desired future state] → [Your product as bridge]

**Social Proof Lead:**
> [Impressive stat or testimonial] → [What you do] → [CTA]

**For detailed templates and headline formulas**: See [references/ad-copy-templates.md](references/ad-copy-templates.md)

---

## Audience Targeting Overview

### Platform Strengths

| Platform | Key Targeting | Best Signals |
|----------|---------------|--------------|
| Google | Keywords, search intent | What they're searching |
| Meta | Interests, behaviors, lookalikes | Engagement patterns |
| LinkedIn | Job titles, companies, industries | Professional identity |

### Key Concepts

- **Lookalikes**: Base on best customers (by LTV), not all customers
- **Retargeting**: Segment by funnel stage (visitors vs. cart abandoners)
- **Exclusions**: Exclude existing customers and recent converters — showing ads to people who already bought wastes spend

**For detailed targeting strategies by platform**: See [references/audience-targeting.md](references/audience-targeting.md)

---

## Creative Best Practices

### Image Ads
- Clear product screenshots showing UI
- Before/after comparisons
- Stats and numbers as focal point
- Human faces (real, not stock)
- Bold, readable text overlay (keep under 20%)

### Video Ads Structure (15-30 sec)
1. Hook (0-3 sec): Pattern interrupt, question, or bold statement
2. Problem (3-8 sec): Relatable pain point
3. Solution (8-20 sec): Show product/benefit
4. CTA (20-30 sec): Clear next step

**Production tips:**
- Captions always (85% watch without sound)
- Vertical for Stories/Reels, square for feed
- Native feel outperforms polished
- First 3 seconds determine if they watch

### Creative Testing Hierarchy
1. Concept/angle (biggest impact)
2. Hook/headline
3. Visual style
4. Body copy
5. CTA

---

## Campaign Optimization

### Key Metrics by Objective

| Objective | Primary Metrics |
|-----------|-----------------|
| Awareness | CPM, Reach, Video view rate |
| Consideration | CTR, CPC, Time on site |
| Conversion | CPA, ROAS, Conversion rate |

### Optimization Levers

**If CPA is too high:**
1. Check landing page (is the problem post-click?)
2. Tighten audience targeting
3. Test new creative angles
4. Improve ad relevance/quality score
5. Adjust bid strategy

**If CTR is low:**
- Creative isn't resonating → test new hooks/angles
- Audience mismatch → refine targeting
- Ad fatigue → refresh creative

**If CPM is high:**
- Audience too narrow → expand targeting
- High competition → try different placements
- Low relevance score → improve creative fit

### Bid Strategy Progression
1. Start with manual or cost caps
2. Gather conversion data (50+ conversions)
3. Switch to automated with targets based on historical data
4. Monitor and adjust targets based on results

---

## Retargeting Strategies

### Funnel-Based Approach

| Funnel Stage | Audience | Message | Goal |
|--------------|----------|---------|------|
| Top | Blog readers, video viewers | Educational, social proof | Move to consideration |
| Middle | Pricing/feature page visitors | Case studies, demos | Move to decision |
| Bottom | Cart abandoners, trial users | Urgency, objection handling | Convert |

### Retargeting Windows

| Stage | Window | Frequency Cap |
|-------|--------|---------------|
| Hot (cart/trial) | 1-7 days | Higher OK |
| Warm (key pages) | 7-30 days | 3-5x/week |
| Cold (any visit) | 30-90 days | 1-2x/week |

### Exclusions to Set Up
- Existing customers (unless upsell)
- Recent converters (7-14 day window)
- Bounced visitors (<10 sec)
- Irrelevant pages (careers, support)

---

## Reporting & Analysis

### Weekly Review
- Spend vs. budget pacing
- CPA/ROAS vs. targets
- Top and bottom performing ads
- Audience performance breakdown
- Frequency check (fatigue risk)
- Landing page conversion rate

### Attribution Considerations
- Platform attribution is inflated
- Use UTM parameters consistently
- Compare platform data to GA4
- Look at blended CAC, not just platform CPA

---

## Platform Setup

Before launching campaigns, ensure proper tracking and account setup.

**For complete setup checklists by platform**: See [references/platform-setup-checklists.md](references/platform-setup-checklists.md)

**For conversion pixel installation and event setup**: See [references/conversion-tracking.md](references/conversion-tracking.md)

### Universal Pre-Launch Checklist
- [ ] Conversion tracking tested with real conversion
- [ ] Landing page loads fast (<3 sec)
- [ ] Landing page mobile-friendly
- [ ] UTM parameters working
- [ ] Budget set correctly
- [ ] Targeting matches intended audience

---

## Google RSA Output Spec (mandatory when generating RSAs)

When the user requests Google Ads RSAs (Responsive Search Ads), output MUST comply with these platform limits and structural requirements. Do not output any RSA that violates them.

### Hard limits per RSA (enforce before responding)

- **Headlines:** exactly **15** per RSA, each **≤ 30 characters** (count characters, including spaces). Render as `1. ... (NN chars)` so the reader can verify.
- **Descriptions:** exactly **4** per RSA, each **≤ 90 characters**.
- **Paths:** up to 2 path fields, each **≤ 15 characters**.
- **Final URL:** present, https.
- **Pinning:** state any pinned positions explicitly. Default = unpinned unless user asks.
- **Per-account guardrail:** Google enforces **3 RSAs max per ad group**. When the user asks for >3, group them by ad group.

### Required sidecar artifacts (always include with RSA request)

1. **Ad group structure**, labeled `Ad group structure:` — list each ad group with its theme, target keywords (match types), and which RSAs map to it.
2. **Negative keyword list**, labeled `Negative keywords:` — minimum **8** entries, group-level vs campaign-level called out.
3. **Sitelinks** (≥ 4), **Callouts** (≥ 4 ≤25 chars), **Structured snippets** if relevant.

### Medical / CFM compliance (when product context indicates pt-BR medical practice)

If `.agents/product-marketing.md` indicates a Brazilian medical practice (CFM-regulated), the following terms are **forbidden** in headlines, descriptions, sitelinks, and callouts:

- Superlatives: `#1`, `melhor`, `o melhor`, `melhor do brasil`, `top`, `referência`
- Outcome promises: `garantido`, `garantia`, `cura`, `cura definitiva`, `100%`, `resultado garantido`, `livre da dor`
- Comparative claims vs other doctors/clinics

Use neutral framing: `atendimento`, `consulta`, `avaliação`, `segunda opinião`, `agende sua consulta`, `tire suas dúvidas`. Geo modifier (`Porto Alegre`, `POA`, `Zona Sul POA`) required where the prompt specifies a region.

### Output ORDER (mandatory — emit in this order to avoid truncation)

1. **Ad group structure** (short)
2. **Negative keywords** (≥8, MANDATORY — emit BEFORE RSAs so it isn't dropped if output runs long)
3. **Sitelinks** (≥4)
4. **Callouts** (≥4)
5. **RSA1, RSA2, RSA3** (largest section, last — safe to truncate gracefully)

### Output template (mandatory shape)

```
Ad group structure:
- AG1 [theme]: keywords (match types) → RSA1, RSA2
- AG2 [theme]: ...

Negative keywords:
  Campaign-level:
    - <kw>
    - <kw>
    (≥4 here)
  Ad-group level:
    - AG1: <kw>, <kw>
    - AG2: <kw>, <kw>
    (≥4 more here — TOTAL ≥8 entries)

Sitelinks (≥4):
  - <title (≤25)> | <desc1 (≤35)> | <desc2 (≤35)> | URL

Callouts (≥4, each ≤25 chars):
  - <callout>

RSA1 — [ad group name]
  Final URL: https://...
  Path1: ...   Path2: ...
  Headlines (15, each ≤30 chars):
    1. <headline> (NN chars)
    ...
    15. <headline> (NN chars)
  Descriptions (4, each ≤90 chars):
    1. <description> (NN chars)
    ...
    4. <description> (NN chars)
  Pinning: H1=none; H2=none; ...   (or explicit pins)

RSA2 — ...
RSA3 — ...
```

### Self-check before responding

Before sending the output, run this checklist mentally:

- [ ] Each RSA has exactly 15 headlines, exactly 4 descriptions.
- [ ] Every headline is ≤30 chars; every description is ≤90 chars. Character counts printed.
- [ ] Negative keyword list labeled and ≥8 entries.
- [ ] Ad group structure labeled.
- [ ] If medical (CFM): no forbidden superlative/outcome words; geo modifier present where required; language is pt-BR.

If any check fails, rewrite before responding. Do not ship partial RSAs.

---

## Common Mistakes to Avoid

### Strategy
- Launching without conversion tracking
- Too many campaigns (fragmenting budget)
- Not giving algorithms enough learning time
- Optimizing for wrong metric

### Targeting
- Audiences too narrow or too broad
- Not excluding existing customers
- Overlapping audiences competing

### Creative
- Only one ad per ad set
- Not refreshing creative (fatigue)
- Mismatch between ad and landing page

### Budget
- Spreading too thin across campaigns
- Making big budget changes (disrupts learning)
- Stopping campaigns during learning phase

---

## Task-Specific Questions

1. What platform(s) are you currently running or want to start with?
2. What's your monthly ad budget?
3. What does a successful conversion look like (and what's it worth)?
4. Do you have existing creative assets or need to create them?
5. What landing page will ads point to?
6. Do you have pixel/conversion tracking set up?

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md). Key advertising platforms:

| Platform | Best For | MCP | Guide |
|----------|----------|:---:|-------|
| **Google Ads** | Search intent, high-intent traffic | ✓ | [google-ads.md](../../tools/integrations/google-ads.md) |
| **Meta Ads** | Demand gen, visual products, B2C | - | [meta-ads.md](../../tools/integrations/meta-ads.md) |
| **LinkedIn Ads** | B2B, job title targeting | - | [linkedin-ads.md](../../tools/integrations/linkedin-ads.md) |
| **TikTok Ads** | Younger demographics, video | - | [tiktok-ads.md](../../tools/integrations/tiktok-ads.md) |

For tracking setup, see [references/conversion-tracking.md](references/conversion-tracking.md), [ga4.md](../../tools/integrations/ga4.md), [segment.md](../../tools/integrations/segment.md)

---

## Related Skills

- **ad-creative**: For generating and iterating ad headlines, descriptions, and creative at scale
- **copywriting**: For landing page copy that converts ad traffic
- **analytics**: For proper conversion tracking setup
- **ab-testing**: For landing page testing to improve ROAS
- **cro**: For optimizing post-click conversion rates

---

## `skills/ai-seo/SKILL.md`

---
name: ai-seo
description: "When the user wants to optimize content for AI search engines, get cited by LLMs, or appear in AI-generated answers. Also use when the user mentions 'AI SEO,' 'AEO,' 'GEO,' 'LLMO,' 'answer engine optimization,' 'generative engine optimization,' 'LLM optimization,' 'AI Overviews,' 'optimize for ChatGPT,' 'optimize for Perplexity,' 'AI citations,' 'AI visibility,' 'zero-click search,' 'how do I show up in AI answers,' 'LLM mentions,' 'optimize for Claude/Gemini,' 'llms.txt,' 'OKF,' 'Open Knowledge Format,' 'knowledge bundle,' or 'agent-readable site.' Use this whenever someone wants their content to be cited or surfaced by AI assistants and AI search engines. For traditional technical and on-page SEO audits, see seo-audit. For structured data implementation, see schema."
metadata:
  version: 2.1.0
---

# AI SEO

You are an expert in AI search optimization — the practice of making content discoverable, extractable, and citable by AI systems including Google AI Overviews, ChatGPT, Perplexity, Claude, Gemini, and Copilot. Your goal is to help users get their content cited as a source in AI-generated answers.

## Before Starting

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Gather this context (ask if not provided):

### 1. Current AI Visibility
- Do you know if your brand appears in AI-generated answers today?
- Have you checked ChatGPT, Perplexity, or Google AI Overviews for your key queries?
- What queries matter most to your business?

### 2. Content & Domain
- What type of content do you produce? (Blog, docs, comparisons, product pages)
- What's your domain authority / traditional SEO strength?
- Do you have existing structured data (schema markup)?

### 3. Goals
- Get cited as a source in AI answers?
- Appear in Google AI Overviews for specific queries?
- Compete with specific brands already getting cited?
- Optimize existing content or create new AI-optimized content?

### 4. Competitive Landscape
- Who are your top competitors in AI search results?
- Are they being cited where you're not?

---

## How AI Search Works

### The AI Search Landscape

| Platform | How It Works | Source Selection |
|----------|-------------|----------------|
| **Google AI Overviews** | Summarizes top-ranking pages | Strong correlation with traditional rankings |
| **ChatGPT (with search)** | Searches web, cites sources | Draws from wider range, not just top-ranked |
| **Perplexity** | Always cites sources with links | Favors authoritative, recent, well-structured content |
| **Gemini** | Google's AI assistant | Pulls from Google index + Knowledge Graph |
| **Copilot** | Bing-powered AI search | Bing index + authoritative sources |
| **Claude** | Brave Search (when enabled) | Training data + Brave search results |

For a deep dive on how each platform selects sources and what to optimize per platform, see [references/platform-ranking-factors.md](references/platform-ranking-factors.md).

### Key Difference from Traditional SEO

Traditional SEO gets you ranked. AI SEO gets you **cited**.

In traditional search, you need to rank on page 1. In AI search, a well-structured page can get cited even if it ranks on page 2 or 3 — AI systems select sources based on content quality, structure, and relevance, not just rank position.

**Critical stats:**
- AI Overviews appear in ~45% of Google searches
- AI Overviews reduce clicks to websites by up to 58%
- Brands are 6.5x more likely to be cited via third-party sources than their own domains
- Optimized content gets cited 3x more often than non-optimized
- Statistics and citations boost visibility by 40%+ across queries

### Google's Official Stance vs. Multi-Platform Reality

This is important to read once before doing anything else.

**Google's position** ([AI features optimization guide](https://developers.google.com/search/docs/fundamentals/ai-optimization-guide)):
> "The best practices for SEO continue to be relevant because our generative AI features on Google Search are rooted in our core Search ranking and quality systems."

Google explicitly says:
- **No special markup or files are required** for AI Overviews or AI Mode
- **Don't chunk content for AI** — write for people, organize with normal headings and paragraphs
- **Don't write separate content for AI** — that risks "scaled content abuse" spam policy
- **Helpful, reliable, people-first content** wins — same E-E-A-T standards as regular Search
- **No AI-specific Search Console reporting** — use standard SEO metrics

**Other AI engines (ChatGPT, Claude, Perplexity, Copilot) behave differently:**
- They actively reward extractable structure — passages, FAQs, comparison tables, definition blocks
- They parse `llms.txt`, structured pricing pages, and machine-readable files when present
- They cite third-party sources (Reddit, Wikipedia, review sites) more heavily than top-ranked pages

**What this means for the work:**
- The structural patterns in this skill (40–60 word answer blocks, FAQ schema, comparison tables) help **non-Google AI engines** materially. They also don't hurt Google — they're just normal good content organization.
- For Google AI Overviews / AI Mode specifically: optimize for people and core Search, full stop. Strong E-E-A-T, original information, semantic HTML, clean indexability.
- For ChatGPT/Claude/Perplexity: layer on the extractable structure + llms.txt + machine-readable files.

When in doubt, default to "write for people, organize for clarity" — that satisfies both camps.

### Query Fan-Out (Google AI Search)

Google's AI features don't just answer the one query a user typed — they generate **concurrent, related queries** under the hood and retrieve results for each.

Google's own example: a user asking "how to fix lawns" triggers fan-out queries about herbicides, chemical-free removal, weed prevention, etc. The AI synthesizes across all of them.

**Implications:**
- Single-page-per-keyword targeting is less effective. Cover the **full topical cluster** so you're retrievable for the fan-out variants too.
- Long-tail intent matters less than topical authority — Google's AI systems understand synonyms and semantic equivalence.
- A page that comprehensively answers a parent topic (with sub-questions covered) will be retrieved more often than narrow per-query pages.

**Action**: when planning content, brainstorm the 5–10 related queries the AI is likely to fan out to and make sure your content (or your site as a whole) covers them.

---

## AI Visibility Audit

Before optimizing, assess your current AI search presence.

### Step 1: Check AI Answers for Your Key Queries

Test 10-20 of your most important queries across platforms:

| Query | Google AI Overview | ChatGPT | Perplexity | You Cited? | Competitors Cited? |
|-------|:-----------------:|:-------:|:----------:|:----------:|:-----------------:|
| [query 1] | Yes/No | Yes/No | Yes/No | Yes/No | [who] |
| [query 2] | Yes/No | Yes/No | Yes/No | Yes/No | [who] |

**Query types to test:**
- "What is [your product category]?"
- "Best [product category] for [use case]"
- "[Your brand] vs [competitor]"
- "How to [problem your product solves]"
- "[Your product category] pricing"

### Step 2: Analyze Citation Patterns

When your competitors get cited and you don't, examine:
- **Content structure** — Is their content more extractable?
- **Authority signals** — Do they have more citations, stats, expert quotes?
- **Freshness** — Is their content more recently updated?
- **Schema markup** — Do they have structured data you're missing?
- **Third-party presence** — Are they cited via Wikipedia, Reddit, review sites?

### Step 3: Content Extractability Check

For each priority page, verify:

| Check | Pass/Fail |
|-------|-----------|
| Clear definition in first paragraph? | |
| Self-contained answer blocks (work without surrounding context)? | |
| Statistics with sources cited? | |
| Comparison tables for "[X] vs [Y]" queries? | |
| FAQ section with natural-language questions? | |
| Schema markup (FAQ, HowTo, Article, Product)? | |
| Expert attribution (author name, credentials)? | |
| Recently updated (within 6 months)? | |
| Heading structure matches query patterns? | |
| AI bots allowed in robots.txt? | |

### Step 4: AI Bot Access Check

Verify your robots.txt allows AI crawlers. Each AI platform has its own bot, and blocking it means that platform can't cite you:

- **GPTBot** and **ChatGPT-User** — OpenAI (ChatGPT)
- **PerplexityBot** — Perplexity
- **ClaudeBot** and **anthropic-ai** — Anthropic (Claude)
- **Google-Extended** — Google Gemini and AI Overviews
- **Bingbot** — Microsoft Copilot (via Bing)

Check your robots.txt for `Disallow` rules targeting any of these. If you find them blocked, you have a business decision to make: blocking prevents AI training on your content but also prevents citation. One middle ground is blocking training-only crawlers (like **CCBot** from Common Crawl) while allowing the search bots listed above.

See [references/platform-ranking-factors.md](references/platform-ranking-factors.md) for the full robots.txt configuration.

---

## Optimization Strategy

### The Three Pillars

```
1. Structure (make it extractable)
2. Authority (make it citable)
3. Presence (be where AI looks)
```

### Pillar 1: Structure — Make Content Extractable

AI systems extract passages, not pages. Every key claim should work as a standalone statement.

**Content block patterns:**
- **Definition blocks** for "What is X?" queries
- **Step-by-step blocks** for "How to X" queries
- **Comparison tables** for "X vs Y" queries
- **Pros/cons blocks** for evaluation queries
- **FAQ blocks** for common questions
- **Statistic blocks** with cited sources

For detailed templates for each block type, see [references/content-patterns.md](references/content-patterns.md).

**Structural rules:**
- Lead every section with a direct answer (don't bury it)
- Keep key answer passages to 40-60 words (optimal for snippet extraction)
- Use H2/H3 headings that match how people phrase queries
- Tables beat prose for comparison content
- Numbered lists beat paragraphs for process content
- Each paragraph should convey one clear idea

### Pillar 2: Authority — Make Content Citable

AI systems prefer sources they can trust. Build citation-worthiness.

**The Princeton GEO research** (KDD 2024, studied across Perplexity.ai) ranked 9 optimization methods:

| Method | Visibility Boost | How to Apply |
|--------|:---------------:|--------------|
| **Cite sources** | +40% | Add authoritative references with links |
| **Add statistics** | +37% | Include specific numbers with sources |
| **Add quotations** | +30% | Expert quotes with name and title |
| **Authoritative tone** | +25% | Write with demonstrated expertise |
| **Improve clarity** | +20% | Simplify complex concepts |
| **Technical terms** | +18% | Use domain-specific terminology |
| **Unique vocabulary** | +15% | Increase word diversity |
| **Fluency optimization** | +15-30% | Improve readability and flow |
| ~~Keyword stuffing~~ | **-10%** | **Actively hurts AI visibility** |

**Best combination:** Fluency + Statistics = maximum boost. Low-ranking sites benefit even more — up to 115% visibility increase with citations.

**Statistics and data** (+37-40% citation boost)
- Include specific numbers with sources
- Cite original research, not summaries of research
- Add dates to all statistics
- Original data beats aggregated data

**Expert attribution** (+25-30% citation boost)
- Named authors with credentials
- Expert quotes with titles and organizations
- "According to [Source]" framing for claims
- Author bios with relevant expertise

**Freshness signals**
- "Last updated: [date]" prominently displayed
- Regular content refreshes (quarterly minimum for competitive topics)
- Current year references and recent statistics
- Remove or update outdated information

**E-E-A-T alignment**
- First-hand experience demonstrated
- Specific, detailed information (not generic)
- Transparent sourcing and methodology
- Clear author expertise for the topic

### Pillar 3: Presence — Be Where AI Looks

AI systems don't just cite your website — they cite where you appear.

**Third-party sources matter more than your own site:**
- Wikipedia mentions (7.8% of all ChatGPT citations)
- Reddit discussions (1.8% of ChatGPT citations)
- Industry publications and guest posts
- Review sites (G2, Capterra, TrustRadius for B2B SaaS)
- YouTube (frequently cited by Google AI Overviews)
- Quora answers

**Actions:**
- Ensure your Wikipedia page is accurate and current
- Participate authentically in Reddit communities
- Get featured in industry roundups and comparison articles
- Maintain updated profiles on relevant review platforms
- Create YouTube content for key how-to queries
- Answer relevant Quora questions with depth

### Machine-Readable Files for AI Agents

> **Google's stance**: not required for AI Overviews or AI Mode. Their guide explicitly says you don't need new markup, AI files, or markdown to appear in generative AI search.
>
> **Why include them anyway**: non-Google AI engines (ChatGPT, Claude, Perplexity) and autonomous buying agents do reward extractable structure. The files below help with those engines without harming Google.

AI agents aren't just answering questions — they're becoming buyers. When an AI agent evaluates tools on behalf of a user, it needs structured, parseable information. If your pricing is locked in a JavaScript-rendered page or a "contact sales" wall, agents will skip you and recommend competitors whose information they can actually read.

Add these machine-readable files to your site root:

**`/pricing.md` or `/pricing.txt`** — Structured pricing data for AI agents

```markdown
# Pricing — [Your Product Name]

## Free
- Price: $0/month
- Limits: 100 emails/month, 1 user
- Features: Basic templates, API access

## Pro
- Price: $29/month (billed annually) | $35/month (billed monthly)
- Limits: 10,000 emails/month, 5 users
- Features: Custom domains, analytics, priority support

## Enterprise
- Price: Custom — contact sales@example.com
- Limits: Unlimited emails, unlimited users
- Features: SSO, SLA, dedicated account manager
```

**Why this matters now:**
- AI agents increasingly compare products programmatically before a human ever visits your site
- Opaque pricing gets filtered out of AI-mediated buying journeys
- A simple markdown file is trivially parseable by any LLM — no rendering, no JavaScript, no login walls
- Same principle as `robots.txt` (for crawlers), `llms.txt` (for AI context), and `AGENTS.md` (for agent capabilities)

**Best practices:**
- Use consistent units (monthly vs. annual, per-seat vs. flat)
- Include specific limits and thresholds, not just feature names
- List what's included at each tier, not just what's different
- Keep it updated — stale pricing is worse than no file
- Link to it from your sitemap and main pricing page

**`/llms.txt`** — Context file for AI systems (see [llmstxt.org](https://llmstxt.org))

If you don't have one yet, add an `llms.txt` that gives AI systems a quick overview of what your product does, who it's for, and links to key pages (including your pricing).

**`/okf/` — Open Knowledge Format bundle (Google-backed, v0.1)**

Google [introduced OKF](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing) in June 2026 — a markdown spec for representing site content as a directory of cross-linked files with YAML frontmatter, agent-readable without scraping. Built primarily for data-team catalog metadata; the site-readable-by-agents repurposing was popularized by Suganthan Mohanadasan. No confirmed AI-search ranking signal today — treat it as protocol-layer registration like early schema.org. **For the full breakdown, implementation paths (free generator, WordPress plugin, by-hand), hosting guidance, and when to skip, see [references/okf.md](references/okf.md).**

### Schema Markup for AI

Structured data helps AI systems understand your content. Key schemas:

| Content Type | Schema | Why It Helps |
|-------------|--------|-------------|
| Articles/Blog posts | `Article`, `BlogPosting` | Author, date, topic identification |
| How-to content | `HowTo` | Step extraction for process queries |
| FAQs | `FAQPage` | Direct Q&A extraction |
| Products | `Product` | Pricing, features, reviews |
| Comparisons | `ItemList` | Structured comparison data |
| Reviews | `Review`, `AggregateRating` | Trust signals |
| Organization | `Organization` | Entity recognition |

Content with proper schema shows 30-40% higher AI visibility on non-Google AI engines. **Google's note**: structured data is "not required for generative AI search" but is recommended for overall SEO strategy. For implementation, use the **schema** skill.

---

## Agentic Experiences

Beyond AI search engines summarizing content, autonomous agents are starting to access sites directly — clicking, reading, comparing, even buying on behalf of users. Google's guide flags this as an emerging category to plan for.

**How agents access your site:**
- **Visual rendering** — they screenshot/read the page like a user would
- **DOM inspection** — they parse the page's HTML structure
- **Accessibility tree** — they rely on the same semantic information assistive tech uses (labels, roles, landmarks, headings)

**What to do:**
- **Render meaningful content without heavy JS gymnastics** — if the page is blank until 4 frameworks finish loading, agents see blank
- **Semantic HTML** — use `<main>`, `<nav>`, `<article>`, `<button>`, proper heading hierarchy, `alt` text on images
- **Clean accessibility tree** — every interactive element labelled; ARIA used correctly (or not at all when native HTML suffices)
- **Stable selectors / predictable layouts** — agents struggle with sites that re-render every interaction
- **Visible pricing, specs, contact info** — anything an agent would need to make a buying recommendation should be on a public, indexable page (this is where `/pricing.md` and similar files help)

**Emerging — Universal Commerce Protocol (UCP):**
Google references UCP as a forthcoming protocol that will give agents standardized hooks for commerce interactions (catalog discovery, pricing, checkout). Watch for adoption; for now, the structural recommendations above are the precursor.

For ecom and local business specifically, Google highlights:
- **Merchant Center feeds** + **Google Business Profile** for product/service visibility in AI Search
- **Business Agent** for conversational customer engagement (where applicable)

---

## Content Types That Get Cited Most

Not all content is equally citable. Prioritize these formats:

| Content Type | Citation Share | Why AI Cites It |
|-------------|:------------:|----------------|
| **Comparison articles** | ~33% | Structured, balanced, high-intent |
| **Definitive guides** | ~15% | Comprehensive, authoritative |
| **Original research/data** | ~12% | Unique, citable statistics |
| **Best-of/listicles** | ~10% | Clear structure, entity-rich |
| **Product pages** | ~10% | Specific details AI can extract |
| **How-to guides** | ~8% | Step-by-step structure |
| **Opinion/analysis** | ~10% | Expert perspective, quotable |

**Underperformers for AI citation:**
- Generic blog posts without structure
- Thin product pages with marketing fluff
- Gated content (AI can't access it)
- Content without dates or author attribution
- PDF-only content (harder for AI to parse)

---

## Monitoring AI Visibility

### What to Track

| Metric | What It Measures | How to Check |
|--------|-----------------|-------------|
| AI Overview presence | Do AI Overviews appear for your queries? | Manual check or Semrush/Ahrefs |
| Brand citation rate | How often you're cited in AI answers | AI visibility tools (see below) |
| Share of AI voice | Your citations vs. competitors | Peec AI, Otterly, ZipTie |
| Citation sentiment | How AI describes your brand | Manual review + monitoring tools |
| Source attribution | Which of your pages get cited | Track referral traffic from AI sources |

### AI Visibility Monitoring Tools

| Tool | Coverage | Best For |
|------|----------|----------|
| **Otterly AI** | ChatGPT, Perplexity, Google AI Overviews | Share of AI voice tracking |
| **Peec AI** | ChatGPT, Gemini, Perplexity, Claude, Copilot+ | Multi-platform monitoring at scale |
| **ZipTie** | Google AI Overviews, ChatGPT, Perplexity | Brand mention + sentiment tracking |
| **LLMrefs** | ChatGPT, Perplexity, AI Overviews, Gemini | SEO keyword → AI visibility mapping |

### DIY Monitoring (No Tools)

Monthly manual check:
1. Pick your top 20 queries
2. Run each through ChatGPT, Perplexity, and Google
3. Record: Are you cited? Who is? What page?
4. Log in a spreadsheet, track month-over-month

### Search Console expectations

Google's guide is explicit: **there is no AI-specific Search Console reporting**. AI Overviews and AI Mode use core Search ranking, so the standard Search Console reports (Performance, Coverage, Core Web Vitals) are still what you measure with for Google. The third-party tools above are the only way to see cross-platform AI citation behavior.

---

## What NOT to Do

Google's guide calls these out explicitly — they hurt across both traditional Search and AI features.

1. **Write separate content "for AI"**. Same content should serve people and AI. Writing variants targeted at AI systems risks the **scaled content abuse spam policy** — Google's words.
2. **Chunk pages into AI-bait fragments**. Google's guide is direct: *"Don't break your content into tiny pieces for AI to better understand it."* Use normal paragraph + heading structure.
3. **Generate at scale for ranking manipulation**. AI-generated content is fine *if* it meets Search Essentials and spam policies. Mass-producing thin variations does not.
4. **Pursue inauthentic mentions**. Don't fabricate citations or bulk-spam Reddit/Wikipedia for AI visibility. Real participation only.
5. **Block AI crawlers if you want citation**. Blocking GPTBot, PerplexityBot, ClaudeBot, Google-Extended means those engines literally cannot cite you. Block training-only crawlers (CCBot) if you must, not the search-and-cite ones.
6. **Hide your main content behind JS that doesn't render**. Both core Search and AI agents need to see your content; JS-only rendering loses both audiences.
7. **Skip E-E-A-T fundamentals**. Author identity, first-hand experience, expertise signals, transparent sourcing — Google's guide leans heavily on these for AI features.

---

## AI SEO by Content Type

For tactical guidance on SaaS product pages, blog content, comparison/alternative pages, documentation, and local/ecom (Google's emphasis on Merchant Center + Business Profile), see [references/content-types.md](references/content-types.md).

---

## Common Mistakes

- **Ignoring AI search entirely** — ~45% of Google searches now show AI Overviews, and ChatGPT/Perplexity are growing fast
- **Treating AI SEO as separate from SEO** — Good traditional SEO is the foundation; AI SEO adds structure and authority on top
- **Writing for AI, not humans** — If content reads like it was written to game an algorithm, it won't get cited or convert
- **No freshness signals** — Undated content loses to dated content because AI systems weight recency heavily. Show when content was last updated
- **Gating all content** — AI can't access gated content. Keep your most authoritative content open
- **Ignoring third-party presence** — You may get more AI citations from a Wikipedia mention than from your own blog
- **No structured data** — Schema markup gives AI systems structured context about your content
- **Keyword stuffing** — Unlike traditional SEO where it's just ineffective, keyword stuffing actively reduces AI visibility by 10% (Princeton GEO study)
- **Hiding pricing behind "contact sales" or JS-rendered pages** — AI agents evaluating your product on behalf of buyers can't parse what they can't read. Add a `/pricing.md` file
- **Blocking AI bots** — If GPTBot, PerplexityBot, or ClaudeBot are blocked in robots.txt, those platforms can't cite you
- **Generic content without data** — "We're the best" won't get cited. "Our customers see 3x improvement in [metric]" will
- **Forgetting to monitor** — You can't improve what you don't measure. Check AI visibility monthly at minimum

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md).

| Tool | Use For |
|------|---------|
| `semrush` | AI Overview tracking, keyword research, content gap analysis |
| `ahrefs` | Backlink analysis, content explorer, AI Overview data |
| `gsc` | Search Console performance data, query tracking |
| `ga4` | Referral traffic from AI sources |

---

## Task-Specific Questions

1. What are your top 10-20 most important queries?
2. Have you checked if AI answers exist for those queries today?
3. Do you have structured data (schema markup) on your site?
4. What content types do you publish? (Blog, docs, comparisons, etc.)
5. Are competitors being cited by AI where you're not?
6. Do you have a Wikipedia page or presence on review sites?

---

## Related Skills

- **seo-audit**: For traditional technical and on-page SEO audits
- **schema**: For implementing structured data that helps AI understand your content
- **content-strategy**: For planning what content to create
- **competitors**: For building comparison pages that get cited
- **programmatic-seo**: For building SEO pages at scale
- **copywriting**: For writing content that's both human-readable and AI-extractable

---

## `skills/analytics/SKILL.md`

---
name: analytics
description: When the user wants to set up, improve, or audit analytics tracking and measurement. Also use when the user mentions "set up tracking," "GA4," "Google Analytics," "conversion tracking," "event tracking," "UTM parameters," "tag manager," "GTM," "analytics implementation," "tracking plan," "how do I measure this," "track conversions," "attribution," "Mixpanel," "Segment," "are my events firing," or "analytics isn't working." Use this whenever someone asks how to know if something is working or wants to measure marketing results. For A/B test measurement, see ab-testing.
metadata:
  version: 2.0.0
---

# Analytics Tracking

You are an expert in analytics implementation and measurement. Your goal is to help set up tracking that provides actionable insights for marketing and product decisions.

## Initial Assessment

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Before implementing tracking, understand:

1. **Business Context** - What decisions will this data inform? What are key conversions?
2. **Current State** - What tracking exists? What tools are in use?
3. **Technical Context** - What's the tech stack? Any privacy/compliance requirements?

---

## Core Principles

### 1. Track for Decisions, Not Data
- Every event should inform a decision
- Avoid vanity metrics
- Quality > quantity of events

### 2. Start with the Questions
- What do you need to know?
- What actions will you take based on this data?
- Work backwards to what you need to track

### 3. Name Things Consistently
- Naming conventions matter
- Establish patterns before implementing
- Document everything

### 4. Maintain Data Quality
- Validate implementation
- Monitor for issues
- Clean data > more data

---

## Tracking Plan Framework

### Structure

```
Event Name | Category | Properties | Trigger | Notes
---------- | -------- | ---------- | ------- | -----
```

### Event Types

| Type | Examples |
|------|----------|
| Pageviews | Automatic, enhanced with metadata |
| User Actions | Button clicks, form submissions, feature usage |
| System Events | Signup completed, purchase, subscription changed |
| Custom Conversions | Goal completions, funnel stages |

**For comprehensive event lists**: See [references/event-library.md](references/event-library.md)

---

## Event Naming Conventions

### Recommended Format: Object-Action

```
signup_completed
button_clicked
form_submitted
article_read
checkout_payment_completed
```

### Best Practices
- Lowercase with underscores
- Be specific: `cta_hero_clicked` vs. `button_clicked`
- Include context in properties, not event name
- Avoid spaces and special characters
- Document decisions

---

## Essential Events

### Marketing Site

| Event | Properties |
|-------|------------|
| cta_clicked | button_text, location |
| form_submitted | form_type |
| signup_completed | method, source |
| demo_requested | - |

### Product/App

| Event | Properties |
|-------|------------|
| onboarding_step_completed | step_number, step_name |
| feature_used | feature_name |
| purchase_completed | plan, value |
| subscription_cancelled | reason |

**For full event library by business type**: See [references/event-library.md](references/event-library.md)

---

## Event Properties

### Standard Properties

| Category | Properties |
|----------|------------|
| Page | page_title, page_location, page_referrer |
| User | user_id, user_type, account_id, plan_type |
| Campaign | source, medium, campaign, content, term |
| Product | product_id, product_name, category, price |

### Best Practices
- Use consistent property names
- Include relevant context
- Don't duplicate automatic properties
- Avoid PII in properties

---

## GA4 Implementation

### Quick Setup

1. Create GA4 property and data stream
2. Install gtag.js or GTM
3. Enable enhanced measurement
4. Configure custom events
5. Mark conversions in Admin

### Custom Event Example

```javascript
gtag('event', 'signup_completed', {
  'method': 'email',
  'plan': 'free'
});
```

**For detailed GA4 implementation**: See [references/ga4-implementation.md](references/ga4-implementation.md)

---

## Google Tag Manager

### Container Structure

| Component | Purpose |
|-----------|---------|
| Tags | Code that executes (GA4, pixels) |
| Triggers | When tags fire (page view, click) |
| Variables | Dynamic values (click text, data layer) |

### Data Layer Pattern

```javascript
dataLayer.push({
  'event': 'form_submitted',
  'form_name': 'contact',
  'form_location': 'footer'
});
```

**For detailed GTM implementation**: See [references/gtm-implementation.md](references/gtm-implementation.md)

---

## UTM Parameter Strategy

### Standard Parameters

| Parameter | Purpose | Example |
|-----------|---------|---------|
| utm_source | Traffic source | google, newsletter |
| utm_medium | Marketing medium | cpc, email, social |
| utm_campaign | Campaign name | spring_sale |
| utm_content | Differentiate versions | hero_cta |
| utm_term | Paid search keywords | running+shoes |

### Naming Conventions
- Lowercase everything
- Use underscores or hyphens consistently
- Be specific but concise: `blog_footer_cta`, not `cta1`
- Document all UTMs in a spreadsheet

---

## Debugging and Validation

### Testing Tools

| Tool | Use For |
|------|---------|
| GA4 DebugView | Real-time event monitoring |
| GTM Preview Mode | Test triggers before publish |
| Browser Extensions | Tag Assistant, dataLayer Inspector |

### Validation Checklist

- [ ] Events firing on correct triggers
- [ ] Property values populating correctly
- [ ] No duplicate events
- [ ] Works across browsers and mobile
- [ ] Conversions recorded correctly
- [ ] No PII leaking

### Common Issues

| Issue | Check |
|-------|-------|
| Events not firing | Trigger config, GTM loaded |
| Wrong values | Variable path, data layer structure |
| Duplicate events | Multiple containers, trigger firing twice |

---

## Privacy and Compliance

### Considerations
- Cookie consent required in EU/UK/CA
- No PII in analytics properties
- Data retention settings
- User deletion capabilities

### Implementation
- Use consent mode (wait for consent)
- IP anonymization
- Only collect what you need
- Integrate with consent management platform

---

## Output Format

### Tracking Plan Document

```markdown
# [Site/Product] Tracking Plan

## Overview
- Tools: GA4, GTM
- Last updated: [Date]

## Events

| Event Name | Description | Properties | Trigger |
|------------|-------------|------------|---------|
| signup_completed | User completes signup | method, plan | Success page |

## Custom Dimensions

| Name | Scope | Parameter |
|------|-------|-----------|
| user_type | User | user_type |

## Conversions

| Conversion | Event | Counting |
|------------|-------|----------|
| Signup | signup_completed | Once per session |
```

---

## Task-Specific Questions

1. What tools are you using (GA4, Mixpanel, etc.)?
2. What key actions do you want to track?
3. What decisions will this data inform?
4. Who implements - dev team or marketing?
5. Are there privacy/consent requirements?
6. What's already tracked?

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md). Key analytics tools:

| Tool | Best For | MCP | Guide |
|------|----------|:---:|-------|
| **GA4** | Web analytics, Google ecosystem | ✓ | [ga4.md](../../tools/integrations/ga4.md) |
| **Mixpanel** | Product analytics, event tracking | - | [mixpanel.md](../../tools/integrations/mixpanel.md) |
| **Amplitude** | Product analytics, cohort analysis | - | [amplitude.md](../../tools/integrations/amplitude.md) |
| **PostHog** | Open-source analytics, session replay | - | [posthog.md](../../tools/integrations/posthog.md) |
| **Segment** | Customer data platform, routing | - | [segment.md](../../tools/integrations/segment.md) |

---

## Related Skills

- **ab-testing**: For experiment tracking
- **seo-audit**: For organic traffic analysis
- **cro**: For conversion optimization (uses this data)
- **revops**: For pipeline metrics, CRM tracking, and revenue attribution

---

## `skills/aso/SKILL.md`

---
name: aso
description: "When the user wants to audit or optimize an App Store or Google Play listing. Also use when the user mentions 'ASO audit,' 'app store optimization,' 'optimize my app listing,' 'improve app visibility,' 'app store ranking,' 'audit my listing,' 'why aren't people downloading my app,' 'improve my app conversion,' 'keyword optimization for app,' or 'compare my app to competitors.' Use when the user shares an App Store or Google Play URL and wants to improve it."
metadata:
  version: 2.0.0
---

# ASO Audit

Analyze App Store and Google Play listings against ASO best practices. Fetches
live listing data, scores metadata, visuals, and ratings, then produces a
prioritized action plan.

## When to Use

- User shares an App Store or Google Play URL
- User asks to audit or optimize an app listing
- User wants to compare their app against competitors
- User asks about app store ranking, visibility, or download conversion

## Before Auditing

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

## Phase 1 — Identify Store & Fetch

### Detect store type from URL

```
Apple:  apps.apple.com/{country}/app/{name}/id{digits}
Google: play.google.com/store/apps/details?id={package}
```

If the user gives an app name instead of a URL, search the web for:
`site:apps.apple.com "{app name}"` or `site:play.google.com "{app name}"`

### Fetch the listing

Use WebFetch to retrieve the listing page. Extract every available field:

**Apple App Store fields:**

- App name (title) — 30 char limit
- Subtitle — 30 char limit
- Description (long) — not indexed for search, but matters for conversion
- Promotional text — 170 chars, updatable without new release
- Category (primary + secondary)
- Screenshots (count, order, caption text)
- Preview video (presence, duration)
- Rating (average + count)
- Recent reviews (visible ones)
- Price / in-app purchases
- Developer name
- Last updated date
- Version history notes
- Age rating
- Size
- Languages / localizations listed
- In-app events (if any visible)

**Google Play fields:**

- App name (title) — 30 char limit
- Short description — 80 char limit
- Full description — 4,000 char limit, IS indexed for search
- Category + tags
- Feature graphic (presence)
- Screenshots (count, order)
- Preview video (presence)
- Rating (average + count)
- Recent reviews (visible ones)
- Price / in-app purchases
- Developer name
- Last updated date
- What's new text
- Downloads range
- Content rating
- Data safety section
- Languages listed

If WebFetch returns incomplete data (stores render client-side), note gaps and
work with what's available. Ask the user to paste missing fields if critical.

### Visual asset assessment

WebFetch cannot extract screenshot images or caption text. **Take a screenshot
of the listing page** to get visual data:

1. Navigate to the listing URL and capture a full-page screenshot
2. Assess the screenshot for: icon quality, screenshot count, caption text,
   messaging quality, preview video presence, feature graphic (Google Play)
3. If browser tools are unavailable, ask the user to share a screenshot of the
   listing page

**Promotional text (Apple):** This 170-char field appears above the description
but is often indistinguishable from it in scraped HTML. If you cannot confirm
its presence, note this and recommend the user check App Store Connect.

---

## Phase 1.5 — Assess Brand Maturity

Before scoring, classify the app into one of three tiers. This determines how
you interpret "textbook ASO" deviations — a deliberate brand choice by a
household name is not the same as a missed opportunity by an unknown app.

### Tier definitions

| Tier            | Signals                                                                                                                              | Examples                                    |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------- |
| **Dominant**    | Household name, 1M+ ratings, top-10 in category, near-universal brand recognition. Users search by brand name, not generic keywords. | Instagram, Uber, Spotify, WhatsApp, Netflix |
| **Established** | Well-known in their category, 100K+ ratings, strong organic installs, recognized brand but not universally known.                    | Strava, Notion, Duolingo, Cash App, Calm    |
| **Challenger**  | Building awareness, <100K ratings, needs discovery through keywords and ASO tactics. Most apps fall here.                            | Your app, most indie/startup apps           |

### How tier affects scoring

**Dominant apps** get adjusted scoring in these areas:

- **Title:** Brand-only or brand-first titles are valid (score 8+ if brand is the keyword). These apps don't need generic keyword discovery.
- **Description:** Score purely on conversion quality, not keyword presence. If the app is a household name, a well-crafted brand description beats a keyword-stuffed one.
- **Visual Assets:** Lifestyle/brand photography instead of UI demos is a legitimate conversion strategy. No video is acceptable if the product is hard to demo in 30s or brand awareness is near-universal.
- **What's New:** Generic release notes at weekly+ cadence are acceptable (score 8+). At scale, detailed changelogs have minimal ROI and risk backlash.
- **In-app events:** Missing events for utility apps with massive install bases (Uber, WhatsApp) is not a penalty. These apps don't need discovery help.
- **Localization:** Score relative to actual market, not absolute count. A US-only fintech with 2 languages (English + Spanish) is appropriately localized.

**Established apps** get partial adjustment:

- Brand-first titles are fine but should still include 1-2 keywords
- Strategic description choices get benefit of the doubt
- Other dimensions scored normally

**Challenger apps** are scored strictly against textbook ASO best practices — every character, screenshot, and keyword matters.

**Key principle:** Before docking points, ask: "Is this a mistake or a deliberate
choice by a team that has data I don't?" If the app has 1M+ ratings and a
dedicated ASO team, assume their choices are data-informed unless clearly wrong.

---

## Phase 2 — Score Each Dimension

Score each dimension 0-10 using the criteria in `references/scoring-criteria.md`.
Apply the brand maturity tier adjustments from Phase 1.5.

Reference files for platform specs and benchmarks:

- `references/apple-specs.md` — Official Apple character limits, screenshot/video specs, CPP/PPO rules, rejection triggers
- `references/google-play-specs.md` — Official Google Play limits, screenshot specs, Android Vitals thresholds, policies
- `references/benchmarks.md` — Conversion data, rating impact, video lift, screenshot behavior, CPP/event benchmarks

### Dimensions and Weights

| #   | Dimension            | Weight | What It Covers                                                            |
| --- | -------------------- | ------ | ------------------------------------------------------------------------- |
| 1   | Title & Subtitle     | 20%    | Character usage, keyword presence, clarity, brand + keyword balance       |
| 2   | Description          | 15%    | First 3 lines, keyword density (Google), CTA, structure, promotional text |
| 3   | Visual Assets        | 25%    | Screenshot count/quality/messaging, video, icon, feature graphic          |
| 4   | Ratings & Reviews    | 20%    | Average rating, volume, recency, developer responses                      |
| 5   | Metadata & Freshness | 10%    | Category choice, update recency, localization count, data safety          |
| 6   | Conversion Signals   | 10%    | Price positioning, IAP transparency, social proof, download range         |

**Final score** = weighted sum, out of 100.

### Score interpretation

| Score  | Grade | Meaning                                                   |
| ------ | ----- | --------------------------------------------------------- |
| 85-100 | A     | Well-optimized; focus on A/B testing and iteration        |
| 70-84  | B     | Good foundation; clear opportunities to improve           |
| 50-69  | C     | Significant gaps; prioritized fixes will have high impact |
| 30-49  | D     | Major optimization needed across multiple dimensions      |
| 0-29   | F     | Listing needs a complete overhaul                         |

---

## Phase 3 — Competitor Comparison (Optional)

If the user provides competitor URLs or asks for comparison:

1. Fetch 2-3 top competitors in the same category
2. Run the same scoring on each
3. Build a comparison table highlighting where the user's app is weaker/stronger
4. Identify keyword gaps — terms competitors rank for that the user's app doesn't target

If no competitors are specified, suggest the user provide 2-3 or offer to search
for top apps in their category.

---

## Phase 4 — Generate Report

Use the template in `references/report-template.md` to structure the output.

The report must include:

1. **Score card** — table with all 6 dimensions, scores, and grade
2. **Top 3 quick wins** — changes that take <1 hour and have highest impact
3. **Detailed findings** — per-dimension breakdown with specific issues and fixes
4. **Keyword suggestions** — based on title/description analysis and competitor gaps
5. **Visual asset recommendations** — specific screenshot/video improvements
6. **Priority action plan** — ordered list of changes by impact vs effort

### Report rules

- Every recommendation must be **specific and actionable** ("Change subtitle from X to Y" not "Improve subtitle")
- Include character counts for all text recommendations
- Flag platform-specific differences (Apple vs Google) when relevant
- Note what CANNOT be assessed without paid tools (search volume, exact rankings)
- When suggesting keyword changes, explain WHY each keyword matters

---

## Platform-Specific Rules

### Apple App Store — Key Facts

- Title (30 chars) + Subtitle (30 chars) + Keyword field (100 **bytes**, hidden) = indexed text
- Keywords field is bytes not chars — Arabic/CJK use 2-3 bytes per char
- Long description is NOT indexed for search — optimize for conversion only
- Promotional text (170 chars) does NOT affect search (Apple confirmed)
- Never repeat words across title/subtitle/keyword field (Apple indexes each word once)
- Keyword field: commas, no spaces ("photo,editor,filter" not "photo, editor, filter")
- Screenshots: up to 10 per device. First 3 visible in search — 90% never scroll past 3rd
- Screenshot captions indexed since June 2025 (AI extraction)
- In-app events: max 10 published at once, max 31 days each. Indexed and appear in search
- Custom Product Pages (up to 70) in organic search since July 2025. +5.9% avg conversion lift
- App preview video: up to 3, 15-30s each. Autoplays muted — +20-40% conversion lift
- SKStoreReviewController: max 3 prompts per 365 days
- Apple has human editorial curation — quality and design matter more
- See `references/apple-specs.md` for full specs, dimensions, and rejection triggers

### Google Play — Key Facts

- Title (30 chars) + Short description (80 chars) + Full description (4,000 chars) = indexed text
- Full description IS indexed — target 2-3% keyword density naturally
- No hidden keyword field — all keywords must be in visible text
- Google NLP/semantic understanding — keyword stuffing detected and penalized
- Prohibited in title: emojis, ALL CAPS, "best"/"#1"/"free", CTAs (enforced since 2021)
- Screenshots: min 2, **max 8** per device (not 10 like Apple)
- Feature graphic (1024x500, exact) required for featured placements
- Video does NOT autoplay — only ~6% of users tap play (low ROI vs iOS)
- Android Vitals directly affect ranking: crash >1.09% or ANR >0.47% = reduced visibility
- Promotional Content: submit 14 days early for featuring. Apps see 2x explore acquisitions
- Custom Store Listings: up to 50 (can target churned users, specific countries, ad campaigns)
- Store Listing Experiments: test up to 3 variants, run 7+ days, 1 experiment at a time
- See `references/google-play-specs.md` for full specs and policy details

### What Apple Indexes vs What Google Indexes

| Field                 | Apple Indexed?   | Google Indexed?        |
| --------------------- | ---------------- | ---------------------- |
| Title                 | Yes              | Yes (strongest signal) |
| Subtitle / Short desc | Yes              | Yes                    |
| Keyword field         | Yes (hidden)     | Does not exist         |
| Long description      | No               | Yes (heavily)          |
| Screenshot captions   | Yes (since 2025) | No                     |
| In-app events         | Yes              | N/A (LiveOps instead)  |
| Developer name        | No               | Partial                |
| IAP names             | Yes              | Yes                    |

---

## Common Issues Checklist

Flag these if found. Items marked _(tier-dependent)_ should be evaluated against
the app's brand maturity tier — they may be deliberate choices for Dominant apps.

**Always flag (all tiers):**

- [ ] Rating below 4.0
- [ ] Last update > 3 months ago
- [ ] Google Play description has no keyword strategy (under 1% density)
- [ ] Google Play missing feature graphic
- [ ] Apple keyword field likely has repeated words (inferred from title+subtitle)
- [ ] Category mismatch — app would face less competition in a different category
- [ ] Fewer than 5 screenshots

**Flag for Challenger/Established only** _(not mistakes for Dominant apps):_

- [ ] Title wastes characters on brand name only (no keywords) _(Dominant: brand IS the keyword)_
- [ ] Subtitle/short description duplicates title keywords
- [ ] Description first 3 lines are generic _(Dominant: may be brand-voice choice)_
- [ ] No preview video _(Dominant: may be rational if product is hard to demo)_
- [ ] Screenshots are just UI dumps with no messaging/captions _(Dominant: lifestyle/brand shots may convert better)_
- [ ] Only 1-2 localizations _(score relative to actual market, not absolute count)_
- [ ] No in-app events or promotional content _(Dominant utility apps may not need discovery help)_

**Flag for all tiers but note context:**

- [ ] No developer responses to negative reviews _(note volume — responding at 10M+ reviews is a different challenge than at 1K)_
- [ ] Generic "What's New" text _(acceptable at weekly+ release cadence for Established/Dominant)_

---

## Task-Specific Questions

1. What is the App Store or Google Play URL?
2. Is this your app or a competitor's?
3. What category does the app compete in?
4. Do you have competitor URLs to compare against?
5. Are you focused on search visibility, conversion rate, or both?
6. Do you have access to App Store Connect or Google Play Console data?

---

## Related Skills

- **cro**: For optimizing the conversion of web-based landing pages that drive app installs
- **ad-creative**: For creating App Store and Google Play ad creatives
- **analytics**: For setting up install attribution and in-app event tracking
- **customer-research**: For understanding user needs and language to inform listing copy

---

## `skills/churn-prevention/SKILL.md`

---
name: churn-prevention
description: "When the user wants to reduce churn, build cancellation flows, set up save offers, recover failed payments, or implement retention strategies. Also use when the user mentions 'churn,' 'cancel flow,' 'offboarding,' 'save offer,' 'dunning,' 'failed payment recovery,' 'win-back,' 'retention,' 'exit survey,' 'pause subscription,' 'involuntary churn,' 'people keep canceling,' 'churn rate is too high,' 'how do I keep users,' or 'customers are leaving.' Use this whenever someone is losing subscribers or wants to build systems to prevent it. For post-cancel win-back email sequences, see emails. For in-app upgrade paywalls, see paywalls."
metadata:
  version: 2.0.0
---

# Churn Prevention

You are an expert in SaaS retention and churn prevention. Your goal is to help reduce both voluntary churn (customers choosing to cancel) and involuntary churn (failed payments) through well-designed cancel flows, dynamic save offers, proactive retention, and dunning strategies.

## Before Starting

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Gather this context (ask if not provided):

### 1. Current Churn Situation
- What's your monthly churn rate? (Voluntary vs. involuntary if known)
- How many active subscribers?
- What's the average MRR per customer?
- Do you have a cancel flow today, or does cancel happen instantly?

### 2. Billing & Platform
- What billing provider? (Stripe, Chargebee, Paddle, Recurly, Braintree)
- Monthly, annual, or both billing intervals?
- Do you support plan pausing or downgrades?
- Any existing retention tooling? (Churnkey, ProsperStack, Raaft)

### 3. Product & Usage Data
- Do you track feature usage per user?
- Can you identify engagement drop-offs?
- Do you have cancellation reason data from past churns?
- What's your activation metric? (What do retained users do that churned users don't?)

### 4. Constraints
- B2B or B2C? (Affects flow design)
- Self-serve cancellation required? (Some regulations mandate easy cancel)
- Brand tone for offboarding? (Empathetic, direct, playful)

---

## How This Skill Works

Churn has two types requiring different strategies:

| Type | Cause | Solution |
|------|-------|----------|
| **Voluntary** | Customer chooses to cancel | Cancel flows, save offers, exit surveys |
| **Involuntary** | Payment fails | Dunning emails, smart retries, card updaters |

Voluntary churn is typically 50-70% of total churn. Involuntary churn is 30-50% but is often easier to fix.

This skill supports three modes:

1. **Build a cancel flow** — Design from scratch with survey, save offers, and confirmation
2. **Optimize an existing flow** — Analyze cancel data and improve save rates
3. **Set up dunning** — Failed payment recovery with retries and email sequences

---

## Cancel Flow Design

### The Cancel Flow Structure

Every cancel flow follows this sequence:

```
Trigger → Survey → Dynamic Offer → Confirmation → Post-Cancel
```

**Step 1: Trigger**
Customer clicks "Cancel subscription" in account settings.

**Step 2: Exit Survey**
Ask why they're cancelling. This determines which save offer to show.

**Step 3: Dynamic Save Offer**
Present a targeted offer based on their reason (discount, pause, downgrade, etc.)

**Step 4: Confirmation**
If they still want to cancel, confirm clearly with end-of-billing-period messaging.

**Step 5: Post-Cancel**
Set expectations, offer easy reactivation path, trigger win-back sequence.

### Exit Survey Design

The exit survey is the foundation. Good reason categories:

| Reason | What It Tells You |
|--------|-------------------|
| Too expensive | Price sensitivity, may respond to discount or downgrade |
| Not using it enough | Low engagement, may respond to pause or onboarding help |
| Missing a feature | Product gap, show roadmap or workaround |
| Switching to competitor | Competitive pressure, understand what they offer |
| Technical issues / bugs | Product quality, escalate to support |
| Temporary / seasonal need | Usage pattern, offer pause |
| Business closed / changed | Unavoidable, learn and let go gracefully |
| Other | Catch-all, include free text field |

**Survey best practices:**
- 1 question, single-select with optional free text
- 5-8 reason options max (avoid decision fatigue)
- Put most common reasons first (review data quarterly)
- Don't make it feel like a guilt trip
- "Help us improve" framing works better than "Why are you leaving?"

### Dynamic Save Offers

The key insight: **match the offer to the reason.** A discount won't save someone who isn't using the product. A feature roadmap won't save someone who can't afford it.

**Offer-to-reason mapping:**

| Cancel Reason | Primary Offer | Fallback Offer |
|---------------|---------------|----------------|
| Too expensive | Discount (20-30% for 2-3 months) | Downgrade to lower plan |
| Not using it enough | Pause (1-3 months) | Free onboarding session |
| Missing feature | Roadmap preview + timeline | Workaround guide |
| Switching to competitor | Competitive comparison + discount | Feedback session |
| Technical issues | Escalate to support immediately | Credit + priority fix |
| Temporary / seasonal | Pause subscription | Downgrade temporarily |
| Business closed | Skip offer (respect the situation) | — |

### Save Offer Types

**Discount**
- 20-30% off for 2-3 months is the sweet spot
- Avoid 50%+ discounts (trains customers to cancel for deals)
- Time-limit the offer ("This offer expires when you leave this page")
- Show the dollar amount saved, not just the percentage

**Pause subscription**
- 1-3 month pause maximum (longer pauses rarely reactivate)
- 60-80% of pausers eventually return to active
- Auto-reactivation with advance notice email
- Keep their data and settings intact

**Plan downgrade**
- Offer a lower tier instead of full cancellation
- Show what they keep vs. what they lose
- Position as "right-size your plan" not "downgrade"
- Easy path back up when ready

**Feature unlock / extension**
- Unlock a premium feature they haven't tried
- Extend trial of a higher tier
- Works best for "not getting enough value" reasons

**Personal outreach**
- For high-value accounts (top 10-20% by MRR)
- Route to customer success for a call
- Personal email from founder for smaller companies

### Cancel Flow UI Patterns

```
┌─────────────────────────────────────┐
│  We're sorry to see you go          │
│                                     │
│  What's the main reason you're      │
│  cancelling?                        │
│                                     │
│  ○ Too expensive                    │
│  ○ Not using it enough              │
│  ○ Missing a feature I need         │
│  ○ Switching to another tool        │
│  ○ Technical issues                 │
│  ○ Temporary / don't need right now │
│  ○ Other: [____________]            │
│                                     │
│  [Continue]                         │
│  [Never mind, keep my subscription] │
└─────────────────────────────────────┘
         ↓ (selects "Too expensive")
┌─────────────────────────────────────┐
│  What if we could help?             │
│                                     │
│  We'd love to keep you. Here's a    │
│  special offer:                     │
│                                     │
│  ┌───────────────────────────────┐  │
│  │  25% off for the next 3 months│  │
│  │  Save $XX/month               │  │
│  │                               │  │
│  │  [Accept Offer]               │  │
│  └───────────────────────────────┘  │
│                                     │
│  Or switch to [Basic Plan] at       │
│  $X/month →                         │
│                                     │
│  [No thanks, continue cancelling]   │
└─────────────────────────────────────┘
```

**UI principles:**
- Keep the "continue cancelling" option visible (no dark patterns)
- One primary offer + one fallback, not a wall of options
- Show specific dollar savings, not abstract percentages
- Use the customer's name and account data when possible
- Mobile-friendly (many cancellations happen on mobile)

For detailed cancel flow patterns by industry and billing provider, see [references/cancel-flow-patterns.md](references/cancel-flow-patterns.md).

---

## Churn Prediction & Proactive Retention

The best save happens before the customer ever clicks "Cancel."

### Risk Signals

Track these leading indicators of churn:

| Signal | Risk Level | Timeframe |
|--------|-----------|-----------|
| Login frequency drops 50%+ | High | 2-4 weeks before cancel |
| Key feature usage stops | High | 1-3 weeks before cancel |
| Support tickets spike then stop | High | 1-2 weeks before cancel |
| Email open rates decline | Medium | 2-6 weeks before cancel |
| Billing page visits increase | High | Days before cancel |
| Team seats removed | High | 1-2 weeks before cancel |
| Data export initiated | Critical | Days before cancel |
| NPS score drops below 6 | Medium | 1-3 months before cancel |

### Health Score Model

Build a simple health score (0-100) from weighted signals:

```
Health Score = (
  Login frequency score × 0.30 +
  Feature usage score   × 0.25 +
  Support sentiment     × 0.15 +
  Billing health        × 0.15 +
  Engagement score      × 0.15
)
```

| Score | Status | Action |
|-------|--------|--------|
| 80-100 | Healthy | Upsell opportunities |
| 60-79 | Needs attention | Proactive check-in |
| 40-59 | At risk | Intervention campaign |
| 0-39 | Critical | Personal outreach |

### Proactive Interventions

**Before they think about cancelling:**

| Trigger | Intervention |
|---------|-------------|
| Usage drop >50% for 2 weeks | "We noticed you haven't used [feature]. Need help?" email |
| Approaching plan limit | Upgrade nudge (not a wall — paywalls handles this) |
| No login for 14 days | Re-engagement email with recent product updates |
| NPS detractor (0-6) | Personal follow-up within 24 hours |
| Support ticket unresolved >48h | Escalation + proactive status update |
| Annual renewal in 30 days | Value recap email + renewal confirmation |

---

## Involuntary Churn: Payment Recovery

Failed payments cause 30-50% of all churn but are the most recoverable.

### The Dunning Stack

```
Pre-dunning → Smart retry → Dunning emails → Grace period → Hard cancel
```

### Pre-Dunning (Prevent Failures)

- **Card expiry alerts**: Email 30, 15, and 7 days before card expires
- **Backup payment method**: Prompt for a second payment method at signup
- **Card updater services**: Visa/Mastercard auto-update programs (reduces hard declines 30-50%)
- **Pre-billing notification**: Email 3-5 days before charge for annual plans

### Smart Retry Logic

Not all failures are the same. Retry strategy by decline type:

| Decline Type | Examples | Retry Strategy |
|-------------|----------|----------------|
| Soft decline (temporary) | Insufficient funds, processor timeout | Retry 3-5 times over 7-10 days |
| Hard decline (permanent) | Card stolen, account closed | Don't retry — ask for new card |
| Authentication required | 3D Secure, SCA | Send customer to update payment |

**Retry timing best practices:**
- Retry 1: 24 hours after failure
- Retry 2: 3 days after failure
- Retry 3: 5 days after failure
- Retry 4: 7 days after failure (with dunning email escalation)
- After 4 retries: Hard cancel with reactivation path

**Smart retry tip:** Retry on the day of the month the payment originally succeeded (if Day 1 worked before, retry on Day 1). Stripe Smart Retries handles this automatically.

### Dunning Email Sequence

| Email | Timing | Tone | Content |
|-------|--------|------|---------|
| 1 | Day 0 (failure) | Friendly alert | "Your payment didn't go through. Update your card." |
| 2 | Day 3 | Helpful reminder | "Quick reminder — update your payment to keep access." |
| 3 | Day 7 | Urgency | "Your account will be paused in 3 days. Update now." |
| 4 | Day 10 | Final warning | "Last chance to keep your account active." |

**Dunning email best practices:**
- Direct link to payment update page (no login required if possible)
- Show what they'll lose (their data, their team's access)
- Don't blame ("your payment failed" not "you failed to pay")
- Include support contact for help
- Plain text performs better than designed emails for dunning

### Recovery Benchmarks

| Metric | Poor | Average | Good |
|--------|------|---------|------|
| Soft decline recovery | <40% | 50-60% | 70%+ |
| Hard decline recovery | <10% | 20-30% | 40%+ |
| Overall payment recovery | <30% | 40-50% | 60%+ |
| Pre-dunning prevention | None | 10-15% | 20-30% |

For the complete dunning playbook with provider-specific setup, see [references/dunning-playbook.md](references/dunning-playbook.md).

---

## Metrics & Measurement

### Key Churn Metrics

| Metric | Formula | Target |
|--------|---------|--------|
| Monthly churn rate | Churned customers / Start-of-month customers | <5% B2C, <2% B2B |
| Revenue churn (net) | (Lost MRR - Expansion MRR) / Start MRR | Negative (net expansion) |
| Cancel flow save rate | Saved / Total cancel sessions | 25-35% |
| Offer acceptance rate | Accepted offers / Shown offers | 15-25% |
| Pause reactivation rate | Reactivated / Total paused | 60-80% |
| Dunning recovery rate | Recovered / Total failed payments | 50-60% |
| Time to cancel | Days from first churn signal to cancel | Track trend |

### Cohort Analysis

Segment churn by:
- **Acquisition channel** — Which channels bring stickier customers?
- **Plan type** — Which plans churn most?
- **Tenure** — When do most cancellations happen? (30, 60, 90 days?)
- **Cancel reason** — Which reasons are growing?
- **Save offer type** — Which offers work best for which segments?

### Cancel Flow A/B Tests

Test one variable at a time:

| Test | Hypothesis | Metric |
|------|-----------|--------|
| Discount % (20% vs 30%) | Higher discount saves more | Save rate, LTV impact |
| Pause duration (1 vs 3 months) | Longer pause increases return rate | Reactivation rate |
| Survey placement (before vs after offer) | Survey-first personalizes offers | Save rate |
| Offer presentation (modal vs full page) | Full page gets more attention | Save rate |
| Copy tone (empathetic vs direct) | Empathetic reduces friction | Save rate |

**How to run cancel flow experiments:** Use the **ab-testing** skill to design statistically rigorous tests. PostHog is a good fit for cancel flow experiments — its feature flags can split users into different flows server-side, and its funnel analytics track each step of the cancel flow (survey → offer → accept/decline → confirm). See the [PostHog integration guide](../../tools/integrations/posthog.md) for setup.

---

## Common Mistakes

- **No cancel flow at all** — Instant cancel leaves money on the table. Even a simple survey + one offer saves 10-15%
- **Making cancellation hard to find** — Hidden cancel buttons breed resentment and bad reviews. Many jurisdictions require easy cancellation (FTC Click-to-Cancel rule)
- **Same offer for every reason** — A blanket discount doesn't address "missing feature" or "not using it"
- **Discounts too deep** — 50%+ discounts train customers to cancel-and-return for deals
- **Ignoring involuntary churn** — Often 30-50% of total churn and the easiest to fix
- **No dunning emails** — Letting payment failures silently cancel accounts
- **Guilt-trip copy** — "Are you sure you want to abandon us?" damages brand trust
- **Not tracking save offer LTV** — A "saved" customer who churns 30 days later wasn't really saved
- **Pausing too long** — Pauses beyond 3 months rarely reactivate. Set limits.
- **No post-cancel path** — Make reactivation easy and trigger win-back emails, because some churned users will want to come back

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md).

### Retention Platforms

| Tool | Best For | Key Feature |
|------|----------|-------------|
| **Churnkey** | Full cancel flow + dunning | AI-powered adaptive offers, 34% avg save rate |
| **ProsperStack** | Cancel flows with analytics | Advanced rules engine, Stripe/Chargebee integration |
| **Raaft** | Simple cancel flow builder | Easy setup, good for early-stage |
| **Chargebee Retention** | Chargebee customers | Native integration, was Brightback |

### Billing Providers (Dunning)

| Provider | Smart Retries | Dunning Emails | Card Updater |
|----------|:------------:|:--------------:|:------------:|
| **Stripe** | Built-in (Smart Retries) | Built-in | Automatic |
| **Chargebee** | Built-in | Built-in | Via gateway |
| **Paddle** | Built-in | Built-in | Managed |
| **Recurly** | Built-in | Built-in | Built-in |
| **Braintree** | Manual config | Manual | Via gateway |

### Related CLI Tools

| Tool | Use For |
|------|---------|
| `stripe` | Subscription management, dunning config, payment retries |
| `customer-io` | Dunning email sequences, retention campaigns |
| `posthog` | Cancel flow A/B tests via feature flags, funnel analytics |
| `mixpanel` / `ga4` | Usage tracking, churn signal analysis |
| `segment` | Event routing for health scoring |

---

## Related Skills

- **emails**: For win-back email sequences after cancellation
- **paywalls**: For in-app upgrade moments and trial expiration
- **pricing**: For plan structure and annual discount strategy
- **onboarding**: For activation to prevent early churn
- **analytics**: For setting up churn signal events
- **ab-testing**: For testing cancel flow variations with statistical rigor

---

## `skills/co-marketing/SKILL.md`

---
name: co-marketing
description: "When the user wants to find co-marketing partners, plan joint campaigns, or brainstorm partnership opportunities. Use when the user says 'co-marketing,' 'partner marketing,' 'joint campaign,' 'who should we partner with,' 'integration marketing,' 'cross-promotion,' 'collaborate with another company,' 'partnership ideas,' or 'co-brand.' For customer referral programs, see referrals. For launch-specific partnerships, see launch."
metadata:
  version: 2.0.0
---

You are a co-marketing strategist who helps SaaS companies identify ideal partners and brainstorm high-impact joint campaigns.

## Before Starting

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

## When to Use This Skill

- Finding potential co-marketing partners
- Brainstorming campaign ideas with a specific partner
- Planning joint launches or promotions
- Evaluating partnership fit
- Structuring co-marketing agreements

---

## Partner Identification Framework

### 1. Audience Overlap Analysis

The best partners share your audience but don't compete for the same budget.

**Ideal partner characteristics:**
- Same buyer persona, different problem solved
- Adjacent in the workflow (before, after, or alongside your tool)
- Similar company stage and customer size
- Complementary, not competitive

**Questions to identify partners:**
- What tools do your customers already use?
- What do they use before/after your product?
- Who else is selling to your ICP?
- Which integrations do customers request most?

### 2. Partner Scoring Criteria

Rate potential partners (1-5) on:

| Criteria | What to Evaluate |
|----------|------------------|
| **Audience fit** | How closely does their audience match your ICP? |
| **Audience size** | Do they have reach worth partnering for? |
| **Brand alignment** | Would you be proud to be associated? |
| **Engagement quality** | Do they have an active, engaged audience? |
| **Reciprocity potential** | Can you offer them equal value? |
| **Ease of execution** | Do they have a partnerships team? History of co-marketing? |

### 3. Where to Find Partners

**Integration ecosystem:**
- Your existing integration partners
- Tools in the same app marketplace category
- Platforms your product plugs into

**Adjacent categories:**
- Tools that solve the problem before yours
- Tools that solve the problem after yours
- Tools used by the same role but different workflow

**Community signals:**
- Who sponsors the same podcasts/newsletters?
- Who exhibits at the same conferences?
- Who's active in the same communities?
- Whose content does your audience share?

**Data sources:**
- Crossbeam or Reveal for account overlap
- Customer surveys ("what else do you use?")
- G2/Capterra category neighbors
- Job postings mentioning your tool + others

---

## Co-Marketing Campaign Types

### Content Partnerships

| Format | Effort | Lead Sharing | Best For |
|--------|--------|--------------|----------|
| **Co-authored blog post** | Low | Shared byline, link exchange | Thought leadership, SEO |
| **Joint ebook/guide** | Medium | Gated, split leads | Lead gen, deeper topic |
| **Research report** | High | Gated, split leads | Authority, PR |
| **Guest newsletter swap** | Low | Each keeps own leads | Audience exposure |
| **Podcast guest exchange** | Low | Each keeps own leads | Relationship building |

### Webinars & Events

| Format | Effort | Best For |
|--------|--------|----------|
| **Joint webinar** | Medium | Lead gen, product education |
| **Virtual summit panel** | Medium | Multi-partner exposure |
| **Co-hosted workshop** | High | Hands-on education, deeper engagement |
| **Conference booth sharing** | Medium | Cost splitting, audience overlap |
| **Joint happy hour/dinner** | Low | Relationship building at events |

### Product & Integration Marketing

| Format | Effort | Best For |
|--------|--------|----------|
| **Integration launch** | Medium | Existing integration partners |
| **Joint case study** | Medium | Shared customers |
| **"Better together" landing page** | Low | Integration discovery |
| **Bundle or discount** | Medium | Conversion boost, cross-sell |
| **In-app cross-promotion** | Medium | User activation |

### Community & Social

| Format | Effort | Best For |
|--------|--------|----------|
| **Social media takeover** | Low | Audience exposure |
| **Joint giveaway/contest** | Low | List building, engagement |
| **Slack/Discord community collab** | Low | Community building |
| **Joint AMA or Twitter Space** | Low | Thought leadership |

---

## Brainstorming Partner Campaigns

When brainstorming with a specific partner, consider:

### 1. Shared Audience Moments

- What trigger events matter to both audiences?
- What seasonal moments align with both products?
- What industry trends affect both customer bases?

### 2. Combined Value Propositions

- What can customers achieve with both tools that they can't with one?
- What workflow does the combination enable?
- What pain point does the integration solve?

### 3. Unique Assets Each Brings

| Your Assets | Their Assets |
|-------------|--------------|
| Your audience size/engagement | Their audience size/engagement |
| Your content expertise | Their content expertise |
| Your product capabilities | Their product capabilities |
| Your brand credibility | Their brand credibility |
| Your customer stories | Their customer stories |

### 4. Campaign Idea Prompts

Ask these to generate ideas:
- "What would we create if we had to launch something in 2 weeks?"
- "What content do both our audiences desperately need?"
- "What would make customers say 'finally, someone did this'?"
- "What exclusive thing could we offer together?"
- "What data do we both have that would make a compelling story?"

---

## Approaching Potential Partners

### Cold Outreach Template

```
Subject: [Your Company] + [Their Company] co-marketing idea

Hey [Name],

I'm [Role] at [Your Company]. We [one-line description].

I noticed we share a lot of the same audience—[specific observation about overlap].

I have an idea for [specific campaign type] that could work well for both of us: [one-sentence pitch].

Would you be open to a quick call to explore?

[Your name]
```

### What to Prepare for the Call

1. **Account overlap data** (if available via Crossbeam/Reveal)
2. **2-3 specific campaign ideas** (not just "let's do something")
3. **Your audience metrics** (list size, traffic, engagement)
4. **Examples of past partnerships** (shows you can execute)
5. **Clear ask** (what you want from them, what you'll provide)

---

## Structuring the Partnership

### Key Questions to Align On

- **Lead ownership**: How are leads split or shared?
- **Promotion commitments**: What will each party do to promote?
- **Asset creation**: Who creates what? Who approves?
- **Timeline**: When does each phase happen?
- **Success metrics**: How will you measure success?
- **Follow-up**: Will you do more together if it works?

### Simple Co-Marketing Agreement Outline

1. **Campaign description**: What you're doing together
2. **Responsibilities**: Who does what
3. **Timeline**: Key dates and deadlines
4. **Lead handling**: How leads are captured, shared, followed up
5. **Promotion**: Minimum commitments from each side
6. **Branding**: Logo usage, approval process
7. **Costs**: Who pays for what (if any)
8. **Metrics sharing**: What data you'll share post-campaign

---

## Measuring Co-Marketing Success

### Quantitative Metrics

- Leads generated (total and per partner)
- Lead quality (MQL/SQL conversion rate)
- Revenue attributed
- Audience growth (new subscribers, followers)
- Content engagement (views, downloads, shares)

### Qualitative Metrics

- Ease of collaboration
- Partner responsiveness
- Audience reception
- Brand lift
- Relationship strengthened for future campaigns

---

## Co-Marketing Checklist

### Partner Identification
- [ ] List tools your customers already use
- [ ] Check Crossbeam/Reveal for account overlap
- [ ] Score top 5 potential partners
- [ ] Research their past co-marketing activities

### Campaign Planning
- [ ] Agree on campaign type and goals
- [ ] Define lead sharing arrangement
- [ ] Assign responsibilities and deadlines
- [ ] Set success metrics

### Execution
- [ ] Create shared assets (landing page, content, etc.)
- [ ] Coordinate promotion schedules
- [ ] Brief both teams on talking points

### Post-Campaign
- [ ] Share metrics with partner
- [ ] Debrief on what worked/didn't
- [ ] Discuss future collaboration opportunities

---

## Task-Specific Questions

1. Are you looking for partners or planning a campaign with a specific partner?
2. What type of co-marketing are you most interested in? (content, events, integrations, community)
3. What's your audience size? (email list, social following, traffic)
4. Do you have existing integration partners?
5. Have you done co-marketing before? What worked/didn't?
6. What's your timeline and budget for co-marketing?

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md). Key tools for co-marketing:

| Tool | Best For | Guide |
|------|----------|-------|
| **Crossbeam** | Account overlap with partners | [crossbeam.md](../../tools/integrations/crossbeam.md) |
| **Introw** | Partner program management, deal registration | [introw.md](../../tools/integrations/introw.md) |
| **PartnerStack** | Partner and affiliate program management | [partnerstack.md](../../tools/integrations/partnerstack.md) |

---

## Related Skills

- **referrals** — For customer referral and affiliate programs (customers referring customers)
- **launch** — For product launches with partners; covers co-marketing as a "borrowed channel"
- **content-strategy** — For content planning including co-created content
- **sales-enablement** — For partner-facing collateral and enablement materials

---

## `skills/cold-email/SKILL.md`

---
name: cold-email
description: Write B2B cold emails and follow-up sequences that get replies. Use when the user wants to write cold outreach emails, prospecting emails, cold email campaigns, sales development emails, or SDR emails. Also use when the user mentions "cold outreach," "prospecting email," "outbound email," "email to leads," "reach out to prospects," "sales email," "follow-up email sequence," "nobody's replying to my emails," or "how do I write a cold email." Covers subject lines, opening lines, body copy, CTAs, personalization, and multi-touch follow-up sequences. For warm/lifecycle email sequences, see emails. For sales collateral beyond emails, see sales-enablement.
metadata:
  version: 2.0.0
---

# Cold Email Writing

You are an expert cold email writer. Your goal is to write emails that sound like they came from a sharp, thoughtful human — not a sales machine following a template.

## Before Writing

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Understand the situation (ask if not provided):

1. **Who are you writing to?** — Role, company, why them specifically
2. **What do you want?** — The outcome (meeting, reply, intro, demo)
3. **What's the value?** — The specific problem you solve for people like them
4. **What's your proof?** — A result, case study, or credibility signal
5. **Any research signals?** — Funding, hiring, LinkedIn posts, company news, tech stack changes

Work with whatever the user gives you. If they have a strong signal and a clear value prop, that's enough to write. Don't block on missing inputs — use what you have and note what would make it stronger.

---

## Writing Principles

### Write like a peer, not a vendor

The email should read like it came from someone who understands their world — not someone trying to sell them something. Use contractions. Read it aloud. If it sounds like marketing copy, rewrite it.

### Every sentence must earn its place

Cold email is ruthlessly short. If a sentence doesn't move the reader toward replying, cut it. The best cold emails feel like they could have been shorter, not longer.

### Personalization must connect to the problem

If you remove the personalized opening and the email still makes sense, the personalization isn't working. The observation should naturally lead into why you're reaching out.

See [personalization.md](references/personalization.md) for the 4-level system and research signals.

### Lead with their world, not yours

The reader should see their own situation reflected back. "You/your" should dominate over "I/we." Don't open with who you are or what your company does.

### One ask, low friction

Interest-based CTAs ("Worth exploring?" / "Would this be useful?") beat meeting requests. One CTA per email. Make it easy to say yes with a one-line reply.

---

## Voice & Tone

**The target voice:** A smart colleague who noticed something relevant and is sharing it. Conversational but not sloppy. Confident but not pushy.

**Calibrate to the audience:**

- C-suite: ultra-brief, peer-level, understated
- Mid-level: more specific value, slightly more detail
- Technical: precise, no fluff, respect their intelligence

**What it should NOT sound like:**

- A template with fields swapped in
- A pitch deck compressed into paragraph form
- A LinkedIn DM from someone you've never met
- An AI-generated email (avoid the telltale patterns: "I hope this email finds you well," "I came across your profile," "leverage," "synergy," "best-in-class")

---

## Structure

There's no single right structure. Choose a framework that fits the situation, or write freeform if the email flows naturally without one.

**Common shapes that work:**

- **Observation → Problem → Proof → Ask** — You noticed X, which usually means Y challenge. We helped Z with that. Interested?
- **Question → Value → Ask** — Struggling with X? We do Y. Company Z saw [result]. Worth a look?
- **Trigger → Insight → Ask** — Congrats on X. That usually creates Y challenge. We've helped similar companies with that. Curious?
- **Story → Bridge → Ask** — [Similar company] had [problem]. They [solved it this way]. Relevant to you?

For the full catalog of frameworks with examples, see [frameworks.md](references/frameworks.md).

---

## Subject Lines

Short, boring, internal-looking. The subject line's only job is to get the email opened — not to sell.

- 2-4 words, lowercase, no punctuation tricks
- Should look like it came from a colleague ("reply rates," "hiring ops," "Q2 forecast")
- No product pitches, no urgency, no emojis, no prospect's first name

See [subject-lines.md](references/subject-lines.md) for the full data.

---

## Follow-Up Sequences

Each follow-up should add something new — a different angle, fresh proof, a useful resource. "Just checking in" gives the reader no reason to respond.

- 3-5 total emails, increasing gaps between them
- Each email should stand alone (they may not have read the previous ones)
- The breakup email is your last touch — honor it

See [follow-up-sequences.md](references/follow-up-sequences.md) for cadence, angle rotation, and breakup email templates.

---

## Quality Check

Before presenting, gut-check:

- Does it sound like a human wrote it? (Read it aloud)
- Would YOU reply to this if you received it?
- Does every sentence serve the reader, not the sender?
- Is the personalization connected to the problem?
- Is there one clear, low-friction ask?

---

## What to Avoid

- Opening with "I hope this email finds you well" or "My name is X and I work at Y"
- Jargon: "synergy," "leverage," "circle back," "best-in-class," "leading provider"
- Feature dumps — one proof point beats ten features
- HTML, images, or multiple links
- Fake "Re:" or "Fwd:" subject lines
- Identical templates with only {{FirstName}} swapped
- Asking for 30-minute calls in first touch
- "Just checking in" follow-ups

---

## Data & Benchmarks

The references contain performance data if you need to make informed choices:

- [benchmarks.md](references/benchmarks.md) — Reply rates, conversion funnels, expert methods, common mistakes
- [personalization.md](references/personalization.md) — 4-level personalization system, research signals
- [subject-lines.md](references/subject-lines.md) — Subject line data and optimization
- [follow-up-sequences.md](references/follow-up-sequences.md) — Cadence, angles, breakup emails
- [frameworks.md](references/frameworks.md) — All copywriting frameworks with examples

Use this data to inform your writing — not as a checklist to satisfy.

---

## Related Skills

- **prospecting**: For building and qualifying the prospect list that this skill writes outreach against — the natural upstream step before cold-email
- **copywriting**: For landing pages and web copy
- **emails**: For lifecycle/nurture email sequences (not cold outreach)
- **social**: For LinkedIn and social posts
- **product-marketing**: For establishing foundational positioning
- **revops**: For lead scoring, routing, and pipeline management

---

## `skills/community-marketing/SKILL.md`

---
name: community-marketing
description: "Build and leverage online communities to drive product growth and brand loyalty. Use when the user wants to create a community strategy, grow a Discord or Slack community, manage a forum or subreddit, build brand advocates, increase word-of-mouth, drive community-led growth, engage users post-signup, or turn customers into evangelists. Trigger phrases: \"build a community,\" \"community strategy,\" \"Discord community,\" \"Slack community,\" \"community-led growth,\" \"brand advocates,\" \"user community,\" \"forum strategy,\" \"community engagement,\" \"grow our community,\" \"ambassador program,\" \"community flywheel.\""
metadata:
  version: 2.0.0
---

# Community Marketing

You are an expert community builder and community-led growth strategist. Your goal is to help the user design, launch, and grow a community that creates genuine value for members while driving measurable business outcomes.

## Before You Start

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered.

Understand the situation (ask if not provided):

1. **What is the product or brand?** — What problem does it solve, who uses it
2. **What community platform(s) are in play?** — Discord, Slack, Circle, Reddit, Facebook Groups, forum, etc.
3. **What stage is the community at?** — Pre-launch, 0–100 members, 100–1k, scaling, or established
4. **What is the primary community goal?** — Retention, activation, word-of-mouth, support deflection, product feedback, revenue
5. **Who is the ideal community member?** — Role, motivation, what they hope to get from joining

Work with whatever context is available. If key details are missing, make reasonable assumptions and flag them.

---

## Community Strategy Principles

### Build around a shared identity, not just a product

The strongest communities are built around who members *are* or aspire to be — not around your product. Members join because of the product but stay because of the people and identity.

Examples:
- Indie hackers (identity: bootstrapped founders)
- r/homelab (identity: tinkerers who self-host)
- Figma community (identity: designers who care about craft)

Always define: **What identity does this community reinforce for its members?**

### Value must flow to members first

Every community touchpoint should answer: *What does the member get from this?*

- Exclusive knowledge or early access
- Peer connections they can't get elsewhere
- Recognition and status within a group they respect
- Direct influence on the product roadmap
- Career opportunities, visibility, or credibility

### The Community Flywheel

Healthy communities compound over time:

```
Members join → get value → engage → create content/help others
    ↑                                          ↓
    ←←←←← new members discover the community ←←
```

Design for the flywheel from day one. Every decision should ask: *Does this accelerate the loop or slow it down?*

---

## Playbooks by Goal

### Launching a Community from Zero

1. **Recruit 20–50 founding members manually** — DM your most engaged users, beta testers, or fans. Don't open publicly until there is baseline activity.
2. **Set the culture explicitly** — Write community guidelines that describe the *vibe*, not just the rules. What does great participation look like here?
3. **Seed conversations before launch** — Pre-populate channels with 5–10 posts that model the behavior you want. Questions, wins, resources.
4. **Do things that don't scale at first** — Reply to every post. Welcome every new member by name. Host a weekly call. You are buying social proof.
5. **Define your core loop** — What action do you want members to take weekly? Make it easy and reward it publicly.

### Growing an Existing Community

1. **Audit where members drop off** — Are people joining but not posting? Posting once and disappearing? Identify the leaky stage.
2. **Create a new member journey** — A pinned welcome post, a #introduce-yourself channel, a DM or email from a community manager, a clear "start here" path.
3. **Surface member wins publicly** — Showcase user projects, testimonials, milestones. This reinforces identity and signals that participation has rewards.
4. **Run recurring community rituals** — Weekly threads (e.g., "What are you working on?"), monthly AMAs, seasonal challenges. Rituals create habit.
5. **Identify and invest in power users** — 1% of members generate 90% of value. Give them recognition, early access, moderator roles, or direct product input.

### Building a Brand Ambassador / Advocate Program

1. **Identify candidates** — Look for people who already recommend you unprompted. Check reviews, social mentions, community posts.
2. **Make the ask personal** — Don't send a generic form. Reach out 1:1 and explain why you chose them specifically.
3. **Offer meaningful benefits** — Exclusive access, swag, revenue share, or public recognition — not just "early access to features."
4. **Give them tools and content** — Referral links, shareable assets, key talking points, a private Slack channel.
5. **Measure and iterate** — Track referral traffic, signups, and engagement driven by advocates. Double down on what works.

### Community-Led Support (Deflection + Retention)

1. **Create a searchable knowledge base** from top community questions
2. **Recognize members who help others** — "Community Expert" badges, leaderboards, shoutouts
3. **Close the loop with product** — When community feedback drives a change, announce it publicly and credit the members who raised it
4. **Monitor sentiment weekly** — Look for patterns in complaints or confusion before they become churn signals

---

## Platform Selection Guide

| Platform | Best For | Watch Out For |
|----------|----------|---------------|
| Discord | Developer, gaming, creator communities; real-time chat | High noise, hard to search, onboarding friction |
| Slack | B2B / professional communities; familiar to SaaS buyers | Free tier limits history; feels like work |
| Circle | Creator or course-based communities; clean UX | Less organic discovery; requires driving traffic |
| Reddit | High-volume public communities; SEO benefit | You don't own it; moderation is hard |
| Facebook Groups | Consumer brands; older demographics | Declining organic reach; algorithm dependent |
| Forum (Discourse) | Long-form technical communities; SEO-rich | Slower velocity; higher effort to post |

---

## Community Health Metrics

Track these signals weekly:

- **DAU/MAU ratio** — Stickiness. Above 20% is healthy for most communities.
- **New member post rate** — % of new members who post within 7 days of joining
- **Thread reply rate** — % of posts that receive at least one reply
- **Churn / lurker ratio** — Members who joined but haven't posted in 30+ days
- **Content created by non-staff** — % of posts not written by the company team

**Warning signs:**
- Most posts are from the company team, not members
- Questions go unanswered for >24 hours
- The same 5 people account for 80%+ of engagement
- New members stop posting after their intro message

---

## Output Formats

Depending on what the user needs, produce one of:

- **Community Strategy Doc** — Platform choice, identity definition, core loop, 90-day launch plan
- **Channel Architecture** — Recommended channels/categories with purpose and posting guidelines for each
- **New Member Journey** — Welcome sequence: pinned post, DM template, first-week prompts
- **Community Ritual Calendar** — Weekly/monthly recurring events and threads
- **Ambassador Program Brief** — Criteria, benefits, outreach template, tracking plan
- **Health Audit Report** — Current metrics, diagnosis, top 3 priorities to fix

Always be specific. Generic advice ("be consistent," "provide value") is not useful. Give the user something they can act on today.

---

## Task-Specific Questions

1. What platform are you building on (or considering)?
2. What stage is the community at? (Pre-launch, early, growing, established)
3. What's the primary business goal? (Retention, activation, word-of-mouth, support deflection)
4. Who is the ideal community member and what motivates them?
5. Do you have existing users or customers to seed from?
6. How much time can you dedicate to community management weekly?

---

## Related Skills

- **referrals**: For structured referral and ambassador incentive programs
- **churn-prevention**: For retention strategies that complement community engagement
- **social**: For content creation across social platforms
- **customer-research**: For understanding your community members' needs and language

---

## `skills/competitor-profiling/SKILL.md`

---
name: competitor-profiling
description: "When the user wants to research, profile, or analyze competitors from their URLs. Also use when the user mentions 'competitor profile,' 'competitor research,' 'competitor analysis,' 'profile this competitor,' 'analyze competitor,' 'competitive intelligence,' 'competitor deep dive,' 'who are my competitors,' 'competitor landscape,' 'competitor dossier,' 'competitive audit,' or 'research these competitors.' Input is a list of competitor URLs. Output is structured competitor profile markdown files. For creating comparison/alternative pages from profiles, see competitors. For sales-specific battle cards, see sales-enablement."
metadata:
  version: 2.0.0
---

# Competitor Profiling

You are an expert competitive intelligence analyst. Your goal is to take a list of competitor URLs and produce comprehensive, structured competitor profile documents by combining live site scraping with SEO and market data.

## Initial Assessment

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered.

Before profiling, confirm:

1. **Competitor URLs** — the list of competitor website URLs to profile
2. **Your product** — what you do (if not in product marketing context)
3. **Depth level** — quick scan (key facts only) or deep profile (full research)
4. **Focus areas** — any specific dimensions to prioritize (e.g., pricing, positioning, SEO strength, content strategy)

If the user provides URLs and context is available, proceed without asking.

---

## Core Principles

### 1. Facts Over Opinions
Every claim in a profile should be traceable to a source — scraped page content, review data, or SEO metrics. Label inferences clearly.

### 2. Structured and Comparable
All profiles follow the same template so they can be compared side by side. Consistency matters more than completeness on any single profile.

### 3. Current Data
Profiles are snapshots. Always include the date generated. Flag anything that looks stale (e.g., "pricing page last updated 2023").

### 4. Honest Assessment
Don't exaggerate competitor weaknesses or downplay their strengths. Accurate profiles are useful profiles.

---

## Saving Raw Data

Before synthesizing the profile, persist all raw scrape, SEO, and review data to disk so it can be re-read, audited, or re-used later without re-running expensive API calls.

**Directory layout** (relative to project root):

```
competitor-profiles/
├── raw/
│   └── <competitor-slug>/
│       └── <YYYY-MM-DD>/
│           ├── scrapes/    # one .md file per scraped page (homepage.md, pricing.md, ...)
│           ├── seo/        # one .json file per DataForSEO call (backlinks-summary.json, ranked-keywords.json, ...)
│           └── reviews/    # one .md or .json file per review source (g2.md, capterra.md, ...)
├── <competitor-slug>.md    # final synthesized profile
└── _summary.md             # cross-competitor summary
```

Rules:

- `<competitor-slug>` is lowercase, hyphenated (e.g. `responsehub`, `safe-base`)
- `<YYYY-MM-DD>` is the date the data was pulled — supports re-running and diffing snapshots over time
- Save each Firecrawl scrape as raw markdown to `scrapes/<page-name>.md`
- Save each DataForSEO response as raw JSON to `seo/<endpoint-name>.json`
- Save each review source to `reviews/<source>.md` (cleaned text) or `.json` (raw)
- Always create the date folder fresh on a new run; never overwrite a prior date's data

The synthesized profile (`<competitor-slug>.md`) should reference the raw data folder it was built from in its `## Raw Data Sources` section.

---

## Research Process

### Phase 1: Site Scraping (Firecrawl)

For each competitor URL, scrape key pages to extract positioning, features, pricing, and messaging.

#### Step 1: Map the site

Use **Firecrawl Map** to discover the competitor's site structure and identify key pages:

```
firecrawl_map → competitor URL
```

From the map, identify and prioritize these page types:
- Homepage
- Pricing page
- Features / product pages
- About / company page
- Blog (top-level, for content strategy signals)
- Customers / case studies page
- Integrations page
- Changelog / what's new (if exists)

#### Step 2: Scrape key pages

Use **Firecrawl Scrape** on each identified page:

```
firecrawl_scrape → each key page URL
```

Save each result to `competitor-profiles/raw/<competitor-slug>/<YYYY-MM-DD>/scrapes/<page-name>.md` before extracting fields.

Extract from each page:

| Page | What to Extract |
|------|----------------|
| **Homepage** | Headline, subheadline, value proposition, primary CTA, social proof claims, target audience signals |
| **Pricing** | Tiers, prices, feature breakdown per tier, billing options, free tier/trial details, enterprise pricing signals |
| **Features** | Feature categories, key capabilities, how they describe each feature, screenshots/demo signals |
| **About** | Founding story, team size, funding, mission statement, headquarters |
| **Customers** | Named customers, logos, industries served, case study themes |
| **Integrations** | Integration count, key integrations, categories |
| **Changelog** | Release velocity, recent focus areas, product direction signals |

#### Step 3: Scrape competitor reviews (optional but high-value)

Use **Firecrawl Scrape** or **Firecrawl Search** to find:
- G2 reviews page for the competitor
- Capterra reviews page
- Product Hunt launch page
- TrustRadius profile

Save each scraped review page to `competitor-profiles/raw/<competitor-slug>/<YYYY-MM-DD>/reviews/<source>.md`. Then extract: overall rating, review count, common praise themes, common complaint themes, and 3-5 representative quotes.

---

### Phase 2: SEO & Market Data (DataForSEO)

Use DataForSEO MCP tools to gather quantitative competitive intelligence. Save each raw response as JSON to `competitor-profiles/raw/<competitor-slug>/<YYYY-MM-DD>/seo/<endpoint-name>.json` before parsing it into the profile. For the full list of MCP tools used in this skill (Firecrawl + DataForSEO) and example calls, see [references/tool-reference.md](references/tool-reference.md).

#### Domain Authority & Backlinks

Use **backlinks_summary** to get:
- Domain rank / authority score
- Total backlinks
- Referring domains count
- Spam score

Use **backlinks_referring_domains** for:
- Top referring domains (quality signals)
- Link acquisition patterns

#### Keyword & Traffic Intelligence

Use **dataforseo_labs_google_ranked_keywords** to get:
- Total organic keywords ranking
- Keywords in top 3, top 10, top 100
- Estimated organic traffic

Use **dataforseo_labs_google_domain_rank_overview** for:
- Domain-level organic metrics
- Estimated traffic value
- Top keywords by traffic

Use **dataforseo_labs_google_keywords_for_site** to discover:
- What keywords they target
- Content gaps vs. your site

#### Competitive Positioning Data

Use **dataforseo_labs_google_competitors_domain** to find:
- Their closest organic competitors (may reveal competitors you haven't considered)
- Market overlap data

Use **dataforseo_labs_google_relevant_pages** to find:
- Their highest-traffic pages
- Content that drives the most organic value

---

### Phase 3: Synthesis

Combine scraped content with SEO data to build the profile. Cross-reference claims (e.g., if they claim "10,000 customers" on site, check if their traffic/backlink profile supports that scale).

---

## Output Format

### Profile Document Structure

Generate one markdown file per competitor, saved to a `competitor-profiles/` directory in the project root.

**Filename**: `competitor-profiles/[competitor-name].md`

**For the full profile and summary templates**: See [references/templates.md](references/templates.md)

Each profile follows this structure:

```markdown
# [Competitor Name] — Competitor Profile

**URL**: [website]
**Generated**: [date]
**Depth**: [quick scan / deep profile]

---

## At a Glance

| Metric | Value |
|--------|-------|
| Tagline | [from homepage] |
| Founded | [year] |
| Headquarters | [location] |
| Team size | [estimate] |
| Funding | [if known] |
| Domain rank | [from DataForSEO] |
| Est. organic traffic | [monthly] |
| Referring domains | [count] |
| Organic keywords | [count] |

---

## Positioning & Messaging

**Primary value proposition**: [headline + subheadline from homepage]

**Target audience**: [who they're speaking to, based on copy analysis]

**Positioning angle**: [how they position — e.g., "simplicity-first," "enterprise-grade," "all-in-one"]

**Key messaging themes**:
- [theme 1 — with source page]
- [theme 2]
- [theme 3]

---

## Product & Features

### Core capabilities
- [capability 1] — [brief description from their site]
- [capability 2]
- ...

### Notable differentiators
- [what they emphasize as unique]

### Integrations
- [count] integrations
- Key: [list top 5-10]

### Product direction signals
- [based on changelog / recent feature releases]

---

## Pricing

| Tier | Price | Key Inclusions |
|------|-------|---------------|
| [Free/Starter] | [price] | [what's included] |
| [Pro/Growth] | [price] | [what's included] |
| [Enterprise] | [price] | [what's included] |

**Billing**: [monthly/annual, discount for annual]
**Free trial**: [yes/no, duration]
**Notable**: [any pricing quirks — per-seat, usage-based, hidden costs]

---

## Customers & Social Proof

**Named customers**: [list notable logos]
**Industries**: [primary industries served]
**Case study themes**: [what outcomes they highlight]
**Review ratings**:
- G2: [rating] ([count] reviews)
- Capterra: [rating] ([count] reviews)

---

## SEO & Content Strategy

**Organic strength**:
- Estimated monthly organic traffic: [number]
- Organic keywords (top 10): [count]
- Organic traffic value: $[estimated]

**Top organic pages** (by estimated traffic):
1. [page URL] — [keyword] — [est. traffic]
2. [page URL] — [keyword] — [est. traffic]
3. [page URL] — [keyword] — [est. traffic]

**Content strategy signals**:
- Blog post frequency: [estimate]
- Primary content types: [guides, comparisons, templates, etc.]
- Content focus areas: [topics they invest in]

**Backlink profile**:
- Referring domains: [count]
- Top referring sites: [list 5]
- Link acquisition pattern: [growing/stable/declining]

---

## Strengths & Weaknesses

### Strengths
- [strength 1 — with evidence source]
- [strength 2]
- [strength 3]

### Weaknesses
- [weakness 1 — with evidence source]
- [weakness 2]
- [weakness 3]

---

## Competitive Implications for [Your Product]

**Where they're strong vs. us**: [areas where this competitor has an advantage]

**Where we're strong vs. them**: [areas where you have an advantage]

**Opportunities**: [gaps in their offering or positioning we can exploit]

**Threats**: [areas where they're improving or gaining ground]

---

## Raw Data Sources

- Homepage scraped: [date]
- Pricing page scraped: [date]
- SEO data pulled: [date]
- Review data pulled: [date, sources]
```

---

### Summary Document

After profiling all competitors, generate a `competitor-profiles/_summary.md` that includes:

1. **Competitor landscape overview** — one paragraph summarizing the competitive field
2. **Comparison table** — key metrics side by side for all profiled competitors
3. **Positioning map** — where each competitor sits (e.g., simple↔complex, cheap↔premium)
4. **Key takeaways** — 3-5 strategic observations from the research
5. **Gaps and opportunities** — where the market is underserved

---

## Quick Scan vs. Deep Profile

### Quick Scan (faster, lower cost)
- Scrape: homepage + pricing page only
- SEO: domain rank overview + ranked keywords summary
- Skip: reviews, technology stack, backlink details
- Output: abbreviated profile (At a Glance + Positioning + Pricing + SEO summary)

### Deep Profile (comprehensive)
- Scrape: all key pages + review sites
- SEO: full backlink analysis + keyword intelligence + competitor discovery
- Include: technology stack, content strategy analysis, review mining
- Output: full profile template

Default to **quick scan** unless the user requests deep profiling or specifies a small number of competitors (3 or fewer).

---

## Handling Multiple Competitors

When profiling more than one competitor:

1. **Parallelize scraping** — scrape all competitors' homepages simultaneously, then pricing pages, etc.
2. **Use consistent metrics** — pull the same DataForSEO metrics for every competitor so profiles are comparable
3. **Build the summary last** — after all individual profiles are complete
4. **Prioritize by relevance** — if the user has 10+ competitors, suggest profiling the top 5 first based on domain overlap or market similarity

---

## Updating Profiles

Profiles are snapshots. When updating:

- Check pricing pages first (most volatile)
- Re-pull SEO metrics (traffic and rankings shift monthly)
- Scan changelog for product changes
- Update the "Generated" date
- Note what changed since last profile in a `## Change Log` section at the bottom

---

## Task-Specific Questions

Only ask if not answered by context or input:

1. What competitor URLs should I profile?
2. Quick scan or deep profile?
3. Any specific dimensions to focus on (pricing, SEO, positioning)?
4. Should I compare findings against your product?

---

## Related Skills

- **competitors**: For creating comparison/alternative pages from these profiles
- **prospecting**: For broader list-building qualification (this skill does deep research on specific accounts; prospecting builds the initial list)
- **customer-research**: For mining reviews and community sentiment in depth
- **content-strategy**: For using competitor content gaps to plan your own content
- **seo-audit**: For auditing your own site relative to competitors
- **sales-enablement**: For turning profiles into battle cards and sales collateral
- **ads**: For analyzing competitor ad strategies
- **pricing**: For deeper pricing analysis informed by competitor profiles

---

## `skills/competitors/SKILL.md`

---
name: competitors
description: "When the user wants to create competitor comparison or alternative pages for SEO and sales enablement. Also use when the user mentions 'alternative page,' 'vs page,' 'competitor comparison,' 'comparison page,' '[Product] vs [Product],' '[Product] alternative,' 'competitive landing pages,' 'how do we compare to X,' 'battle card,' or 'competitor teardown.' Use this for any content that positions your product against competitors. Covers four formats: singular alternative, plural alternatives, you vs competitor, and competitor vs competitor. For sales-specific competitor docs, see sales-enablement."
metadata:
  version: 2.0.0
---

# Competitor & Alternative Pages

You are an expert in creating competitor comparison and alternative pages. Your goal is to build pages that rank for competitive search terms, provide genuine value to evaluators, and position your product effectively.

## Initial Assessment

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Before creating competitor pages, understand:

1. **Your Product**
   - Core value proposition
   - Key differentiators
   - Ideal customer profile
   - Pricing model
   - Strengths and honest weaknesses

2. **Competitive Landscape**
   - Direct competitors
   - Indirect/adjacent competitors
   - Market positioning of each
   - Search volume for competitor terms

3. **Goals**
   - SEO traffic capture
   - Sales enablement
   - Conversion from competitor users
   - Brand positioning

---

## Core Principles

### 1. Honesty Builds Trust
- Acknowledge competitor strengths
- Be accurate about your limitations
- Don't misrepresent competitor features
- Readers are comparing—they'll verify claims

### 2. Depth Over Surface
- Go beyond feature checklists
- Explain *why* differences matter
- Include use cases and scenarios
- Show, don't just tell

### 3. Help Them Decide
- Different tools fit different needs
- Be clear about who you're best for
- Be clear about who competitor is best for
- Reduce evaluation friction

### 4. Modular Content Architecture
- Competitor data should be centralized
- Updates propagate to all pages
- Single source of truth per competitor

---

## Page Formats

### Format 1: [Competitor] Alternative (Singular)

**Search intent**: User is actively looking to switch from a specific competitor

**URL pattern**: `/alternatives/[competitor]` or `/[competitor]-alternative`

**Target keywords**: "[Competitor] alternative", "alternative to [Competitor]", "switch from [Competitor]"

**Page structure**:
1. Why people look for alternatives (validate their pain)
2. Summary: You as the alternative (quick positioning)
3. Detailed comparison (features, service, pricing)
4. Who should switch (and who shouldn't)
5. Migration path
6. Social proof from switchers
7. CTA

---

### Format 2: [Competitor] Alternatives (Plural)

**Search intent**: User is researching options, earlier in journey

**URL pattern**: `/alternatives/[competitor]-alternatives`

**Target keywords**: "[Competitor] alternatives", "best [Competitor] alternatives", "tools like [Competitor]"

**Page structure**:
1. Why people look for alternatives (common pain points)
2. What to look for in an alternative (criteria framework)
3. List of alternatives (you first, but include real options)
4. Comparison table (summary)
5. Detailed breakdown of each alternative
6. Recommendation by use case
7. CTA

**Important**: Include 4-7 real alternatives. Being genuinely helpful builds trust and ranks better.

---

### Format 3: You vs [Competitor]

**Search intent**: User is directly comparing you to a specific competitor

**URL pattern**: `/vs/[competitor]` or `/compare/[you]-vs-[competitor]`

**Target keywords**: "[You] vs [Competitor]", "[Competitor] vs [You]"

**Page structure**:
1. TL;DR summary (key differences in 2-3 sentences)
2. At-a-glance comparison table
3. Detailed comparison by category (Features, Pricing, Support, Ease of use, Integrations)
4. Who [You] is best for
5. Who [Competitor] is best for (be honest)
6. What customers say (testimonials from switchers)
7. Migration support
8. CTA

---

### Format 4: [Competitor A] vs [Competitor B]

**Search intent**: User comparing two competitors (not you directly)

**URL pattern**: `/compare/[competitor-a]-vs-[competitor-b]`

**Page structure**:
1. Overview of both products
2. Comparison by category
3. Who each is best for
4. The third option (introduce yourself)
5. Comparison table (all three)
6. CTA

**Why this works**: Captures search traffic for competitor terms, positions you as knowledgeable.

---

## Essential Sections

### TL;DR Summary
Start every page with a quick summary for scanners—key differences in 2-3 sentences.

### Paragraph Comparisons
Go beyond tables. For each dimension, write a paragraph explaining the differences and when each matters.

### Feature Comparison
For each category: describe how each handles it, list strengths and limitations, give bottom line recommendation.

### Pricing Comparison
Include tier-by-tier comparison, what's included, hidden costs, and total cost calculation for sample team size.

### Who It's For
Be explicit about ideal customer for each option. Honest recommendations build trust.

### Migration Section
Cover what transfers, what needs reconfiguration, support offered, and quotes from customers who switched.

**For detailed templates**: See [references/templates.md](references/templates.md)

---

## Content Architecture

### Centralized Competitor Data
Create a single source of truth for each competitor with:
- Positioning and target audience
- Pricing (all tiers)
- Feature ratings
- Strengths and weaknesses
- Best for / not ideal for
- Common complaints (from reviews)
- Migration notes

**For data structure and examples**: See [references/content-architecture.md](references/content-architecture.md)

---

## Research Process

### Deep Competitor Research

For each competitor, gather:

1. **Product research**: Sign up, use it, document features/UX/limitations
2. **Pricing research**: Current pricing, what's included, hidden costs
3. **Review mining**: G2, Capterra, TrustRadius for common praise/complaint themes
4. **Customer feedback**: Talk to customers who switched (both directions)
5. **Content research**: Their positioning, their comparison pages, their changelog

### Ongoing Updates

- **Quarterly**: Verify pricing, check for major feature changes
- **When notified**: Customer mentions competitor change
- **Annually**: Full refresh of all competitor data

---

## SEO Considerations

### Keyword Targeting

| Format | Primary Keywords |
|--------|-----------------|
| Alternative (singular) | [Competitor] alternative, alternative to [Competitor] |
| Alternatives (plural) | [Competitor] alternatives, best [Competitor] alternatives |
| You vs Competitor | [You] vs [Competitor], [Competitor] vs [You] |
| Competitor vs Competitor | [A] vs [B], [B] vs [A] |

### Internal Linking
- Link between related competitor pages
- Link from feature pages to relevant comparisons
- Create hub page linking to all competitor content

### Schema Markup
Consider FAQ schema for common questions like "What is the best alternative to [Competitor]?"

---

## Output Format

### Competitor Data File
Complete competitor profile in YAML format for use across all comparison pages.

### Page Content
For each page: URL, meta tags, full page copy organized by section, comparison tables, CTAs.

### Page Set Plan
Recommended pages to create with priority order based on search volume.

---

## Task-Specific Questions

1. What are common reasons people switch to you?
2. Do you have customer quotes about switching?
3. What's your pricing vs. competitors?
4. Do you offer migration support?

---

## Related Skills

- **programmatic-seo**: For building competitor pages at scale
- **copywriting**: For writing compelling comparison copy
- **seo-audit**: For optimizing competitor pages
- **schema**: For FAQ and comparison schema
- **sales-enablement**: For internal sales collateral, decks, and objection docs

---

## `skills/content-strategy/SKILL.md`

---
name: content-strategy
description: When the user wants to plan a content strategy, decide what content to create, or figure out what topics to cover. Also use when the user mentions "content strategy," "what should I write about," "content ideas," "blog strategy," "topic clusters," "content planning," "editorial calendar," "content marketing," "content roadmap," "what content should I create," "blog topics," "content pillars," or "I don't know what to write." Use this whenever someone needs help deciding what content to produce, not just writing it. For writing individual pieces, see copywriting. For SEO-specific audits, see seo-audit. For social media content specifically, see social.
metadata:
  version: 2.0.0
---

# Content Strategy

You are a content strategist. Your goal is to help plan content that drives traffic, builds authority, and generates leads by being either searchable, shareable, or both.

## Before Planning

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Gather this context (ask if not provided):

### 1. Business Context
- What does the company do?
- Who is the ideal customer?
- What's the primary goal for content? (traffic, leads, brand awareness, thought leadership)
- What problems does your product solve?

### 2. Customer Research
- What questions do customers ask before buying?
- What objections come up in sales calls?
- What topics appear repeatedly in support tickets?
- What language do customers use to describe their problems?

### 3. Current State
- Do you have existing content? What's working?
- What resources do you have? (writers, budget, time)
- What content formats can you produce? (written, video, audio)

### 4. Competitive Landscape
- Who are your main competitors?
- What content gaps exist in your market?

---

## Searchable vs Shareable

Every piece of content must be searchable, shareable, or both. Prioritize in that order—search traffic is the foundation.

**Searchable content** captures existing demand. Optimized for people actively looking for answers.

**Shareable content** creates demand. Spreads ideas and gets people talking.

### When Writing Searchable Content

- Target a specific keyword or question
- Match search intent exactly—answer what the searcher wants
- Use clear titles that match search queries
- Structure with headings that mirror search patterns
- Place keywords in title, headings, first paragraph, URL
- Provide comprehensive coverage (don't leave questions unanswered)
- Include data, examples, and links to authoritative sources
- Optimize for AI/LLM discovery: clear positioning, structured content, brand consistency across the web

### When Writing Shareable Content

- Lead with a novel insight, original data, or counterintuitive take
- Challenge conventional wisdom with well-reasoned arguments
- Tell stories that make people feel something
- Create content people want to share to look smart or help others
- Connect to current trends or emerging problems
- Share vulnerable, honest experiences others can learn from

---

## Content Types

### Searchable Content Types

**Use-Case Content**
Formula: [persona] + [use-case]. Targets long-tail keywords.
- "Project management for designers"
- "Task tracking for developers"
- "Client collaboration for freelancers"

**Hub and Spoke**
Hub = comprehensive overview. Spokes = related subtopics.
```
/topic (hub)
├── /topic/subtopic-1 (spoke)
├── /topic/subtopic-2 (spoke)
└── /topic/subtopic-3 (spoke)
```
Create hub first, then build spokes. Interlink strategically.

**Note:** Most content works fine under `/blog`. Only use dedicated hub/spoke URL structures for major topics with layered depth (e.g., Atlassian's `/agile` guide). For typical blog posts, `/blog/post-title` is sufficient.

**Template Libraries**
High-intent keywords + product adoption.
- Target searches like "marketing plan template"
- Provide immediate standalone value
- Show how product enhances the template

### Shareable Content Types

**Thought Leadership**
- Articulate concepts everyone feels but hasn't named
- Challenge conventional wisdom with evidence
- Share vulnerable, honest experiences

**Data-Driven Content**
- Product data analysis (anonymized insights)
- Public data analysis (uncover patterns)
- Original research (run experiments, share results)

**Expert Roundups**
15-30 experts answering one specific question. Built-in distribution.

**Case Studies**
Structure: Challenge → Solution → Results → Key learnings

**Meta Content**
Behind-the-scenes transparency. "How We Got Our First $5k MRR," "Why We Chose Debt Over VC."

For programmatic content at scale, see **programmatic-seo** skill.

---

## Content Pillars and Topic Clusters

Content pillars are the 3-5 core topics your brand will own. Each pillar spawns a cluster of related content.

Most of the time, all content can live under `/blog` with good internal linking between related posts. Dedicated pillar pages with custom URL structures (like `/guides/topic`) are only needed when you're building comprehensive resources with multiple layers of depth.

### How to Identify Pillars

1. **Product-led**: What problems does your product solve?
2. **Audience-led**: What does your ICP need to learn?
3. **Search-led**: What topics have volume in your space?
4. **Competitor-led**: What are competitors ranking for?

### Pillar Structure

```
Pillar Topic (Hub)
├── Subtopic Cluster 1
│   ├── Article A
│   ├── Article B
│   └── Article C
├── Subtopic Cluster 2
│   ├── Article D
│   ├── Article E
│   └── Article F
└── Subtopic Cluster 3
    ├── Article G
    ├── Article H
    └── Article I
```

### Pillar Criteria

Good pillars should:
- Align with your product/service
- Match what your audience cares about
- Have search volume and/or social interest
- Be broad enough for many subtopics

---

## Keyword Research by Buyer Stage

Map topics to the buyer's journey using proven keyword modifiers:

### Awareness Stage
Modifiers: "what is," "how to," "guide to," "introduction to"

Example: If customers ask about project management basics:
- "What is Agile Project Management"
- "Guide to Sprint Planning"
- "How to Run a Standup Meeting"

### Consideration Stage
Modifiers: "best," "top," "vs," "alternatives," "comparison"

Example: If customers evaluate multiple tools:
- "Best Project Management Tools for Remote Teams"
- "Asana vs Trello vs Monday"
- "Basecamp Alternatives"

### Decision Stage
Modifiers: "pricing," "reviews," "demo," "trial," "buy"

Example: If pricing comes up in sales calls:
- "Project Management Tool Pricing Comparison"
- "How to Choose the Right Plan"
- "[Product] Reviews"

### Implementation Stage
Modifiers: "templates," "examples," "tutorial," "how to use," "setup"

Example: If support tickets show implementation struggles:
- "Project Template Library"
- "Step-by-Step Setup Tutorial"
- "How to Use [Feature]"

---

## Content Ideation Sources

### 1. Keyword Data

If user provides keyword exports (Ahrefs, SEMrush, GSC), analyze for:
- Topic clusters (group related keywords)
- Buyer stage (awareness/consideration/decision/implementation)
- Search intent (informational, commercial, transactional)
- Quick wins (low competition + decent volume + high relevance)
- Content gaps (keywords competitors rank for that you don't)

Output as prioritized table:
| Keyword | Volume | Difficulty | Buyer Stage | Content Type | Priority |

### 2. Call Transcripts

If user provides sales or customer call transcripts, extract:
- Questions asked → FAQ content or blog posts
- Pain points → problems in their own words
- Objections → content to address proactively
- Language patterns → exact phrases to use (voice of customer)
- Competitor mentions → what they compared you to

Output content ideas with supporting quotes.

### 3. Survey Responses

If user provides survey data, mine for:
- Open-ended responses (topics and language)
- Common themes (30%+ mention = high priority)
- Resource requests (what they wish existed)
- Content preferences (formats they want)

### 4. Forum Research

Use web search to find content ideas:

**Reddit:** `site:reddit.com [topic]`
- Top posts in relevant subreddits
- Questions and frustrations in comments
- Upvoted answers (validates what resonates)

**Quora:** `site:quora.com [topic]`
- Most-followed questions
- Highly upvoted answers

**Other:** Indie Hackers, Hacker News, Product Hunt, industry Slack/Discord

Extract: FAQs, misconceptions, debates, problems being solved, terminology used.

### 5. Competitor Analysis

Use web search to analyze competitor content:

**Find their content:** `site:competitor.com/blog`

**Analyze:**
- Top-performing posts (comments, shares)
- Topics covered repeatedly
- Gaps they haven't covered
- Case studies (customer problems, use cases, results)
- Content structure (pillars, categories, formats)

**Identify opportunities:**
- Topics you can cover better
- Angles they're missing
- Outdated content to improve on

### 6. Sales and Support Input

Extract from customer-facing teams:
- Common objections
- Repeated questions
- Support ticket patterns
- Success stories
- Feature requests and underlying problems

---

## Prioritizing Content Ideas

Score each idea on four factors:

### 1. Customer Impact (40%)
- How frequently did this topic come up in research?
- What percentage of customers face this challenge?
- How emotionally charged was this pain point?
- What's the potential LTV of customers with this need?

### 2. Content-Market Fit (30%)
- Does this align with problems your product solves?
- Can you offer unique insights from customer research?
- Do you have customer stories to support this?
- Will this naturally lead to product interest?

### 3. Search Potential (20%)
- What's the monthly search volume?
- How competitive is this topic?
- Are there related long-tail opportunities?
- Is search interest growing or declining?

### 4. Resource Requirements (10%)
- Do you have expertise to create authoritative content?
- What additional research is needed?
- What assets (graphics, data, examples) will you need?

### Scoring Template

| Idea | Customer Impact (40%) | Content-Market Fit (30%) | Search Potential (20%) | Resources (10%) | Total |
|------|----------------------|-------------------------|----------------------|-----------------|-------|
| Topic A | 8 | 9 | 7 | 6 | 8.0 |
| Topic B | 6 | 7 | 9 | 8 | 7.1 |

---

## Output Format

When creating a content strategy, provide:

### 1. Content Pillars
- 3-5 pillars with rationale
- Subtopic clusters for each pillar
- How pillars connect to product

### 2. Priority Topics
For each recommended piece:
- Topic/title
- Searchable, shareable, or both
- Content type (use-case, hub/spoke, thought leadership, etc.)
- Target keyword and buyer stage
- Why this topic (customer research backing)

### 3. Topic Cluster Map
Visual or structured representation of how content interconnects.

---

## Task-Specific Questions

1. What patterns emerge from your last 10 customer conversations?
2. What questions keep coming up in sales calls?
3. Where are competitors' content efforts falling short?
4. What unique insights from customer research aren't being shared elsewhere?
5. Which existing content drives the most conversions, and why?

---

## References

- **[Headless CMS Guide](references/headless-cms.md)**: CMS selection, content modeling for marketing, editorial workflows, platform comparison (Sanity, Contentful, Strapi)

---

## Related Skills

- **copywriting**: For writing individual content pieces
- **seo-audit**: For technical SEO and on-page optimization
- **ai-seo**: For optimizing content for AI search engines and getting cited by LLMs
- **programmatic-seo**: For scaled content generation
- **site-architecture**: For page hierarchy, navigation design, and URL structure
- **emails**: For email-based content
- **social**: For social media content

---

## `skills/copy-editing/SKILL.md`

---
name: copy-editing
description: "When the user wants to edit, review, or improve existing marketing copy, or refresh outdated content. Also use when the user mentions 'edit this copy,' 'review my copy,' 'copy feedback,' 'proofread,' 'polish this,' 'make this better,' 'copy sweep,' 'tighten this up,' 'this reads awkwardly,' 'clean up this text,' 'too wordy,' 'sharpen the messaging,' 'refresh this content,' 'update this page,' 'this content is outdated,' or 'content audit.' Use this when the user already has copy and wants it improved or refreshed rather than rewritten from scratch. For writing new copy, see copywriting."
metadata:
  version: 2.0.0
---

# Copy Editing

You are an expert copy editor specializing in marketing and conversion copy. Your goal is to systematically improve existing copy through focused editing passes while preserving the core message.

## Core Philosophy

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists (or `.claude/product-marketing.md`, or the legacy `product-marketing-context.md` filename, in older setups), read it before editing. Use brand voice and customer language from that context to guide your edits.

Good copy editing isn't about rewriting—it's about enhancing. Each pass focuses on one dimension, catching issues that get missed when you try to fix everything at once.

**Key principles:**
- Don't change the core message; focus on enhancing it
- Multiple focused passes beat one unfocused review
- Each edit should have a clear reason
- Preserve the author's voice while improving clarity

---

## The Seven Sweeps Framework

Edit copy through seven sequential passes, each focusing on one dimension. After each sweep, loop back to check previous sweeps aren't compromised.

### Sweep 1: Clarity

**Focus:** Can the reader understand what you're saying?

**What to check:**
- Confusing sentence structures
- Unclear pronoun references
- Jargon or insider language
- Ambiguous statements
- Missing context

**Common clarity killers:**
- Sentences trying to say too much
- Abstract language instead of concrete
- Assuming reader knowledge they don't have
- Burying the point in qualifications

**Process:**
1. Read through quickly, highlighting unclear parts
2. Don't correct yet—just note problem areas
3. After marking issues, recommend specific edits
4. Verify edits maintain the original intent

**After this sweep:** Confirm the "Rule of One" (one main idea per section) and "You Rule" (copy speaks to the reader) are intact.

---

### Sweep 2: Voice and Tone

**Focus:** Is the copy consistent in how it sounds?

**What to check:**
- Shifts between formal and casual
- Inconsistent brand personality
- Mood changes that feel jarring
- Word choices that don't match the brand

**Common voice issues:**
- Starting casual, becoming corporate
- Mixing "we" and "the company" references
- Humor in some places, serious in others (unintentionally)
- Technical language appearing randomly

**Process:**
1. Read aloud to hear inconsistencies
2. Mark where tone shifts unexpectedly
3. Recommend edits that smooth transitions
4. Ensure personality remains throughout

**After this sweep:** Return to Clarity Sweep to ensure voice edits didn't introduce confusion.

---

### Sweep 3: So What

**Focus:** Does every claim answer "why should I care?"

**What to check:**
- Features without benefits
- Claims without consequences
- Statements that don't connect to reader's life
- Missing "which means..." bridges

**The So What test:**
For every statement, ask "Okay, so what?" If the copy doesn't answer that question with a deeper benefit, it needs work.

❌ "Our platform uses AI-powered analytics"
*So what?*
✅ "Our AI-powered analytics surface insights you'd miss manually—so you can make better decisions in half the time"

**Common So What failures:**
- Feature lists without benefit connections
- Impressive-sounding claims that don't land
- Technical capabilities without outcomes
- Company achievements that don't help the reader

**Process:**
1. Read each claim and literally ask "so what?"
2. Highlight claims missing the answer
3. Add the benefit bridge or deeper meaning
4. Ensure benefits connect to real reader desires

**After this sweep:** Return to Voice and Tone, then Clarity.

---

### Sweep 4: Prove It

**Focus:** Is every claim supported with evidence?

**What to check:**
- Unsubstantiated claims
- Missing social proof
- Assertions without backup
- "Best" or "leading" without evidence

**Types of proof to look for:**
- Testimonials with names and specifics
- Case study references
- Statistics and data
- Third-party validation
- Guarantees and risk reversals
- Customer logos
- Review scores

**Common proof gaps:**
- "Trusted by thousands" (which thousands?)
- "Industry-leading" (according to whom?)
- "Customers love us" (show them saying it)
- Results claims without specifics

**Process:**
1. Identify every claim that needs proof
2. Check if proof exists nearby
3. Flag unsupported assertions
4. Recommend adding proof or softening claims

**After this sweep:** Return to So What, Voice and Tone, then Clarity.

---

### Sweep 5: Specificity

**Focus:** Is the copy concrete enough to be compelling?

**What to check:**
- Vague language ("improve," "enhance," "optimize")
- Generic statements that could apply to anyone
- Round numbers that feel made up
- Missing details that would make it real

**Specificity upgrades:**

| Vague | Specific |
|-------|----------|
| Save time | Save 4 hours every week |
| Many customers | 2,847 teams |
| Fast results | Results in 14 days |
| Improve your workflow | Cut your reporting time in half |
| Great support | Response within 2 hours |

**Common specificity issues:**
- Adjectives doing the work nouns should do
- Benefits without quantification
- Outcomes without timeframes
- Claims without concrete examples

**Process:**
1. Highlight vague words and phrases
2. Ask "Can this be more specific?"
3. Add numbers, timeframes, or examples
4. Remove content that can't be made specific (it's probably filler)

**After this sweep:** Return to Prove It, So What, Voice and Tone, then Clarity.

---

### Sweep 6: Heightened Emotion

**Focus:** Does the copy make the reader feel something?

**What to check:**
- Flat, informational language
- Missing emotional triggers
- Pain points mentioned but not felt
- Aspirations stated but not evoked

**Emotional dimensions to consider:**
- Pain of the current state
- Frustration with alternatives
- Fear of missing out
- Desire for transformation
- Pride in making smart choices
- Relief from solving the problem

**Techniques for heightening emotion:**
- Paint the "before" state vividly
- Use sensory language
- Tell micro-stories
- Reference shared experiences
- Ask questions that prompt reflection

**Process:**
1. Read for emotional impact—does it move you?
2. Identify flat sections that should resonate
3. Add emotional texture while staying authentic
4. Ensure emotion serves the message (not manipulation)

**After this sweep:** Return to Specificity, Prove It, So What, Voice and Tone, then Clarity.

---

### Sweep 7: Zero Risk

**Focus:** Have we removed every barrier to action?

**What to check:**
- Friction near CTAs
- Unanswered objections
- Missing trust signals
- Unclear next steps
- Hidden costs or surprises

**Risk reducers to look for:**
- Money-back guarantees
- Free trials
- "No credit card required"
- "Cancel anytime"
- Social proof near CTA
- Clear expectations of what happens next
- Privacy assurances

**Common risk issues:**
- CTA asks for commitment without earning trust
- Objections raised but not addressed
- Fine print that creates doubt
- Vague "Contact us" instead of clear next step

**Process:**
1. Focus on sections near CTAs
2. List every reason someone might hesitate
3. Check if the copy addresses each concern
4. Add risk reversals or trust signals as needed

**After this sweep:** Return through all previous sweeps one final time: Heightened Emotion, Specificity, Prove It, So What, Voice and Tone, Clarity.

---

## Expert Panel Scoring

Use this after completing the Seven Sweeps for an additional quality gate. For high-stakes copy (landing pages, launch emails, sales pages), a multi-persona expert review catches issues that a single perspective misses.

### How It Works

1. **Assemble 3-5 expert personas** relevant to the copy type
2. **Each persona scores the copy 1-10** on their area of expertise
3. **Collect specific critiques** — not just scores, but what to fix
4. **Revise based on feedback** — address the lowest-scoring areas first
5. **Re-score after revisions** — iterate until all personas score 7+, with an average of 8+ across the panel

### Recommended Expert Panels

**Landing page copy:**
- Conversion copywriter (clarity, CTA strength, benefit hierarchy)
- UX writer (scannability, cognitive load, user flow)
- Target customer persona (does this speak to me? do I trust it?)
- Brand strategist (voice consistency, positioning accuracy)

**Email sequence:**
- Email marketing specialist (subject lines, open/click optimization)
- Copywriter (hooks, storytelling, persuasion)
- Spam filter analyst (deliverability red flags, trigger words)
- Target customer persona (relevance, value, unsubscribe risk)

**Sales page / long-form:**
- Direct response copywriter (offer structure, objection handling, urgency)
- Skeptical buyer persona (proof gaps, trust issues, red flags)
- Editor (flow, readability, conciseness)
- SEO specialist (keyword coverage, search intent alignment)

### Scoring Rubric

| Score | Meaning |
|-------|---------|
| 9-10 | Publish-ready. No meaningful improvements. |
| 7-8 | Strong. Minor tweaks only. |
| 5-6 | Functional but has clear gaps. Needs another pass. |
| 3-4 | Significant issues. Major revision needed. |
| 1-2 | Fundamentally broken. Rethink approach. |

### When to Use

- **Always** for launch copy, pricing pages, and high-traffic landing pages
- **Recommended** for email sequences, sales pages, and ad copy
- **Optional** for blog posts, social content, and internal docs
- **Skip** for quick updates, minor edits, and low-stakes content

---

## Quick-Pass Editing Checks

Use these for faster reviews when a full seven-sweep process isn't needed.

### Word-Level Checks

**Cut these words:**
- Very, really, extremely, incredibly (weak intensifiers)
- Just, actually, basically (filler)
- In order to (use "to")
- That (often unnecessary)
- Things, stuff (vague)

**Replace these:**

| Weak | Strong |
|------|--------|
| Utilize | Use |
| Implement | Set up |
| Leverage | Use |
| Facilitate | Help |
| Innovative | New |
| Robust | Strong |
| Seamless | Smooth |
| Cutting-edge | New/Modern |

**Watch for:**
- Adverbs (usually unnecessary)
- Passive voice (switch to active)
- Nominalizations (verb → noun: "make a decision" → "decide")

### Sentence-Level Checks

- One idea per sentence
- Vary sentence length (mix short and long)
- Front-load important information
- Max 3 conjunctions per sentence
- No more than 25 words (usually)

### Paragraph-Level Checks

- One topic per paragraph
- Short paragraphs (2-4 sentences for web)
- Strong opening sentences
- Logical flow between paragraphs
- White space for scannability

---

## Copy Editing Checklist

For a final QA pass before delivering edits, work through the full checklist in [references/checklist.md](references/checklist.md) — covering all seven sweeps plus pre-start and final-check items.

---

## Common Copy Problems & Fixes

### Problem: Wall of Features
**Symptom:** List of what the product does without why it matters
**Fix:** Add "which means..." after each feature to bridge to benefits

### Problem: Corporate Speak
**Symptom:** "Leverage synergies to optimize outcomes"
**Fix:** Ask "How would a human say this?" and use those words

### Problem: Weak Opening
**Symptom:** Starting with company history or vague statements
**Fix:** Lead with the reader's problem or desired outcome

### Problem: Buried CTA
**Symptom:** The ask comes after too much buildup, or isn't clear
**Fix:** Make the CTA obvious, early, and repeated

### Problem: No Proof
**Symptom:** "Customers love us" with no evidence
**Fix:** Add specific testimonials, numbers, or case references

### Problem: Generic Claims
**Symptom:** "We help businesses grow"
**Fix:** Specify who, how, and by how much

### Problem: Mixed Audiences
**Symptom:** Copy tries to speak to everyone, resonates with no one
**Fix:** Pick one audience and write directly to them

### Problem: Feature Overload
**Symptom:** Listing every capability, overwhelming the reader
**Fix:** Focus on 3-5 key benefits that matter most to the audience

---

## Working with Copy Sweeps

When editing collaboratively:

1. **Run a sweep and present findings** - Show what you found, why it's an issue
2. **Recommend specific edits** - Don't just identify problems; propose solutions
3. **Request the updated copy** - Let the author make final decisions
4. **Verify previous sweeps** - After each round of edits, re-check earlier sweeps
5. **Repeat until clean** - Continue until a full sweep finds no new issues

This iterative process ensures each edit doesn't create new problems while respecting the author's ownership of the copy.

---

## References

- [Plain English Alternatives](references/plain-english-alternatives.md): Replace complex words with simpler alternatives
- [Content Refresh](references/content-refresh.md): Full checklist, refresh vs. rewrite matrix, and cadence guide
- [Copy Editing Checklist](references/checklist.md): Full QA checklist across all seven sweeps

---

## Content Refresh Editing

Copy editing isn't just for new content. Existing pages decay over time — outdated stats, stale examples, and drifted brand voice. Use the content refresh framework when traffic is declining, data is stale, or the product has changed.

**For the full refresh checklist, refresh vs. rewrite decision matrix, and cadence guide**: See [references/content-refresh.md](references/content-refresh.md)

---

## Task-Specific Questions

1. What's the goal of this copy? (Awareness, conversion, retention)
2. What action should readers take?
3. Are there specific concerns or known issues?
4. What proof/evidence do you have available?
5. Is this new copy or a refresh of existing content?

---

## Related Skills

- **copywriting**: For writing new copy from scratch (use this skill to edit after your first draft is complete)
- **cro**: For broader page optimization beyond copy
- **marketing-psychology**: For understanding why certain edits improve conversion
- **ab-testing**: For testing copy variations

---

## When to Use Each Skill

| Task | Skill to Use |
|------|--------------|
| Writing new page copy from scratch | copywriting |
| Reviewing and improving existing copy | copy-editing (this skill) |
| Editing copy you just wrote | copy-editing (this skill) |
| Structural or strategic page changes | cro |
