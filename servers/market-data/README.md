# Prices, property, cars, events and sports data (FR, ES, IT, AR, AU)

Grocery and book prices, hotels, property, used cars, events, tenders and sports scores. Remote MCP server hosted by [Apify](https://apify.com/mcp), 16 tools maintained by [bibian](https://apify.com/bibian). Public pages only, no login on the source sites, no personal data.

## Tools

| Tool | What it returns |
|---|---|
| [Woolworths Australia Scraper · No Browser](https://apify.com/bibian/woolworths-products-scraper) | Extract Woolworths Australia grocery products: name, brand, department, category, price, unit (cup) price and special offers, discovered via the product sitemap. |
| [ALDI Australia Scraper · Prices & Specials](https://apify.com/bibian/aldi-australia-products-scraper) | Extract ALDI Australia grocery products: name, brand, selling size, price, unit price and special offers, browsed by category across the whole catalogue. |
| [Precios Claros Argentina Supermarket Prices Scraper](https://apify.com/bibian/preciosclaros-prices-scraper) | Extract supermarket product prices from Precios Claros, Argentina's official government price transparency site: brand, presentation, min/max price and store availability near any location. |
| [Casa del Libro Books Scraper (Spain)](https://apify.com/bibian/casadellibro-books-scraper) | Extract book listings from Casa del Libro, a major Spanish bookstore: title, author, publisher, category, ISBN, format, page count, price, currency, stock status, language and publication date. |
| [Booking.com Scraper: Hotel Prices, No Login](https://apify.com/bibian/booking-hotels-scraper) | Extract hotel listings from Booking.com: price, availability, rating and reviews. |
| [Immonot Real Estate Scraper (France)](https://apify.com/bibian/immonot-real-estate-scraper) | Extract property listings from Immonot, the French notaries' real estate portal (about 25,000 ads): houses, flats, land and commercial premises for sale or rent, with price, areas, rooms, location and the notary office behind each ad. |
| [Studapart Student Housing Scraper (France)](https://apify.com/bibian/studapart-housing-scraper) | Extract student housing listings from Studapart by city: studios, shared flats and student residences with monthly rent, deposit, surface, furnishing, availability dates, amenities and description. |
| [Autosphere Used Cars Scraper (France)](https://apify.com/bibian/autosphere-cars-scraper) | Extract used car listings from Autosphere, a major French dealer network (about 15,000 used and demonstrator cars): brand, model, version, price, year, mileage, fuel, gearbox, dealership city, warranty and lease offer. |
| [Motor.es Used Cars Scraper (Spain)](https://apify.com/bibian/motor-es-cars-scraper) | Extract used car listings from Motor.es, a major Spanish car portal (over 40,000 ads): brand, model, version, price before and after discount, financed price, year, mileage, fuel, power, province and publication date. |
| [DeAutos Used Cars Scraper (Argentina)](https://apify.com/bibian/deautos-cars-scraper) | Extract used car listings from DeAutos.com, an Argentine aggregator of Mercado Libre, Autocosmos, Kavak and DeRuedas ads (about 1,400 cars): make, model, year, mileage, price in ARS or USD, province, body type, price rating and a link to the original ad. |
| [Leboncoin Scraper: Pro Car Listings, No Login](https://apify.com/bibian/leboncoin-cars-scraper) | Extract professional car listings from Leboncoin, France's largest classifieds site: brand, model, year, mileage, price, fuel, gearbox, dealer name and location. Dealers only, never a private seller. |
| [Subito.it Scraper · No Login Needed](https://apify.com/bibian/subito-classifieds-scraper) | Extract classified ads from Subito.it, one of Italy's largest classifieds sites: title, description, price, location and seller type, across any category or region. |
| [BilletReduc Events Scraper (France)](https://apify.com/bibian/billetreduc-events-scraper) | Extract discounted show and event listings from BilletReduc, a major French ticketing site: title, venue, city, dates, price range, category and rating. |
| [e-marchespublics.com Tender Scraper (French Public Procurement)](https://apify.com/bibian/e-marchespublics-tenders-scraper) | Extract French public procurement tenders (appels d'offres) from e-marchespublics.com: title, contracting authority, location, procedure type, submission deadline and a link to the full notice. |
| [ESPN Scraper: Scores, Schedules & Odds](https://apify.com/bibian/espn-scores-scraper) | Extract live scores, schedules and betting odds from ESPN's public API for NFL, NBA, WNBA, MLB, NHL, NCAA football, NCAA basketball and Premier League soccer. |
| [Tennis Explorer Scraper · Matches & Odds](https://apify.com/bibian/tennisexplorer-scraper) | Extract ATP and WTA tennis match results, upcoming matches and pre-match odds from Tennis Explorer: tournament, round players, set scores and betting odds for singles and doubles. |

## Connect

Server URL (Streamable HTTP, OAuth with your Apify account, or `Authorization: Bearer <APIFY_TOKEN>`):

```
https://mcp.apify.com?tools=bibian/woolworths-products-scraper,bibian/aldi-australia-products-scraper,bibian/preciosclaros-prices-scraper,bibian/casadellibro-books-scraper,bibian/booking-hotels-scraper,bibian/immonot-real-estate-scraper,bibian/studapart-housing-scraper,bibian/autosphere-cars-scraper,bibian/motor-es-cars-scraper,bibian/deautos-cars-scraper,bibian/leboncoin-cars-scraper,bibian/subito-classifieds-scraper,bibian/billetreduc-events-scraper,bibian/e-marchespublics-tenders-scraper,bibian/espn-scores-scraper,bibian/tennisexplorer-scraper
```

Claude Desktop, Cursor, VS Code and any client that supports remote MCP servers:

```json
{
  "mcpServers": {
    "bibian-market-data": {
      "url": "https://mcp.apify.com?tools=bibian/woolworths-products-scraper,bibian/aldi-australia-products-scraper,bibian/preciosclaros-prices-scraper,bibian/casadellibro-books-scraper,bibian/booking-hotels-scraper,bibian/immonot-real-estate-scraper,bibian/studapart-housing-scraper,bibian/autosphere-cars-scraper,bibian/motor-es-cars-scraper,bibian/deautos-cars-scraper,bibian/leboncoin-cars-scraper,bibian/subito-classifieds-scraper,bibian/billetreduc-events-scraper,bibian/e-marchespublics-tenders-scraper,bibian/espn-scores-scraper,bibian/tennisexplorer-scraper"
    }
  }
}
```

Each tool is pay per result on Apify: you only pay for the rows you get. Missing a site, a field or a filter? Open an issue on the tool's Apify page.
