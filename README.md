# Why Won't AI Mention My Product

[whywontai.com](https://whywontai.com/) shows what search and AI crawlers actually receive from a website.

A free scan requests up to 10 of your pages as GPTBot, ClaudeBot, PerplexityBot and CCBot, each one separately. It scores six SEO, AEO and GEO categories: crawl and render, indexable body copy, intent match, internal linking, demand capture and AI citability. You see the score and the top 3 issues without an account. A free account gives the full report.

- Free scan: https://whywontai.com/
- Free AI crawler robots.txt checker (17 crawlers): https://whywontai.com/ai-crawler-robots-txt-checker
- Guides: https://whywontai.com/guides
- Pricing: https://whywontai.com/pricing

## Remote MCP server

URL: `https://mcp.whywontai.com/` (Streamable HTTP). Reference: https://whywontai.com/mcp-server

| Tool | Key | What it does |
|---|---|---|
| `check_robots` | No key | Which of 17 search and AI crawlers a site's robots.txt allows, with the rule that decides each one. 30 checks a day without a key. |
| `scan_site` | API key | Starts a full AI visibility scan of a site on your plan. |
| `get_scan` | API key | Score, category scores, technical health, Domain Rating and top issues. |
| `list_issues` | API key | Every issue from a scan, most severe first, with example URLs. |
| `list_scans` | API key | Your recent scans. |
| `get_internal_links` | API key | Internal link suggestions (paid plans). |

### Claude Code

```bash
claude mcp add --transport http whywontai https://mcp.whywontai.com/ \
  --header "Authorization: Bearer YOUR_API_KEY"
```

Leave out the header to use `check_robots` only. To get a key, create a free account, open your dashboard and choose **MCP & API**.

Setup for other clients:

- Claude Code: https://whywontai.com/integrations/claude-code
- Cursor: https://whywontai.com/integrations/cursor
- VS Code: https://whywontai.com/integrations/vs-code

## Contact

https://whywontai.com/contact
