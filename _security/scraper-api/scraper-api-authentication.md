---
api_key_in:
- query
api_specs:
- filename: scraper-api-openapi.yml
  format: yaml
  label: ScraperAPI
  slug: scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scraper-api/refs/heads/main/openapi/scraper-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scraper Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScraperAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ScraperAPI
provider_slug: scraper-api
scheme_count: 1
schemes:
- description: ScraperAPI account key, passed as a query parameter.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/scraper-api-openapi.yml
  type: apiKey
slug: scraper-api-authentication
source_filename: scraper-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scraper-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: ScraperAPI account key, passed as a query parameter.\n  sources:\n  - openapi/scraper-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scraper-api/refs/heads/main/authentication/scraper-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Extraction
- Proxies
- Scraping
---
