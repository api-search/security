---
api_key_in:
- query
api_specs:
- filename: scrapfly-scrape-openapi.yml
  format: yaml
  label: Scrapfly Scrape API
  slug: scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapfly/refs/heads/main/openapi/scrapfly-scrape-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scrapfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scrapfly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scrapfly
provider_slug: scrapfly
scheme_count: 1
schemes:
- description: Scrapfly API key from your dashboard
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/scrapfly-scrape-openapi.yml
  type: apiKey
slug: scrapfly-authentication
source_filename: scrapfly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scrapfly-scrape-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Scrapfly API key from your dashboard\n  sources:\n  - openapi/scrapfly-scrape-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapfly/refs/heads/main/authentication/scrapfly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Data Extraction
- Screenshots
- Web Scraping
- Proxies
- Browser Automation
---
