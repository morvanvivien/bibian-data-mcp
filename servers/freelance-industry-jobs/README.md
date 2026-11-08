# Freelance projects and industry job boards

Freelance projects (Codeur, Freelancer, Workana, PeoplePerHour) and sector job boards. Remote MCP server hosted by [Apify](https://apify.com/mcp), 11 tools maintained by [bibian](https://apify.com/bibian). Public pages only, no login on the source sites, no personal data.

## Tools

| Tool | What it returns |
|---|---|
| [Codeur.com Freelance Projects Scraper (France)](https://apify.com/bibian/codeur-projects-scraper) | Extract freelance projects posted by clients on Codeur.com, France's leading freelance marketplace: title, budget, category, wanted profiles, number of offers and views, publication date and full brief. Ideal for daily lead alerts. |
| [Freelancer.com Projects Scraper - No Login](https://apify.com/bibian/freelancer-projects-scraper) | Extract freelance projects posted by clients on Freelancer.com worldwide: budget, type, bids, categories and skills, no login or account required. |
| [Workana Scraper - LatAm Freelance Projects](https://apify.com/bibian/workana-projects-scraper) | Extract freelance projects posted on Workana, Latin America's freelance marketplace (Argentina, Brazil, Mexico, Chile, Colombia, Peru and more). Budget, skills, category and full description for each open project, ready to pipe into your own job board or lead list. |
| [PeoplePerHour Scraper · Freelance Jobs](https://apify.com/bibian/peopleperhour-scraper) | Extract freelance jobs posted by clients on PeoplePerHour: budget, skills, experience level, country restriction and full description, ready to pipe into your own job board or lead list. |
| [French Freelance Day Rates (TJM) · IT Skills & Cities](https://apify.com/bibian/french-freelance-day-rates) | Median, quartile and average IT freelance daily rates (TJM) in France by skill and city, computed live from current Free-Work freelance missions. |
| [Hospitality Jobs Scraper · 4 Boards, One Schema](https://apify.com/bibian/hospitality-jobs-scraper) | Extract hospitality and restaurant job postings from 4 sector job boards in one run: L'Hôtellerie Restauration (FR), HOGAPAGE (DE), Gastrojobs (DE) and Hosco (worldwide). One unified schema, deduplicated across sources, no login. |
| [Wine & Agriculture Jobs Scraper · 4 Boards](https://apify.com/bibian/wine-agriculture-jobs-scraper) | Extract wine and agriculture job postings from 4 sector boards in one run: Apecita (France), WineBusiness Classifieds (US), Wine Industry Jobs (Australia) and Vitijob (France). One unified schema, deduplicated across sources, no login. |
| [Education & Research Jobs Scraper · 4 Boards, One Schema](https://apify.com/bibian/education-research-jobs-scraper) | Extract education and research job postings from 4 sector job boards in one run: TES (GB), Eteach (GB), jobs.ac.uk (GB) and HigherEdJobs (US). One unified schema, deduplicated across sources, no login. |
| [Nonprofit Jobs Scraper · 4 Boards, One Schema](https://apify.com/bibian/nonprofit-jobs-scraper) | Extract nonprofit and social-sector job postings from 4 job boards in one run: CharityJob (GB), Idealist (US), Pro Bono Australia (AU) and HacesFalta (ES). One unified schema, deduplicated across sources, no login. |
| [Trucking & Logistics Jobs Scraper · 2 Boards, One Schema](https://apify.com/bibian/trucking-logistics-jobs-scraper) | Extract trucking and logistics driver job postings from 2 sector job boards in one run: TDR Jobs (Spain) and CDL Jobs (United States). One unified schema, deduplicated across sources, no login. |
| [Energy & Construction Jobs Scraper · 3 Boards](https://apify.com/bibian/energy-construction-finance-jobs-scraper) | Extract energy and construction job postings from 3 sector job boards in one run: Energy Jobline (global), Energy Job Shop (US/CA oil & gas) and ConstructionJobs (US). One unified schema, deduplicated across sources, no login. |

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account, or `Authorization: Bearer <APIFY_TOKEN>`):

```
https://mcp.apify.com?tools=bibian/codeur-projects-scraper,bibian/freelancer-projects-scraper,bibian/workana-projects-scraper,bibian/peopleperhour-scraper,bibian/french-freelance-day-rates,bibian/hospitality-jobs-scraper,bibian/wine-agriculture-jobs-scraper,bibian/education-research-jobs-scraper,bibian/nonprofit-jobs-scraper,bibian/trucking-logistics-jobs-scraper,bibian/energy-construction-finance-jobs-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-freelance-industry-jobs": {
      "url": "https://mcp.apify.com?tools=bibian/codeur-projects-scraper,bibian/freelancer-projects-scraper,bibian/workana-projects-scraper,bibian/peopleperhour-scraper,bibian/french-freelance-day-rates,bibian/hospitality-jobs-scraper,bibian/wine-agriculture-jobs-scraper,bibian/education-research-jobs-scraper,bibian/nonprofit-jobs-scraper,bibian/trucking-logistics-jobs-scraper,bibian/energy-construction-finance-jobs-scraper"
    }
  }
}
```

Each tool is pay per result on Apify: you only pay for the rows you get. Missing a site, a field or a filter? Open an issue on the tool's Apify page.
