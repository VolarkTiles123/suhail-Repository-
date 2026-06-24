# Volark SEO Engine

Complete SEO Automation System

## Features

- **SEO** - Traditional search engine optimization
- **GEO** - Generative Engine Optimization (ChatGPT, Claude, Gemini, Perplexity, Copilot)
- **AEO** - Answer Engine Optimization (featured snippets, AI Overviews)
- **Local SEO** - Geographic targeting for UAE cities
- **Backlink Building** - Strategic outreach and relationship building
- **Technical SEO** - Site health and crawlability
- **Internal Linking** - Content silo optimization
- **Content Creation** - EEAT-driven, semantic-rich content
- **AI Visibility Tracking** - Monitor mentions across AI platforms

## Target Market

### Countries
- UAE

### Cities
- Dubai
- Sharjah
- Abu Dhabi
- Ajman
- Ras Al Khaimah
- Fujairah
- Umm Al Quwain

## Industry Focus

**Products:**
- Porcelain Tiles
- Ceramic Tiles
- Porcelain Slabs
- Floor Tiles
- Wall Tiles
- Bathroom Tiles
- Kitchen Tiles
- Outdoor Tiles

**Audience:**
- Residential customers
- Contractors
- Architects
- Interior Designers
- Commercial developers

## Repository Structure

```
volark-seo-engine/
├── README.md                 # This file
├── skill.md                  # Master orchestrator prompt
├── config.md                 # System configuration
│
├── agents/                   # Individual agent prompts
│   ├── orchestrator.md
│   ├── keyword_research_agent.md
│   ├── competitor_intelligence_agent.md
│   ├── content_strategy_agent.md
│   ├── content_writer_agent.md
│   ├── onpage_seo_agent.md
│   ├── technical_seo_agent.md
│   ├── schema_agent.md
│   ├── internal_linking_agent.md
│   ├── local_seo_agent.md
│   ├── backlink_agent.md
│   ├── geo_agent.md
│   ├── aeo_agent.md
│   ├── publisher_agent.md
│   └── reporting_agent.md
│
├── knowledge/                # Knowledge bases and reference docs
│   ├── tile_sizes.md
│   ├── uae_locations.md
│   └── tiles_knowledge.md
│
├── templates/                # Content templates
│   ├── blog_post.md
│   └── city_page.md
│
├── workflows/                # Workflow definitions (future)
│   └── .gitkeep
│
├── data/                     # Data files and CSVs
│   ├── keywords.csv
│   ├── backlinks.csv
│   ├── rankings.csv
│   └── content_calendar.csv
│
└── reports/                  # Generated reports (future)
    └── .gitkeep
```

## Usage

1. Clone this repository
2. Copy the `skill.md` to your Claude instructions or system prompt
3. Reference individual agent prompts as needed
4. Update `config.md` with your company details
5. Connect to Google Search Console, GA4, WordPress, and Google Sheets
6. Run workflows through Claude or your automation platform

## Integration Points

- **Google Search Console** - Keyword data, impressions, clicks
- **Google Analytics 4** - Traffic, conversion data
- **WordPress** - Content publishing
- **Google Sheets** - Data tracking and reporting
- **Claude** - SEO agent orchestration

## Next Steps for Advanced Setup

To make this fully automated:

1. Create Python scripts in `/scripts/` for API integrations
2. Set up Node.js MCP (Model Context Protocol) configs
3. Build GitHub Actions workflows for CI/CD
4. Create environment variables file (.env)
5. Set up database for persistent data tracking

## License

proprietary - Volark Tiles

---

Created for Volark Tiles SEO automation in the UAE market.
