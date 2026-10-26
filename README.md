# Jobs and market data MCP server

An MCP server that lets an AI assistant search **public job postings and market data** in the countries and sectors that the big English-language job APIs cover poorly: France, Germany, Spain, Latin America, plus French movie and crowdfunding data. It is a remote server hosted by [Apify](https://apify.com/mcp), exposing seven Actors maintained by [bibian](https://apify.com/bibian).

## Tools

| Tool (Apify Actor) | What it returns |
|---|---|
| [free-work-jobs-scraper](https://apify.com/bibian/free-work-jobs-scraper) | French IT jobs and freelance missions, with daily rates (TJM), skills and remote mode |
| [arbeitsagentur-jobs-scraper](https://apify.com/bibian/arbeitsagentur-jobs-scraper) | German postings from the Bundesagentur fuer Arbeit, with salary when disclosed |
| [infoempleo-jobs-scraper](https://apify.com/bibian/infoempleo-jobs-scraper) | Spanish postings with salary range, region and contract type |
| [latam-jobs-bumeran-scraper](https://apify.com/bibian/latam-jobs-bumeran-scraper) | Bumeran, Zonajobs, Laborum and sister sites: Argentina, Chile, Peru, Ecuador, Panama |
| [codeur-projects-scraper](https://apify.com/bibian/codeur-projects-scraper) | French freelance projects from Codeur.com with budget and brief |
| [allocine-movies-scraper](https://apify.com/bibian/allocine-movies-scraper) | Movies now playing in France, ratings, showtimes count |
| [kisskissbankbank-projects-scraper](https://apify.com/bibian/kisskissbankbank-projects-scraper) | Crowdfunding projects: amount, goal, backers, dates |

No login on the source sites, public pages only, no personal data.

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account):

```
https://mcp.apify.com?tools=bibian/free-work-jobs-scraper,bibian/arbeitsagentur-jobs-scraper,bibian/infoempleo-jobs-scraper,bibian/latam-jobs-bumeran-scraper,bibian/codeur-projects-scraper,bibian/allocine-movies-scraper,bibian/kisskissbankbank-projects-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-data": {
      "url": "https://mcp.apify.com?tools=bibian/free-work-jobs-scraper,bibian/arbeitsagentur-jobs-scraper,bibian/infoempleo-jobs-scraper,bibian/latam-jobs-bumeran-scraper,bibian/codeur-projects-scraper,bibian/allocine-movies-scraper,bibian/kisskissbankbank-projects-scraper"
    }
  }
}
```

The first connection opens an Apify sign-in. You can also send `Authorization: Bearer <APIFY_TOKEN>` if your client prefers a token.

## Cost

Each Actor is billed per result on **your** Apify account, from $0.001 to $0.005 per result plus $0.01 per run start. A 50-result call costs about $0.07 to $0.30 depending on the Actor. Apify's free plan includes monthly credits.

## Also available as REST APIs

[Free-Work Jobs](https://rapidapi.com/VivienMORVAN/api/free-work-jobs), [German Jobs Arbeitsagentur](https://rapidapi.com/VivienMORVAN/api/german-jobs-arbeitsagentur), [Spain Jobs Infoempleo](https://rapidapi.com/VivienMORVAN/api/spain-jobs-infoempleo), [LatAm Jobs Bumeran](https://rapidapi.com/VivienMORVAN/api/latam-jobs-bumeran-zonajobs-laborum), [Codeur](https://rapidapi.com/VivienMORVAN/api/codeur-freelance-projects-france), [AlloCine](https://rapidapi.com/VivienMORVAN/api/allocine-movies-france), [KissKissBankBank](https://rapidapi.com/VivienMORVAN/api/kisskissbankbank-crowdfunding-projects) on RapidAPI.

## Notes

Unofficial tool, not affiliated with the sites it reads. Check each site's terms and the data protection rules that apply to your use.

License: MIT.
