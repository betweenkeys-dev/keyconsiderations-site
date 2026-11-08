# Key Considerations site

Static site for Key Considerations, Juanita Perry's Maryland and DC real estate platform. Plain HTML and CSS, served by GitHub Pages from the `main` branch root. No build step.

## Structure

- `index.html`: home page
- `lunch-and-learn/`: one page per Lunch and Learn clip article
- `assets/styles.css`: all styles, colors defined as variables at the top
- `assets/img/`: logo sizes and icons

## Adding a Lunch and Learn article

1. Copy `lunch-and-learn/gcaar-contract-changes.html` to a new file named after the topic.
2. Replace the bracketed placeholders and the YouTube embed.
3. On `index.html`, link the episode title in the series list and change its pill from "In production" to "Watch now".

## Before going live on the custom domain

- [ ] Confirm the Substack address. Links currently point to a placeholder Substack URL.
- [ ] Move Substack to a subdomain first, so the newsletter keeps working when the root domain moves here.
- [ ] Fill in the brokerage disclosure (office address, phone, license numbers) using eXp's approved wording.
- [ ] Add a `CNAME` file containing the root domain, set the custom domain in Settings > Pages, then update DNS:
  - `A` records for the root: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
  - `CNAME` for `www`: betweenkeys-dev.github.io
- [ ] Turn on "Enforce HTTPS" once the certificate is issued.

## Writing rules

Copy follows Juanita's voice rules in the Key Considerations Master Reference: no em dashes, no absolutes, no slang, warm but controlled.
