---
api_key_in:
- query
api_specs:
- filename: scrapingant-scraping-api-openapi.yml
  format: yaml
  label: ScrapingAnt Scraping API
  slug: scrapingant-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/openapi/scrapingant-scraping-api-openapi.yml
- filename: scrapingant-usage-api-openapi.yml
  format: yaml
  label: ScrapingAnt Usage API
  slug: scrapingant-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/openapi/scrapingant-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scrapingant Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScrapingAnt secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ScrapingAnt
provider_slug: scrapingant
scheme_count: 1
schemes:
- description: ScrapingAnt API key, passed as the x-api-key query parameter. The provider also accepts it as an x-api-key request header (docs.scrapingant.com/request-response-format).
  in: query
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/scrapingant-scraping-api-openapi.yml
  - openapi/scrapingant-usage-api-openapi.yml
  type: apiKey
slug: scrapingant-authentication
source_filename: scrapingant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/scrapingant-scraping-api-openapi.yml, openapi/scrapingant-usage-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: x-api-key\n  description: ScrapingAnt API key, passed as the x-api-key query parameter. The provider also\n    accepts it as an x-api-key request header (docs.scrapingant.com/request-response-format).\n  sources:\n  - openapi/scrapingant-scraping-api-openapi.yml\n  - openapi/scrapingant-usage-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/authentication/scrapingant-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Extraction
- Proxies
- Scraping
- Web Scraping
- Headless Browsers
- AI Agents
- MCP
- LLM
- Data Collection
- Web Data
---
