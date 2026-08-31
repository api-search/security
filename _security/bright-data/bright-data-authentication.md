---
api_key_in: []
api_specs:
- filename: bright-data-access-api-openapi.yml
  format: yaml
  label: Bright Data Access API
  slug: bright-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-access-api-openapi.yml
- filename: bright-data-archive-api-openapi.yml
  format: yaml
  label: Bright Data Archive API
  slug: bright-data-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-archive-api-openapi.yml
- filename: bright-data-billing-api-openapi.yml
  format: yaml
  label: Bright Data Billing API
  slug: bright-data-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-billing-api-openapi.yml
- filename: bright-data-datasets-api-openapi.yml
  format: yaml
  label: Bright Data Datasets API
  slug: bright-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-datasets-api-openapi.yml
- filename: bright-data-delivery-api-openapi.yml
  format: yaml
  label: Bright Data Delivery API
  slug: bright-data-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-delivery-api-openapi.yml
- filename: bright-data-ips-api-openapi.yml
  format: yaml
  label: Bright Data IPs API
  slug: bright-data-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-ips-api-openapi.yml
- filename: bright-data-lookup-api-openapi.yml
  format: yaml
  label: Bright Data Lookup API
  slug: bright-data-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-lookup-api-openapi.yml
- filename: bright-data-proxies-api-openapi.yml
  format: yaml
  label: Bright Data Proxies API
  slug: bright-data-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-proxies-api-openapi.yml
- filename: bright-data-scrape-api-openapi.yml
  format: yaml
  label: Bright Data Scrape API
  slug: bright-data-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-scrape-api-openapi.yml
- filename: bright-data-sessions-api-openapi.yml
  format: yaml
  label: Bright Data Sessions API
  slug: bright-data-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-sessions-api-openapi.yml
- filename: bright-data-shield-api-openapi.yml
  format: yaml
  label: Bright Data Shield API
  slug: bright-data-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-shield-api-openapi.yml
- filename: bright-data-snapshots-api-openapi.yml
  format: yaml
  label: Bright Data Snapshots API
  slug: bright-data-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-snapshots-api-openapi.yml
- filename: bright-data-tokens-api-openapi.yml
  format: yaml
  label: Bright Data Tokens API
  slug: bright-data-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-tokens-api-openapi.yml
- filename: bright-data-unlock-api-openapi.yml
  format: yaml
  label: Bright Data Unlock API
  slug: bright-data-unlock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-unlock-api-openapi.yml
- filename: bright-data-zones-api-openapi.yml
  format: yaml
  label: Bright Data Zones API
  slug: bright-data-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-data/refs/heads/main/openapi/bright-data-zones-api-openapi.yml
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
