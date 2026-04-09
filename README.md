# Reed Scraper

> Extract UK job listings from Reed.co.uk -- Britain's top job site with 250,000+ live jobs

[![Try on Apify](https://img.shields.io/badge/Try_on-Apify_Store-00C853?style=for-the-badge)](https://apify.com/thirdwatch)
[![Website](https://img.shields.io/badge/Website-thirdwatch.dev-000?style=for-the-badge)](https://thirdwatch.dev)

## What it does

Scrapes Reed.co.uk for UK job listings with salaries, descriptions, and employer details. Extracts comprehensive job data including salary ranges, benefits, required qualifications, and application deadlines. The go-to scraper for UK employment market data.

## Output fields

| Field | Type | Description |
|-------|------|-------------|
| title | String | Job title |
| company | String | Employer name |
| location | String | UK location |
| salary | Object | Salary (min, max, currency, period) |
| description | String | Full job description |
| jobType | String | Permanent, temporary, contract |
| sector | String | Industry sector |
| postedDate | String | Posting date |
| expiryDate | String | Application deadline |
| url | String | Direct listing URL |

## Input parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| queries | Array | Job search keywords |
| location | String | UK city or region |
| maxResults | Number | Maximum results per query |
| salaryFrom | Number | Minimum salary filter |

## Example output

```json
{
  "title": "Full Stack Developer",
  "company": "Deloitte",
  "location": "Manchester, UK",
  "salary": {
    "min": 45000,
    "max": 65000,
    "currency": "GBP",
    "period": "yearly"
  },
  "description": "Join our digital team as a Full Stack Developer...",
  "jobType": "Permanent",
  "sector": "IT & Telecoms",
  "postedDate": "2026-04-06",
  "expiryDate": "2026-05-06",
  "url": "https://www.reed.co.uk/jobs/..."
}
```

## Pricing

| Plan | Price |
|------|-------|
| Pay per result | $0.002/result |
| Free tier | Available on Apify |

## Use cases

- UK job market research and salary analysis
- Build UK-focused job board platforms
- Track hiring trends across British industries
- Graduate job market monitoring
- Recruitment agency lead generation

## Getting started

1. Go to the [Apify Store](https://apify.com/thirdwatch)
2. Find the **Reed Scraper**
3. Enter job keywords and UK location
4. Run and download results as JSON, CSV, or Excel

## Related scrapers by Thirdwatch

- [Adzuna Scraper](https://github.com/thirdwatch-dev/adzuna-scraper) -- 19 country job search
- [Indeed Scraper](https://github.com/thirdwatch-dev/indeed-scraper) -- Indeed job listings
- [LinkedIn Jobs Scraper](https://github.com/thirdwatch-dev/linkedin-jobs-scraper) -- LinkedIn jobs
- [Glassdoor Scraper](https://github.com/thirdwatch-dev/glassdoor-scraper) -- Glassdoor jobs + salary
- [Career Site Scraper](https://github.com/thirdwatch-dev/career-site-scraper) -- Lever/Greenhouse/Workday

## About Thirdwatch

[Thirdwatch](https://thirdwatch.dev) builds production-ready web scraping APIs. 18 scrapers for jobs, e-commerce, reviews, social media, and business data.

## License

MIT
