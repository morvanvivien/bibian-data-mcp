# French job boards: Free-Work, HelloWork, France Travail, WTTJ

Job postings and freelance day rates from 8 French job boards, as JSON tools. Remote MCP server hosted by [Apify](https://apify.com/mcp), 10 tools maintained by [bibian](https://apify.com/bibian). Public pages only, no login on the source sites, no personal data.

## Tools

| Tool | What it returns |
|---|---|
| [France Jobs Scraper · 8 Boards, One Schema](https://apify.com/bibian/france-jobs-scraper) | Extract job postings from 8 major French job boards in one run: Free-Work, Welcome to the Jungle, HelloWork, Meteojob, France Travail, Emploi Territorial, Choisir le Service Public and Qapa. One unified schema, deduplicated across sources, no login. |
| [Free-Work Jobs & Freelance Missions Scraper](https://apify.com/bibian/free-work-jobs-scraper) | Extract IT jobs and freelance missions from Free-Work, the leading French tech job board: daily rates, salaries, skills, remote mode, location and full descriptions. |
| [French Freelance Day Rates (TJM) · IT Skills & Cities](https://apify.com/bibian/french-freelance-day-rates) | Median, quartile and average IT freelance daily rates (TJM) in France by skill and city, computed live from current Free-Work freelance missions. |
| [Welcome to the Jungle Scraper · Jobs, No Login](https://apify.com/bibian/welcometothejungle-scraper) | Extract job postings from Welcome to the Jungle (France and Europe): title, contract, salary when published, remote policy, location and hiring company, no account needed. |
| [HelloWork Jobs Scraper · No Login Needed](https://apify.com/bibian/hellowork-jobs-scraper) | Extract job postings from HelloWork (France): title, company, salary when published, remote policy, location and full description, no account needed. |
| [Meteojob Jobs Scraper (France)](https://apify.com/bibian/meteojob-jobs-scraper) | Extract job postings from Meteojob, a major French job board: title, company, salary, location, contract type, work hours and full description. |
| [France Travail Jobs Scraper · No Login](https://apify.com/bibian/francetravail-jobs-scraper) | Extract job postings from France Travail, the French government's official job board: title, employer, location, contract type and description. No login, no browser. |
| [Emploi-Territorial Jobs Scraper (French Public Sector)](https://apify.com/bibian/emploi-territorial-jobs-scraper) | Extract French local government job postings from emploi-territorial.fr (about 27,000 live offers): employer, department, category, grade, deadline, missions, profile and application link. |
| [Choisir le Service Public Scraper · No Login](https://apify.com/bibian/choisirleservicepublic-jobs-scraper) | Extract job postings from Choisir le Service Public, the French government's civil service job board: title, employer, location, salary and full description. No login, no browser. |
| [Qapa Scraper: No Login Temp Jobs France](https://apify.com/bibian/qapa-jobs-scraper) | Extract temporary (interim) and permanent job postings from Qapa, a major French staffing platform: title, company, location, dates, hourly wage and full description. |

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account, or `Authorization: Bearer <APIFY_TOKEN>`):

```
https://mcp.apify.com?tools=bibian/france-jobs-scraper,bibian/free-work-jobs-scraper,bibian/french-freelance-day-rates,bibian/welcometothejungle-scraper,bibian/hellowork-jobs-scraper,bibian/meteojob-jobs-scraper,bibian/francetravail-jobs-scraper,bibian/emploi-territorial-jobs-scraper,bibian/choisirleservicepublic-jobs-scraper,bibian/qapa-jobs-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-france-jobs": {
      "url": "https://mcp.apify.com?tools=bibian/france-jobs-scraper,bibian/free-work-jobs-scraper,bibian/french-freelance-day-rates,bibian/welcometothejungle-scraper,bibian/hellowork-jobs-scraper,bibian/meteojob-jobs-scraper,bibian/francetravail-jobs-scraper,bibian/emploi-territorial-jobs-scraper,bibian/choisirleservicepublic-jobs-scraper,bibian/qapa-jobs-scraper"
    }
  }
}
```

Each tool is pay per result on Apify: you only pay for the rows you get. Missing a site, a field or a filter? Open an issue on the tool's Apify page.
