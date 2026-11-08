# Remote job boards and company career pages (Greenhouse, Lever, Workday)

Remote jobs (RemoteOK, Remotive, WWR, HN) and career pages on Greenhouse, Lever, Workday. Remote MCP server hosted by [Apify](https://apify.com/mcp), 13 tools maintained by [bibian](https://apify.com/bibian). Public pages only, no login on the source sites, no personal data.

## Tools

| Tool | What it returns |
|---|---|
| [Remote Jobs Worldwide · 8 Boards, One Schema](https://apify.com/bibian/remote-jobs-worldwide-scraper) | Extract remote job postings from 8 major remote-work boards in one run: RemoteOK, Remotive, We Work Remotely, Jobicy, Working Nomads, Hacker News Who is Hiring, Wellfound and Get on Board. One unified schema, deduplicated across sources, no login. |
| [RemoteOK Scraper: Remote Jobs & Salaries](https://apify.com/bibian/remoteok-jobs-scraper) | Extract remote job postings from RemoteOK's public API: title, company, tags, location, salary range and full description. No login, no browser. |
| [Remotive Jobs Scraper · Remote Jobs, No Login](https://apify.com/bibian/remotive-jobs-scraper) | Extract remote job postings from remotive.com: title, company, category, remote/country eligibility, employment type and full description. No login, no browser. |
| [We Work Remotely Scraper · No Login](https://apify.com/bibian/weworkremotely-jobs-scraper) | Extract remote job postings from We Work Remotely's own public RSS feed: title, company, region, category and full description. No login, no browser. |
| [Working Nomads Scraper: Remote Jobs](https://apify.com/bibian/workingnomads-jobs-scraper) | Scrape Working Nomads remote job postings from its own public feed: title, company, category, tags, location and full description. No login, no browser. |
| [Jobicy Scraper: Remote Jobs, No Login](https://apify.com/bibian/jobicy-jobs-scraper) | Scrape Jobicy remote job postings via its official public API: title, company, salary, industry, level and full description. No login, no browser. |
| [Hacker News Scraper · Who Is Hiring Threads](https://apify.com/bibian/hackernews-jobs-scraper) | Scrape job posts from Hacker News's monthly "Who is hiring?" threads via the official public Algolia HN Search API: company pitch, location, text and author, straight from the source. No login, no browser. |
| [Greenhouse, Lever, Ashby & Workable Scraper](https://apify.com/bibian/multi-ats-jobs-scraper) | Extract job postings from company career pages hosted on Greenhouse, Lever, Ashby or Workable in one run: title, department, location, remote policy, employment type and full description. |
| [Recruitee, Personio & Teamtailor Jobs Scraper](https://apify.com/bibian/multi-ats-jobs-2-scraper) | Extract job postings from company career pages hosted on Recruitee, Personio or Teamtailor in one run: title, department, location, remote policy, salary when published and full description. |
| [Breezy HR, Pinpoint & JazzHR Jobs Scraper](https://apify.com/bibian/multi-ats-jobs-3-scraper) | Extract job postings from company career pages hosted on Breezy HR, Pinpoint or JazzHR in one run: title, department, location, remote policy, employment type, salary and full description. |
| [Workday Jobs Scraper · Any Career Site](https://apify.com/bibian/workday-jobs-scraper) | Extract job postings from any company career site hosted on Workday (myworkdayjobs.com): title, locations, employment type, posting date, requisition ID and full description. |
| [BambooHR Jobs Scraper · Any Company](https://apify.com/bibian/bamboohr-jobs-scraper) | Extract job postings from any company's public BambooHR careers board: title, department, location, employment status, posting date and full description, by company subdomain. |
| [Universal Job Postings Scraper · Any Job Site](https://apify.com/bibian/universal-job-postings-scraper) | Extract job postings from any job board or company career site that publishes schema.org JobPosting data: title, company, location, remote, salary range, contract type and full description. Give domains, the actor finds the offers through their sitemaps. |

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account, or `Authorization: Bearer <APIFY_TOKEN>`):

```
https://mcp.apify.com?tools=bibian/remote-jobs-worldwide-scraper,bibian/remoteok-jobs-scraper,bibian/remotive-jobs-scraper,bibian/weworkremotely-jobs-scraper,bibian/workingnomads-jobs-scraper,bibian/jobicy-jobs-scraper,bibian/hackernews-jobs-scraper,bibian/multi-ats-jobs-scraper,bibian/multi-ats-jobs-2-scraper,bibian/multi-ats-jobs-3-scraper,bibian/workday-jobs-scraper,bibian/bamboohr-jobs-scraper,bibian/universal-job-postings-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-remote-ats-jobs": {
      "url": "https://mcp.apify.com?tools=bibian/remote-jobs-worldwide-scraper,bibian/remoteok-jobs-scraper,bibian/remotive-jobs-scraper,bibian/weworkremotely-jobs-scraper,bibian/workingnomads-jobs-scraper,bibian/jobicy-jobs-scraper,bibian/hackernews-jobs-scraper,bibian/multi-ats-jobs-scraper,bibian/multi-ats-jobs-2-scraper,bibian/multi-ats-jobs-3-scraper,bibian/workday-jobs-scraper,bibian/bamboohr-jobs-scraper,bibian/universal-job-postings-scraper"
    }
  }
}
```

Each tool is pay per result on Apify: you only pay for the rows you get. Missing a site, a field or a filter? Open an issue on the tool's Apify page.
