# claude-seo

> **Comprehensive SEO audit skill for Claude Code** — 20 sub-skills covering technical SEO, E-E-A-T, schema markup, GEO, local SEO, PDF reports, and Google API integration

<p align="center">
  <a href="https://github.com/hmzainjamil/claude-seo/stargazers"><img src="https://img.shields.io/github/stars/hmzainjamil/claude-seo?style=for-the-badge&labelColor=555&color=yellow" alt="Stars"/></a>
  <a href="https://github.com/hmzainjamil/claude-seo/network/members"><img src="https://img.shields.io/github/forks/hmzainjamil/claude-seo?style=for-the-badge&labelColor=555&color=blue" alt="Forks"/></a>
  <a href="https://github.com/hmzainjamil/claude-seo/issues"><img src="https://img.shields.io/github/issues/hmzainjamil/claude-seo?style=for-the-badge&labelColor=555&color=red" alt="Issues"/></a>
  <a href="https://github.com/hmzainjamil/claude-seo/pulls"><img src="https://img.shields.io/github/issues-pr/hmzainjamil/claude-seo?style=for-the-badge&labelColor=555&color=purple" alt="PRs"/></a>
  <a href="https://github.com/hmzainjamil/claude-seo/commits/main"><img src="https://img.shields.io/github/last-commit/hmzainjamil/claude-seo?style=for-the-badge&labelColor=555&color=green" alt="Last Commit"/></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Sub--skills-20-blue?style=flat&labelColor=555"/>
  <img src="https://img.shields.io/badge/Claude_Code-skill-orange?style=flat&labelColor=555"/>
  <img src="https://img.shields.io/badge/Google_APIs-Search_Console|PageSpeed|CrUX|GA4-green?style=flat&labelColor=555"/>
  <img src="https://img.shields.io/badge/GEO-AI_search-red?style=flat&labelColor=555"/>
  <img src="https://img.shields.io/badge/License-MIT-lightgrey?style=flat&labelColor=555"/>
</p>

---

## Why This Exists

SEO is 20+ distinct disciplines: technical crawlability, on-page optimization, E-E-A-T signals, schema markup, image optimization, sitemap architecture, AI search (GEO), local SEO, international SEO, e-commerce SEO, content quality, Google API data, and more. No single tool covers all of them. This Claude Code skill integrates 20 specialized sub-skills into one command: `/seo-audit https://yoursite.com`.

---

## At a Glance

| Sub-skill | Coverage |
|---|---|
| Technical SEO | Crawlability, redirects, Core Web Vitals, canonicals |
| On-page analysis | Title tags, meta descriptions, heading structure, content |
| E-E-A-T | Experience, Expertise, Authoritativeness, Trust signals |
| Schema markup | JSON-LD generation for 15+ schema types |
| Image optimization | Alt text, file sizes, next-gen formats, lazy loading |
| Sitemap architecture | XML sitemaps, image sitemaps, video sitemaps |
| GEO (AI search) | Citation probability, Perplexity/ChatGPT/Gemini optimization |
| Local SEO | GBP optimization, NAP consistency, local citations |
| Maps intelligence | Google Maps ranking factors, local pack analysis |
| Semantic clustering | Topic cluster analysis, keyword cannibalization |
| SXO | Search experience optimization, intent matching |
| SEO drift monitoring | Ranking changes, traffic drops, algorithm impact |
| E-commerce SEO | Product pages, category optimization, faceted nav |
| International SEO | Hreflang, cultural profiles, multi-region strategy |
| Google APIs | Search Console, PageSpeed Insights, CrUX, GA4 |
| PDF report generation | Branded PDF reports with findings and priorities |
| Strategic planning | 90-day SEO roadmap from audit findings |
| Content quality | Thin content, duplication, readability, topical depth |
| Link analysis | Internal linking structure, anchor text distribution |
| Security/HTTPS | Certificate status, mixed content, HSTS |

---

## 🧠 CONCEPTS

| Concept | Description |
|---|---|
| **E-E-A-T** | Experience, Expertise, Authoritativeness, Trustworthiness — Google's quality rater guidelines |
| **Core Web Vitals** | LCP, INP, CLS — Google's user experience ranking signals |
| **GEO** | Generative Engine Optimization — optimizing for AI answer engines |
| **Schema markup** | JSON-LD structured data — helps both crawlers and AI parse content |
| **Topic cluster** | Pillar page + cluster pages — topical authority structure |
| **Canonical** | `<link rel="canonical">` — prevents duplicate content penalties |
| **Hreflang** | Language/region tags — tells Google which version to serve per locale |
| **CrUX** | Chrome User Experience Report — real-user field data |
| **GA4** | Google Analytics 4 — traffic, engagement, and conversion data |
| **SXO** | Search Experience Optimization — optimizing for user intent signals |

### 🔥 Hot

- **Google API integration** — real data from Search Console + CrUX + PageSpeed, not estimations
- **GEO sub-skill** — tests your URLs against 5 AI engines, identifies citation gaps, generates LLMs.txt
- **PDF report generation** — branded client-ready PDF reports in minutes
- Source → [HMZ](https://github.com/hmzainjamil)

---

## ⚙️ HOW IT WORKS

```
/seo-audit https://example.com
    ↓
1. Technical crawl: robots.txt, sitemap, redirects, HTTPS
2. Core Web Vitals: PageSpeed API → LCP, INP, CLS scores
3. On-page: title tags, meta, headings, content quality
4. Schema: extract + validate all JSON-LD
5. E-E-A-T: author signals, citations, trust indicators
6. GEO: test in ChatGPT/Perplexity/Claude for brand citations
7. Local: GBP status, NAP consistency (if local business)
8. International: hreflang audit (if multi-region)
9. Images: alt text coverage, file sizes, format optimization
10. Priority matrix: sort findings by impact × effort
11. PDF report: generate branded report for client
12. 90-day roadmap: phased action plan from findings
```

---

## 🚀 INSTALL

```bash
# Install skill
mkdir -p ~/.claude/skills/claude-seo
git clone https://github.com/hmzainjamil/claude-seo
cp -r claude-seo/. ~/.claude/skills/claude-seo/

# Install Python dependencies (optional, for full API integration)
pip install requests google-auth google-auth-httplib2 google-api-python-client reportlab

# Configure API keys
export PAGESPEED_API_KEY=your_key
export GSC_CREDENTIALS_PATH=~/.config/gsc-credentials.json
export GA4_PROPERTY_ID=G-XXXXXXXXXX
```

---

## 📟 USAGE

```bash
# Full audit
/seo-audit https://yoursite.com

# Specific sub-skills
/seo-technical https://yoursite.com
/seo-schema https://yoursite.com/page
/seo-geo https://yoursite.com
/seo-local "Business Name" "City, State"
/seo-ecommerce https://yourstore.com
/seo-international https://yoursite.com --markets US,UK,DE,AU

# Generate PDF report
/seo-report https://yoursite.com --brand "Client Name" --output ~/Downloads/

# Schema generation
/schema-gen https://yoursite.com/blog-post --type Article,FAQPage

# 90-day roadmap
/seo-roadmap https://yoursite.com
```

---

## ⚙️ CONFIGURATION

| Variable | Required | Description |
|---|---|---|
| `PAGESPEED_API_KEY` | recommended | PageSpeed Insights API access |
| `GSC_CREDENTIALS_PATH` | optional | Google Search Console OAuth2 credentials |
| `GA4_PROPERTY_ID` | optional | GA4 for traffic + conversion data |
| `CRAWL_DEPTH` | 3 | Max crawl depth for technical audit |
| `CRAWL_LIMIT` | 200 | Max pages per audit |
| `AUDIT_SCOPE` | `full` | `quick` (5min) or `full` (20min) |
| `GEO_ENGINES` | all | `chatgpt,claude,perplexity,gemini,google_aio` |
| `SCHEMA_TYPES` | auto | Comma-separated list of schema types to generate |
| `REPORT_TEMPLATE` | `standard` | `standard` or `minimal` |
| `OUTPUT_FORMAT` | `markdown` | `markdown`, `json`, or `pdf` |
| `PRIORITY_THRESHOLD` | `7` | Issues scored ≥7 added to priority list |
| `LOCALE` | `en-US` | Primary locale for analysis |

---

## 💡 TIPS AND TRICKS

### Audit Workflow
1. **Quick audit first** — run `--audit-scope quick` for initial triage. Full audit only for priority clients. Source → [HMZ](https://github.com/hmzainjamil)
2. **API keys unlock real data** — without GSC credentials, audit uses estimated data. With them, exact click/impression data. Source → [HMZ](https://github.com/hmzainjamil)
3. **Monthly drift monitoring** — schedule monthly audits, compare findings to detect algorithm impacts early. Source → [HMZ](https://github.com/hmzainjamil)

### Schema Strategy
4. **Priority schema types** — Article + FAQPage + BreadcrumbList covers 80% of schema impact for most sites. Source → [HMZ](https://github.com/hmzainjamil)
5. **Validate before publish** — run generated schema through schema.org validator before deploying. Source → [HMZ](https://github.com/hmzainjamil)
6. **Author entity markup** — `Person` schema with `sameAs` Wikipedia URL = strongest E-E-A-T signal available. Source → [HMZ](https://github.com/hmzainjamil)

### GEO Integration
7. **LLMs.txt priority** — generate `/llms.txt` first. Highest ROI single action for AI search visibility. Source → [HMZ](https://github.com/hmzainjamil)
8. **AI citation testing** — test 5-10 brand queries in ChatGPT and Perplexity before and after optimization. Source → [HMZ](https://github.com/hmzainjamil)
9. **Brand mention building** — identified gap between brand citations and organic rankings = GEO opportunity. Source → [HMZ](https://github.com/hmzainjamil)

### Agency Use
10. **PDF reports** — `/seo-report --brand "Client Name"` generates branded PDF in minutes. Bill as premium deliverable. Source → [HMZ](https://github.com/hmzainjamil)
11. **Competitive audits** — run audit on competitor URLs to identify gap opportunities. Source → [HMZ](https://github.com/hmzainjamil)
12. **90-day roadmap** — `/seo-roadmap` turns audit findings into phased action plan. Use as SOW for retainer. Source → [HMZ](https://github.com/hmzainjamil)

---

## 🔧 TROUBLESHOOTING

| Issue | Cause | Fix |
|---|---|---|
| PageSpeed API 403 | Invalid API key | Check key at Google Cloud Console |
| GSC no data | OAuth not configured | Run `gsc-auth.py` to set up credentials |
| Crawl blocked | robots.txt blocking | Check robots.txt for UserAgent restrictions |
| Schema validation fails | Malformed JSON | Run through schema.org validator |
| GEO test empty | AI engine throttled | Retry after 30s delay |
| PDF generation fails | Missing ReportLab | `pip install reportlab` |
| Hreflang errors | Wrong language codes | Use ISO 639-1 + ISO 3166-1 format |

---

## 📊 ARCHITECTURE

```
claude-seo/
├── SKILL.md               # Master skill definition
├── sub-skills/
│   ├── seo-technical.md
│   ├── seo-schema.md
│   ├── seo-geo.md
│   ├── seo-local.md
│   ├── seo-ecommerce.md
│   └── seo-international.md
├── tools/
│   ├── audit.py           # Full audit runner
│   ├── schema_gen.py      # JSON-LD generator
│   ├── pdf_report.py      # ReportLab report generator
│   ├── pagespeed.py       # PageSpeed API client
│   └── gsc_client.py      # Google Search Console client
└── templates/
    ├── report_standard.py
    └── schema_templates/
```

---

## 🗺️ ROADMAP

- [ ] Real-time monitoring — weekly automated audits with email diff reports
- [ ] Competitor tracking — monitor competitor SEO changes automatically
- [ ] CMS integrations — direct schema injection into WordPress/Shopify via API
- [ ] AI writing — auto-generate optimized content from keyword + E-E-A-T brief
- [ ] Agency portal — multi-client dashboard for managing audits

---

## ☠️ STARTUPS / BUSINESSES

SEO audits are $2-15K deliverables from agencies. This skill automates 80% of the work: data gathering, analysis, schema generation, PDF report. An agency equipped with this skill can deliver 10× more audits per month at the same quality.

**Retainer play:** `/seo-drift-monitor` runs monthly, detects algorithm impacts, generates change reports. Sell as $1-3K/mo monitoring retainer with automated reports.

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/claude-seo&type=Date)](https://star-history.com/#hmzainjamil/claude-seo&Date)

---

<p align="center">
  Built by <a href="https://github.com/hmzainjamil">HMZ</a> · <a href="https://github.com/hmzainjamil/claude-seo/issues">Issues</a> · <a href="https://github.com/hmzainjamil/claude-seo/pulls">PRs</a>
</p>
