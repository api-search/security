---
api_key_in:
- header
api_specs:
- filename: hyperbrowser-sessions-api-openapi.yml
  format: yaml
  label: Hyperbrowser Sessions API
  slug: sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-sessions-api-openapi.yml
- filename: hyperbrowser-profiles-api-openapi.yml
  format: yaml
  label: Hyperbrowser Profiles API
  slug: profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-profiles-api-openapi.yml
- filename: hyperbrowser-scrape-api-openapi.yml
  format: yaml
  label: Hyperbrowser Scrape API
  slug: scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-scrape-api-openapi.yml
- filename: hyperbrowser-crawl-api-openapi.yml
  format: yaml
  label: Hyperbrowser Crawl API
  slug: crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-crawl-api-openapi.yml
- filename: hyperbrowser-extract-api-openapi.yml
  format: yaml
  label: Hyperbrowser Extract API
  slug: extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-extract-api-openapi.yml
- filename: hyperbrowser-agents-api-openapi.yml
  format: yaml
  label: Hyperbrowser Agents API
  slug: agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-agents-api-openapi.yml
- filename: hyperbrowser-extensions-api-openapi.yml
  format: yaml
  label: Hyperbrowser Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-extensions-api-openapi.yml
- filename: hyperbrowser-web-api-openapi.yml
  format: yaml
  label: Hyperbrowser Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/openapi/hyperbrowser-web-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hyperbrowser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperbrowser secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hyperbrowser
provider_slug: hyperbrowser
scheme_count: 1
schemes:
- description: Account API key from app.hyperbrowser.ai
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/hyperbrowser-agents-api-openapi.yml
  - openapi/hyperbrowser-crawl-api-openapi.yml
  - openapi/hyperbrowser-extensions-api-openapi.yml
  - openapi/hyperbrowser-extract-api-openapi.yml
  - openapi/hyperbrowser-openapi.json
  - openapi/hyperbrowser-profiles-api-openapi.yml
  - openapi/hyperbrowser-scrape-api-openapi.yml
  - openapi/hyperbrowser-sessions-api-openapi.yml
  - openapi/hyperbrowser-web-api-openapi.yml
  type: apiKey
slug: hyperbrowser-authentication
source_filename: hyperbrowser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperbrowser-agents-api-openapi.yml, openapi/hyperbrowser-crawl-api-openapi.yml,\n  openapi/hyperbrowser-extensions-api-openapi.yml, openapi/hyperbrowser-extract-api-openapi.yml,\n  openapi/hyperbrowser-openapi.json, openapi/hyperbrowser-profiles-api-openapi.yml, openapi/hyperbrowser-scrape-api-openapi.yml,\n  openapi/hyperbrowser-sessions-api-openapi.yml, openapi/hyperbrowser-web-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Account API key from app.hyperbrowser.ai\n  sources:\n  - openapi/hyperbrowser-agents-api-openapi.yml\n  - openapi/hyperbrowser-crawl-api-openapi.yml\n  - openapi/hyperbrowser-extensions-api-openapi.yml\n  - openapi/hyperbrowser-extract-api-openapi.yml\n  - openapi/hyperbrowser-openapi.json\n  - openapi/hyperbrowser-profiles-api-openapi.yml\n  - openapi/hyperbrowser-scrape-api-openapi.yml\n\
  \  - openapi/hyperbrowser-sessions-api-openapi.yml\n  - openapi/hyperbrowser-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbrowser/refs/heads/main/authentication/hyperbrowser-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Headless Browser
- Browser Infrastructure
- Web Scraping
- Web Crawling
- Data Extraction
- AI Agents
- Browser Automation
- Computer Use
- Stealth
- Proxies
- CAPTCHA Solving
- MCP
- HyperAgent
- X402
---
