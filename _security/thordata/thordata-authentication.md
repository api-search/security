---
api_key_in:
- header
api_specs:
- filename: thordata-locations-api-openapi.yml
  format: yaml
  label: Thordata Locations API
  slug: thordata-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-locations-api-openapi.yml
- filename: thordata-proxy-extract-api-openapi.yml
  format: yaml
  label: Thordata Proxy IP Extract API
  slug: thordata-proxy-ip-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-proxy-extract-api-openapi.yml
- filename: thordata-account-api-openapi.yml
  format: yaml
  label: Thordata Account API
  slug: thordata-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-account-api-openapi.yml
- filename: thordata-proxy-api-openapi.yml
  format: yaml
  label: Thordata Proxy API
  slug: thordata-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-proxy-api-openapi.yml
- filename: thordata-proxy-users-api-openapi.yml
  format: yaml
  label: Thordata Proxy Users API
  slug: thordata-proxy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-proxy-users-api-openapi.yml
- filename: thordata-serp-api-api-openapi.yml
  format: yaml
  label: Thordata SERP API
  slug: thordata-serp-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-serp-api-api-openapi.yml
- filename: thordata-tasks-api-openapi.yml
  format: yaml
  label: Thordata Tasks API
  slug: thordata-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-tasks-api-openapi.yml
- filename: thordata-universal-scraping-api-api-openapi.yml
  format: yaml
  label: Thordata Universal Scraping API
  slug: thordata-universal-scraping-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-universal-scraping-api-api-openapi.yml
- filename: thordata-web-scraper-api-api-openapi.yml
  format: yaml
  label: Thordata Web Scraper API
  slug: thordata-web-scraper-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-web-scraper-api-api-openapi.yml
- filename: thordata-whitelist-api-openapi.yml
  format: yaml
  label: Thordata Whitelist API
  slug: thordata-whitelist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/openapi/thordata-whitelist-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Thordata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thordata secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Thordata
provider_slug: thordata
scheme_count: 3
schemes:
- description: Public token (THORDATA_PUBLIC_TOKEN) from the Thordata Dashboard.
  in: header
  name: PublicToken
  parameter: token
  sources:
  - openapi/thordata-locations-api-openapi.yml
  - openapi/thordata-public-api-openapi.yml
  - openapi/thordata-scraper-api-openapi.yml
  - openapi/thordata-universal-api-openapi.yml
  - openapi/thordata-web-scraper-tasks-openapi.yml
  type: apiKey
- description: Public key (THORDATA_PUBLIC_KEY) from the Thordata Dashboard.
  in: header
  name: PublicKey
  parameter: key
  sources:
  - openapi/thordata-locations-api-openapi.yml
  - openapi/thordata-public-api-openapi.yml
  - openapi/thordata-scraper-api-openapi.yml
  - openapi/thordata-web-scraper-tasks-openapi.yml
  type: apiKey
- bearerFormat: Token
  description: Scraper token (THORDATA_SCRAPER_TOKEN) from Dashboard > Account Settings.
  name: ScraperBearer
  scheme: bearer
  sources:
  - openapi/thordata-scraper-api-openapi.yml
  - openapi/thordata-universal-api-openapi.yml
  type: http
slug: thordata-authentication
source_filename: thordata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://raw.githubusercontent.com/Thordata/thordata-sdk-spec/main/v1.json (auth block); openapi/ derived\n  specs; https://doc.thordata.com/doc/scraping/serp-api/configuration\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  credential_pairs:\n  - name: scraperToken\n    env: THORDATA_SCRAPER_TOKEN\n    used_by:\n    - SERP API\n    - Web Unlocker\n    - Universal Scraping API\n    - Web Scraper builder\n    - Video builder\n    source: Dashboard > API Playground > Token\n  - name: publicToken\n    env: THORDATA_PUBLIC_TOKEN\n    used_by:\n    - Public API\n    - Locations API\n    - Web Scraper tasks\n    source: Dashboard\n  - name: publicKey\n    env: THORDATA_PUBLIC_KEY\n    used_by:\n    - Public API\n    - Locations API\n    - Web Scraper tasks\n    source: Dashboard\n  - name: browserUsername / browserPassword\n    env: THORDATA_BROWSER_USERNAME / THORDATA_BROWSER_PASSWORD\n    used_by:\n    -\
  \ Scraping Browser CDP connection\n    source: Dashboard > Scraping Browser > Users\nschemes:\n- name: PublicToken\n  type: apiKey\n  in: header\n  parameter: token\n  description: Public token (THORDATA_PUBLIC_TOKEN) from the Thordata Dashboard.\n  sources:\n  - openapi/thordata-locations-api-openapi.yml\n  - openapi/thordata-public-api-openapi.yml\n  - openapi/thordata-scraper-api-openapi.yml\n  - openapi/thordata-universal-api-openapi.yml\n  - openapi/thordata-web-scraper-tasks-openapi.yml\n- name: PublicKey\n  type: apiKey\n  in: header\n  parameter: key\n  description: Public key (THORDATA_PUBLIC_KEY) from the Thordata Dashboard.\n  sources:\n  - openapi/thordata-locations-api-openapi.yml\n  - openapi/thordata-public-api-openapi.yml\n  - openapi/thordata-scraper-api-openapi.yml\n  - openapi/thordata-web-scraper-tasks-openapi.yml\n- name: ScraperBearer\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  description: Scraper token (THORDATA_SCRAPER_TOKEN) from Dashboard > Account\
  \ Settings.\n  sources:\n  - openapi/thordata-scraper-api-openapi.yml\n  - openapi/thordata-universal-api-openapi.yml\ndocs: https://doc.thordata.com/doc/scraping/serp-api/configuration\nnon_http_auth:\n- surface: Proxy gateway (residential / ISP / datacenter / mobile / high-bandwidth)\n  mechanism: proxy Basic auth\n  credential: username:password, with the td-customer- prefix and product/session modifiers encoded in the username\n  hosts:\n  - pr.thordata.net\n  - t.pr.thordata.net\n  - t.na.thordata.net\n  - t.eu.thordata.net\n  - t.as.thordata.net\n  - dc.pr.thordata.net\n  - m.pr.thordata.net\n  - isp.pr.thordata.net\n  ports:\n    residential: 9999\n    isp: 6666\n    datacenter: 7777\n    mobile: 5555\n  protocols:\n  - https (required by most accounts)\n  - socks5h\n  - http (deprecated, generally rejected)\n  alternative: IP whitelisting via /whitelisted-ips/add-ip removes the need for per-request credentials\n  docs: https://doc.thordata.com/doc/proxies/residential-proxies/user-and-pass-auth\n\
  \  note: Not expressible as an OpenAPI securityScheme - this is transport-layer proxy auth, not API auth.\n- surface: SERP API proxy-based access\n  mechanism: proxy Basic auth against scraping.thordata.com:30001\n  credential: td-customer-serp_USERNAME:PASSWORD\n  docs: https://doc.thordata.com/doc/scraping/serp-api/configuration\n- surface: Scraping Browser\n  mechanism: credentials embedded in a Chrome DevTools Protocol websocket connection URL\n  note: Consumed by Puppeteer / Playwright / Selenium; sub-users are created in the dashboard.\n  docs: https://doc.thordata.com/doc/scraping/scraping-browser/getting-started\nnotes:\n- Two independent credential families. The scraper token authenticates collection endpoints; the publicToken + publicKey\n  pair authenticates account, proxy and task-lifecycle endpoints.\n- The Web Scraper builder endpoints require ALL THREE (Authorization bearer + token + key headers).\n- SERP and Web Unlocker accept the scraper token either as an Authorization\
  \ bearer or in a bare token header.\n- No OAuth 2.0 or OpenID Connect surface exists anywhere in the Thordata platform, so there is no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thordata/refs/heads/main/authentication/thordata-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Proxy network
- Web Scraping
- Data Extraction
- SERP
- Search data
- Web unblocking
- Residential Proxies
- Mobile Proxies
- ISP Proxies
- Datacenter Proxies
- Scraping Browser
- Data-for-AI
- RAG data pipelines
- Web Data
---
