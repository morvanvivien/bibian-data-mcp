# Job boards: Latin America, US, Canada, Australia, Singapore

Job postings from Latin American, North American and Asia Pacific job boards, as JSON. Remote MCP server hosted by [Apify](https://apify.com/mcp), 14 tools maintained by [bibian](https://apify.com/bibian). Public pages only, no login on the source sites, no personal data.

## Tools

| Tool | What it returns |
|---|---|
| [Latin America Jobs Scraper · 4 Networks, 18 Countries](https://apify.com/bibian/latin-america-jobs-scraper) | Extract job postings from 4 Latin American networks in one run: Bumeran/Navent (Zonajobs, Laborum, Multitrabajos, Konzerta), Computrabajo, Get on Board and Gupy. One unified schema, deduplicated across sources, across 18 countries, no login. |
| [Bumeran, Zonajobs & Laborum Jobs Scraper (LatAm)](https://apify.com/bibian/latam-jobs-bumeran-scraper) | Extract job postings from Latin America's leading job boards in one run: Bumeran and Zonajobs (Argentina, Peru, Venezuela), Laborum (Chile), Multitrabajos (Ecuador) and Konzerta (Panama). About 70,000 live jobs with company, location, work mode and full description. |
| [Computrabajo Scraper · 18 Countries](https://apify.com/bibian/computrabajo-jobs-scraper) | Extract job postings from Computrabajo across 18 Latin American countries: title, company, salary, location, employment type and full description. |
| [Get on Board Tech Jobs Scraper (LatAm & Remote)](https://apify.com/bibian/getonbrd-jobs-scraper) | Extract tech job postings from Get on Board, Latin America's leading tech job board: company, seniority, salary range in USD, skills, perks, remote modality, cities, applications count and full description. |
| [Gupy Jobs Scraper · Any Company, No Login](https://apify.com/bibian/gupy-jobs-scraper) | Extract job postings from any company's public Gupy career board (Brazil's largest ATS): title, department, location, workplace type and full description, by company subdomain. No login, no browser. |
| [North America Jobs Scraper · USA & Canada, 6 Boards, One Schema](https://apify.com/bibian/north-america-jobs-scraper) | Extract job postings from 6 major US and Canadian job boards in one run: Job Bank (Canada), The Muse, Built In, Dice, Wellfound and Hacker News Who is Hiring. One unified schema, deduplicated across sources, no login. |
| [Job Bank Canada Scraper · + Salaries](https://apify.com/bibian/jobbank-jobs-scraper) | Extract job postings from Job Bank, the Government of Canada's official job board: title, employer, location, NOC code, salary range and full description. No login, no browser. |
| [Dice.com Jobs Scraper (US Tech Jobs)](https://apify.com/bibian/dice-jobs-scraper) | Extract US tech job postings from Dice.com: title, company, location, salary range, remote/on-site type, contract type and full description. |
| [BuiltIn Scraper: US Tech Job Postings](https://apify.com/bibian/builtin-jobs-scraper) | Extract tech job postings from BuiltIn.com (US): title, company, salary range, location, remote status, industry and full description. |
| [TheMuse Scraper · Jobs API, No Login](https://apify.com/bibian/themuse-jobs-scraper) | Scrape The Muse job postings via its official public API: title, company, locations, categories, levels and full description. No login, no browser. |
| [Wellfound Scraper: Startup Jobs No Login](https://apify.com/bibian/wellfound-jobs-scraper) | Extract startup job postings from Wellfound (ex-AngelList Talent) worldwide: title, company, compensation, remote status and full description, with no login needed. |
| [Asia Pacific Jobs Scraper · AU, NZ & Singapore](https://apify.com/bibian/asia-pacific-jobs-scraper) | Extract job postings from SEEK (Australia, New Zealand) and MyCareersFuture (Singapore) in one run, one unified schema, deduplicated across sources. Malaysia, Philippines, Indonesia, Hong Kong and Thailand stay selectable but have no source yet. |
| [SEEK Jobs Scraper: Australia & NZ, No Login](https://apify.com/bibian/seek-jobs-scraper) | Scrape SEEK job postings for Australia and New Zealand: title, company, salary, location and work type from the public search pages, no login. |
| [MyCareersFuture Scraper: SG Jobs, No Login](https://apify.com/bibian/mycareersfuture-jobs-scraper) | Scrape MyCareersFuture job postings, Singapore's official portal: title, salary, company, skills and full description from the public API, no login. |

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account, or `Authorization: Bearer <APIFY_TOKEN>`):

```
https://mcp.apify.com?tools=bibian/latin-america-jobs-scraper,bibian/latam-jobs-bumeran-scraper,bibian/computrabajo-jobs-scraper,bibian/getonbrd-jobs-scraper,bibian/gupy-jobs-scraper,bibian/north-america-jobs-scraper,bibian/jobbank-jobs-scraper,bibian/dice-jobs-scraper,bibian/builtin-jobs-scraper,bibian/themuse-jobs-scraper,bibian/wellfound-jobs-scraper,bibian/asia-pacific-jobs-scraper,bibian/seek-jobs-scraper,bibian/mycareersfuture-jobs-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-americas-apac-jobs": {
      "url": "https://mcp.apify.com?tools=bibian/latin-america-jobs-scraper,bibian/latam-jobs-bumeran-scraper,bibian/computrabajo-jobs-scraper,bibian/getonbrd-jobs-scraper,bibian/gupy-jobs-scraper,bibian/north-america-jobs-scraper,bibian/jobbank-jobs-scraper,bibian/dice-jobs-scraper,bibian/builtin-jobs-scraper,bibian/themuse-jobs-scraper,bibian/wellfound-jobs-scraper,bibian/asia-pacific-jobs-scraper,bibian/seek-jobs-scraper,bibian/mycareersfuture-jobs-scraper"
    }
  }
}
```

Each tool is pay per result on Apify: you only pay for the rows you get. Missing a site, a field or a filter? Open an issue on the tool's Apify page.
