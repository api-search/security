---
api_key_in:
- query
api_specs:
- filename: zenrows-universal-scraper-openapi.yml
  format: yaml
  label: ZenRows Universal Scraper API
  slug: universal-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/openapi/zenrows-universal-scraper-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zenrows Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZenRows secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ZenRows
provider_slug: zenrows
scheme_count: 1
schemes:
- description: ZenRows API key, passed as the `apikey` query parameter on every request.
  in: query
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/zenrows-universal-scraper-openapi.yml
  type: apiKey
slug: zenrows-authentication
source_filename: zenrows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenrows-universal-scraper-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: ZenRows API key, passed as the `apikey` query parameter on every request.\n  sources:\n  - openapi/zenrows-universal-scraper-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenrows/refs/heads/main/authentication/zenrows-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Scraping
- Data Extraction
- Anti-Bot
- Proxies
- Residential Proxies
- Browser Automation
- Screenshots
- CAPTCHA
- AI
- MCP
- Spain
---
