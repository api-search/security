---
api_key_in: []
api_specs:
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Web Scraper API
  slug: brightdata-web-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data SERP API
  slug: brightdata-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Web Unlocker API
  slug: brightdata-web-unlocker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Proxy & Zone Management API
  slug: brightdata-proxy-zone-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Datasets API
  slug: brightdata-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
- filename: brightdata-openapi.yml
  format: yaml
  label: Bright Data Browser API (Scraping Browser)
  slug: brightdata-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/openapi/brightdata-openapi.yml
auth_types:
- http
- userPassword
description: ''
kind: authentication
layout: security
method: derived
name: Brightdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bright Data secures its APIs with http and userPassword across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bright Data
provider_slug: brightdata
scheme_count: 2
schemes:
- bearerFormat: apiKey
  description: 'Bright Data platform API token from the control panel, sent as ''Authorization: Bearer <API_KEY>'' on all api.brightdata.com REST calls (Web Scraper, SERP, Web Unlocker, Zones, Browser API session).'
  name: api_token
  scheme: bearer
  sources:
  - openapi/brightdata-openapi.yml
  type: http
- description: Proxy and Scraping Browser zones authenticate with zone credentials (username 'brd-customer-<CUSTOMER_ID>-zone-<ZONE>' and the zone password). For the Scraping Browser these are embedded in the CDP WebSocket URL userinfo ('wss://...@brd.superproxy.io:9222'); for proxy traffic they are sent as HTTP(S)/SOCKS proxy credentials against brd.superproxy.io.
  name: zone_credentials
  sources:
  - asyncapi/brightdata-asyncapi.yml
  type: userPassword
slug: brightdata-authentication
source_filename: brightdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/brightdata-openapi.yml\nsummary:\n  types:\n  - http\n  - userPassword\nschemes:\n- name: api_token\n  type: http\n  scheme: bearer\n  bearerFormat: apiKey\n  description: >-\n    Bright Data platform API token from the control panel, sent as\n    'Authorization: Bearer <API_KEY>' on all api.brightdata.com REST calls\n    (Web Scraper, SERP, Web Unlocker, Zones, Browser API session).\n  sources:\n  - openapi/brightdata-openapi.yml\n- name: zone_credentials\n  type: userPassword\n  description: >-\n    Proxy and Scraping Browser zones authenticate with zone credentials\n    (username 'brd-customer-<CUSTOMER_ID>-zone-<ZONE>' and the zone password).\n    For the Scraping Browser these are embedded in the CDP WebSocket URL\n    userinfo ('wss://...@brd.superproxy.io:9222'); for proxy traffic they are\n    sent as HTTP(S)/SOCKS proxy credentials against brd.superproxy.io.\n  sources:\n  - asyncapi/brightdata-asyncapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightdata/refs/heads/main/authentication/brightdata-authentication.yml
summary_line: http/userPassword · 2 schemes
tags:
- Web Data
- Web Scraping
- Web Intelligence
- Proxy
- Data Extraction
- SERP
- Web Unlocker
- Datasets
- Data Collection
- Browser Automation
---
