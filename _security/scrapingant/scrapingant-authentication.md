---
api_key_in:
- query
api_specs:
- filename: scrapingant-openapi.yml
  format: yaml
  label: ScrapingAnt
  slug: scrapingant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/openapi/scrapingant-openapi.yml
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
- description: ScrapingAnt API key (also accepted as header x-api-key).
  in: query
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/scrapingant-openapi.yml
  type: apiKey
slug: scrapingant-authentication
source_filename: scrapingant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scrapingant-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: x-api-key\n  description: ScrapingAnt API key (also accepted as header x-api-key).\n  sources:\n  - openapi/scrapingant-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingant/refs/heads/main/authentication/scrapingant-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Extraction
- Proxies
- Scraping
---
