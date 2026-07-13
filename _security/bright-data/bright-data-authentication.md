---
api_key_in: []
api_specs:
- filename: bright-data-web-unlocker-api-openapi.yml
  format: yaml
  label: Bright Data Web Unlocker API
  slug: web-unlocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-unlocker-api-openapi.yml
- filename: bright-data-serp-api-openapi.yml
  format: yaml
  label: Bright Data SERP API
  slug: serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-serp-api-openapi.yml
- filename: bright-data-web-scraper-api-openapi.yml
  format: yaml
  label: Bright Data Web Scraper API
  slug: web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-scraper-api-openapi.yml
- filename: bright-data-scraping-browser-api-openapi.yml
  format: yaml
  label: Bright Data Scraping Browser API
  slug: scraping-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scraping-browser-api-openapi.yml
- filename: bright-data-deep-lookup-api-openapi.yml
  format: yaml
  label: Bright Data Deep Lookup API
  slug: deep-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-deep-lookup-api-openapi.yml
- filename: bright-data-web-archive-api-openapi.yml
  format: yaml
  label: Bright Data Web Archive API
  slug: web-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-web-archive-api-openapi.yml
- filename: bright-data-dataset-marketplace-api-openapi.yml
  format: yaml
  label: Bright Data Dataset Marketplace API
  slug: dataset-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-dataset-marketplace-api-openapi.yml
- filename: bright-data-account-management-api-openapi.yml
  format: yaml
  label: Bright Data Account Management API
  slug: account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-account-management-api-openapi.yml
- filename: bright-data-proxy-manager-api-openapi.yml
  format: yaml
  label: Bright Data Proxy Manager API
  slug: proxy-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-proxy-manager-api-openapi.yml
- filename: bright-data-scraping-shield-api-openapi.yml
  format: yaml
  label: Bright Data Scraping Shield API
  slug: scraping-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scraping-shield-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bright Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bright Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bright Data
provider_slug: bright-data
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/bright-data-account-management-api-openapi.yml
  - openapi/bright-data-dataset-marketplace-api-openapi.yml
  - openapi/bright-data-deep-lookup-api-openapi.yml
  - openapi/bright-data-scraping-browser-api-openapi.yml
  - openapi/bright-data-scraping-shield-api-openapi.yml
  - openapi/bright-data-serp-api-openapi.yml
  - openapi/bright-data-web-archive-api-openapi.yml
  - openapi/bright-data-web-scraper-api-openapi.yml
  - openapi/bright-data-web-unlocker-api-openapi.yml
  type: http
slug: bright-data-authentication
source_filename: bright-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bright-data-account-management-api-openapi.yml, openapi/bright-data-dataset-marketplace-api-openapi.yml,\n  openapi/bright-data-deep-lookup-api-openapi.yml, openapi/bright-data-scraping-browser-api-openapi.yml,\n  openapi/bright-data-scraping-shield-api-openapi.yml, openapi/bright-data-serp-api-openapi.yml,\n  openapi/bright-data-web-archive-api-openapi.yml, openapi/bright-data-web-scraper-api-openapi.yml,\n  openapi/bright-data-web-unlocker-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bright-data-account-management-api-openapi.yml\n  - openapi/bright-data-dataset-marketplace-api-openapi.yml\n  - openapi/bright-data-deep-lookup-api-openapi.yml\n  - openapi/bright-data-scraping-browser-api-openapi.yml\n  - openapi/bright-data-scraping-shield-api-openapi.yml\n  - openapi/bright-data-serp-api-openapi.yml\n  - openapi/bright-data-web-archive-api-openapi.yml\n\
  \  - openapi/bright-data-web-scraper-api-openapi.yml\n  - openapi/bright-data-web-unlocker-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/authentication/bright-data-authentication.yml
summary_line: http · 1 scheme
tags:
- Web Data
- Web Scraping
- Proxy
- Residential Proxy
- Datacenter Proxy
- ISP Proxy
- Mobile Proxy
- SERP
- Web Unlocker
- Scraping Browser
- Dataset Marketplace
- MCP
- AI Agents
---
