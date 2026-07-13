---
api_key_in:
- query
api_specs:
- filename: scrapingbee-openapi.yml
  format: yaml
  label: ScrapingBee HTML API
  slug: html-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapingbee/refs/heads/main/openapi/scrapingbee-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scrapingbee Authentication
name_suffix: Authentication
oauth_flows: []
overview: ScrapingBee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ScrapingBee
provider_slug: scrapingbee
scheme_count: 1
schemes:
- description: ScrapingBee account key, passed as a query parameter.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/scrapingbee-openapi.yml
  type: apiKey
slug: scrapingbee-authentication
source_filename: scrapingbee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scrapingbee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: ScrapingBee account key, passed as a query parameter.\n  sources:\n  - openapi/scrapingbee-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingbee/refs/heads/main/authentication/scrapingbee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Extraction
- Anti-Bot
- Data Aggregation
- Data Extraction
- Headless Browser
- JavaScript Rendering
- Proxy Rotation
- Screenshots
- Search Engine
- Web Scraping
---
