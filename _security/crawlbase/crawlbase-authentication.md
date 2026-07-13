---
api_key_in: []
api_specs:
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Crawling API
  slug: crawlbase-crawling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Scraper API
  slug: crawlbase-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Cloud Storage API
  slug: crawlbase-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Screenshots API
  slug: crawlbase-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
- filename: crawlbase-openapi.yml
  format: yaml
  label: Crawlbase Leads API
  slug: crawlbase-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/openapi/crawlbase-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Crawlbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crawlbase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crawlbase
provider_slug: crawlbase
scheme_count: 1
schemes:
- description: 'Crawlbase authenticates every request with a `token` query parameter (for example `?token=YOUR_TOKEN`), not an Authorization header. Each account is issued two tokens: a Normal (TCP) token for static HTML/JSON responses, and a JavaScript token that renders the target in headless Chrome. The Scraper and Screenshots APIs require the JavaScript token when rendering is involved. The same token model applies across the Crawling, Scraper, Storage, Screenshots, and Leads products. Crawlbase also supports a proxy interface (smartproxy.crawlbase.com) where the token is supplied as the proxy username.'
  in: query
  name: tokenAuth
  parameterName: token
  sources:
  - https://crawlbase.com/docs/crawling-api/
  - https://crawlbase.com/docs/scraper-api/
  - https://crawlbase.com/docs/screenshots-api/
  tokenTypes:
  - name: Normal (TCP) token
    use: Static HTML/JSON pages; faster and cheaper.
  - name: JavaScript token
    use: SPAs, client-side rendering, lazy-loaded content, screenshots; renders in headless Chrome.
  type: apiKey
slug: crawlbase-authentication
source_filename: crawlbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://crawlbase.com/docs/crawling-api/\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameterName: token\n  description: >-\n    Crawlbase authenticates every request with a `token` query parameter (for\n    example `?token=YOUR_TOKEN`), not an Authorization header. Each account is\n    issued two tokens: a Normal (TCP) token for static HTML/JSON responses, and\n    a JavaScript token that renders the target in headless Chrome. The Scraper\n    and Screenshots APIs require the JavaScript token when rendering is involved.\n    The same token model applies across the Crawling, Scraper, Storage,\n    Screenshots, and Leads products. Crawlbase also supports a proxy interface\n    (smartproxy.crawlbase.com) where the token is supplied as the proxy username.\n  tokenTypes:\n  - name: Normal (TCP) token\n    use: Static HTML/JSON pages; faster and cheaper.\n  - name: JavaScript token\n\
  \    use: SPAs, client-side rendering, lazy-loaded content, screenshots; renders in headless Chrome.\n  sources:\n  - https://crawlbase.com/docs/crawling-api/\n  - https://crawlbase.com/docs/scraper-api/\n  - https://crawlbase.com/docs/screenshots-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlbase/refs/heads/main/authentication/crawlbase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Scraping
- Web Crawling
- Web Intelligence
- Data Extraction
- Proxy
- Scraper API
- Data Collection
- SERP
- Web Data
---
