# Job Boards MCP Server: 35 job sites, 50+ countries

One `search_jobs` tool over 35 public job boards: France Travail, Free-Work, HelloWork, Arbeitsagentur, Reed, Infoempleo, EURES (every EU and EEA country), Computrabajo, Bumeran, Gupy, Job Bank, Dice, Built In, MyCareersFuture, RemoteOK, Remotive, We Work Remotely and more. Give a country code or `REMOTE` plus keywords; get title, company, location, work mode, salary when published, date posted and the posting URL, deduplicated across boards. A free `list_job_sources` tool lists the boards per country.

Unlike the themed servers in this repository, this one is a single MCP server with two tools, running on Apify Standby: [apify.com/bibian/job-boards-mcp-server](https://apify.com/bibian/job-boards-mcp-server).

## Connect

```
https://bibian--job-boards-mcp-server.apify.actor/mcp
```

Header `Authorization: Bearer <APIFY_TOKEN>`.

```json
{
  "mcpServers": {
    "job-boards": {
      "url": "https://bibian--job-boards-mcp-server.apify.actor/mcp",
      "headers": { "Authorization": "Bearer <APIFY_TOKEN>" }
    }
  }
}
```

$0.002 per job returned, plus a $0.005 start fee per session (a session lasts up to 100 seconds); a search with no result adds nothing. Public pages and public APIs only, no personal data.
