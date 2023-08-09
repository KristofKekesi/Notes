This file is used by crawler bots to link the internet together or to collect datasets.

- ==Must be located in the root directory of the website!==
- ==The file is case-sensitive, use lowercase letters with uppercase first letters!==
- Use UTF-8 coding (set by default)

## Instructions and terms
### User-agent
User-agent is used link the instructions below to a specific bot.  There's a list of bots online but it's incomplete (checked 2023-08-09).

==To select all bots use: \*==
Example:
`User-agent: Googlebot`

Most important bots are:
- Googlebot (Google)
- Googlebot-Image (Google)
- Googlebot-News (Google)
- Googlebot-Video (Google)
- Googlebot-Mobile (Google)
- AdsBot-Google (Google)
- DuckDuckBot (DuckDuckGo)
- Applebot (Apple)
- Bingbot (Microsoft)
- msnbot (Microsoft)
- Twitterbot/1.0 (Twitter)
- ==GPTBot (ChatGPT)==

### Disallow
Use to disallow bots from crawling any content on your website. This can be any page, photo, video, file or even directory.

- \*: With an asterix you stand any number or character
- $: Stands for the end of the line (useful for file extensions)

Example:
`Disallow: /`

### Allow
Use to allow bots permission to crawl content on your website. ==Allows disallowed content to crawl even if you disallow below!==

### Sitemap
You can link your site's sitemap. It's optional but I highly recommend using it.
	You can also link your sitemap in your HTML and in Google Search Console. Recommend using both. You can even remove your assets from Google with Google Search Console after crawling.

==Allways use whole URL!==

Example
`Sitemap: https://www.example.com/sitemap.xml`

## Examples
### Disallow everything
```
User-agent: *
Disallow: /
```
==For more privacy use the HTML meta tag as well.==
	`<meta name='robots' content='noindex,follow' />`

