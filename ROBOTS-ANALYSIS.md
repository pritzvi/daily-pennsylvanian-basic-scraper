# Robots Analysis for the Daily Pennsylvanian

The Daily Pennsylvanian's `robots.txt` file is available at
[https://www.thedp.com/robots.txt](https://www.thedp.com/robots.txt).

## Contents of the `robots.txt` file on [ ... date you accessed the file ... ]

```
User-agent: *
Crawl-delay: 10
Allow: /

User-agent: SemrushBot
Disallow: /
```

## Explanation

This robots.txt file contains two directives for web crawlers. The first directive applies to all crawlers (User-agent: *) and requests they wait 10 seconds between page requests (Crawl-delay: 10) while allowing them to access all parts of the site (Allow: /). The second directive specifically targets SemrushBot (a commercial SEO crawling tool) and completely prohibits it from accessing any part of the website (Disallow: /). This configuration allows most search engines to index the site at a controlled rate while blocking a specific crawler that may be consuming too many resources.
