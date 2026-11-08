# European job boards: Germany, Spain, Switzerland, Poland, UK, EURES

Job postings from German, Spanish, Swiss, Polish, Swedish and UK job boards plus EURES. Remote MCP server hosted by [Apify](https://apify.com/mcp), 15 tools maintained by [bibian](https://apify.com/bibian). Public pages only, no login on the source sites, no personal data.

## Tools

| Tool | What it returns |
|---|---|
| [Europe Jobs Scraper · 12 Boards, 7 Countries, One Schema](https://apify.com/bibian/europe-jobs-scraper) | Extract job postings from 12 major European job boards plus EURES in one run: Free-Work, France Travail, HelloWork, Reed, Arbeitsagentur, Stellenanzeigen, Jobware, Infoempleo, Trabajos, TicJob, Arbetsformedlingen, Jobs.ch. One unified schema, deduplicated across sources, no login. |
| [Arbeitsagentur Jobs Scraper · No Login](https://apify.com/bibian/arbeitsagentur-jobs-scraper) | Extract German job postings from the Bundesagentur für Arbeit's public Jobsuche API: title, company, location, salary, contract type and full description. No login, no browser. |
| [StepStone Jobs Scraper · No Login Needed](https://apify.com/bibian/stepstone-jobs-scraper) | Extract job postings from StepStone, Germany's leading job board: title, company, salary when published, remote policy, location and full description, no account needed. |
| [Stellenanzeigen.de Jobs Scraper: No Login](https://apify.com/bibian/stellenanzeigen-jobs-scraper) | Extract job postings from stellenanzeigen.de, a major German job board: title, company, location, employment type, industry and full description. |
| [Jobware Scraper: German Jobs, Company & Salary](https://apify.com/bibian/jobware-scraper) | Extract German job postings from jobware.de: title, company, location, employment type, salary estimate and full description. No login, no browser. |
| [Meinestadt Scraper · No Login, All Cities](https://apify.com/bibian/meinestadt-jobs-scraper) | Extract local German job postings from meinestadt.de's Stellenmarkt across any city: title, company, address, salary, employment type, skills, benefits and full description. |
| [Jobs.ch Scraper · Swiss Jobs, No Login](https://apify.com/bibian/jobs-ch-jobs-scraper) | Extract Swiss job postings from jobs.ch: title, company, location, employment type, work hours, salary range and full description. No login, no browser. |
| [Pracuj.pl Scraper · Polish Jobs, No Login](https://apify.com/bibian/pracuj-jobs-scraper) | Extract Polish job postings from pracuj.pl: title, company, location, salary, contract type, work mode, remote policy and full description. No login, no browser. |
| [Arbetsformedlingen Scraper: Sweden Jobs](https://apify.com/bibian/arbetsformedlingen-jobs-scraper) | Scrape Swedish job ads from Arbetsformedlingen (JobTech): employer, occupation codes, location, schedule and full description from the official API. |
| [EURES Jobs Scraper: All EU/EEA Countries](https://apify.com/bibian/eures-jobs-scraper) | Extract live job vacancies from EURES, the European Union's official job portal covering all EU/EEA countries: title, country, region, work schedule, publication date and occupation tags. No login, no captcha-solving. |
| [Reed.co.uk Jobs Scraper · No Login Needed](https://apify.com/bibian/reed-jobs-scraper) | Extract job postings from Reed.co.uk, one of the UK's largest job boards: title, company, salary range, location, employment type and full description. |
| [Infoempleo Jobs Scraper (Spain)](https://apify.com/bibian/infoempleo-jobs-scraper) | Extract job postings from Infoempleo, one of Spain's main job boards: title, company, salary range, location, experience, contract details and full description. |
| [Trabajos.com Jobs Scraper · No Login](https://apify.com/bibian/trabajos-jobs-scraper) | Extract job postings from Trabajos.com, a Spanish job board: title, company, location, salary, contract type, work schedule and full description. |
| [Empléate.gob.es Jobs Scraper (Spain)](https://apify.com/bibian/empleate-jobs-scraper) | Extract job postings from Empléate, Spain's official public employment service (SEPE) job board: title, company, salary when published, province, contract type and full description, no account needed. |
| [Ticjob Scraper: Spain Tech Job Postings](https://apify.com/bibian/ticjob-jobs-scraper) | Extract IT and tech job postings from Ticjob, a Spanish job board specialized in technology roles (SAP, developers, cloud, infrastructure): title, company, location, contract type, dates and full description. |

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account, or `Authorization: Bearer <APIFY_TOKEN>`):

```
https://mcp.apify.com?tools=bibian/europe-jobs-scraper,bibian/arbeitsagentur-jobs-scraper,bibian/stepstone-jobs-scraper,bibian/stellenanzeigen-jobs-scraper,bibian/jobware-scraper,bibian/meinestadt-jobs-scraper,bibian/jobs-ch-jobs-scraper,bibian/pracuj-jobs-scraper,bibian/arbetsformedlingen-jobs-scraper,bibian/eures-jobs-scraper,bibian/reed-jobs-scraper,bibian/infoempleo-jobs-scraper,bibian/trabajos-jobs-scraper,bibian/empleate-jobs-scraper,bibian/ticjob-jobs-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-europe-jobs": {
      "url": "https://mcp.apify.com?tools=bibian/europe-jobs-scraper,bibian/arbeitsagentur-jobs-scraper,bibian/stepstone-jobs-scraper,bibian/stellenanzeigen-jobs-scraper,bibian/jobware-scraper,bibian/meinestadt-jobs-scraper,bibian/jobs-ch-jobs-scraper,bibian/pracuj-jobs-scraper,bibian/arbetsformedlingen-jobs-scraper,bibian/eures-jobs-scraper,bibian/reed-jobs-scraper,bibian/infoempleo-jobs-scraper,bibian/trabajos-jobs-scraper,bibian/empleate-jobs-scraper,bibian/ticjob-jobs-scraper"
    }
  }
}
```

Each tool is pay per result on Apify: you only pay for the rows you get. Missing a site, a field or a filter? Open an issue on the tool's Apify page.
