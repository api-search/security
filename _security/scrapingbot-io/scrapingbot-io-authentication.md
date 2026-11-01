---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scrapingbot-io-openapi-generated.yml
  format: yaml
  label: scrapingbot-io API
  slug: scrapingbot-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapingbot-io/openapi/_ae-authored/scrapingbot-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Scrapingbot Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: scrapingbot-io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: scrapingbot-io
provider_slug: scrapingbot-io
scheme_count: 3
schemes:
- description: API key header (recommended)
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: API_KEY
  description: Bearer token form of API key
  scheme: bearer
  type: http
- description: API key as query parameter (less secure)
  in: query
  name: api_key
  type: apiKey
slug: scrapingbot-io-authentication
source_filename: scrapingbot-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: \"https://scrapingbot.io/docs#authentication\"\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"API key header (recommended)\"\n  - type: http\n    scheme: bearer\n    bearerFormat: API_KEY\n    description: \"Bearer token form of API key\"\n  - type: apiKey\n    name: api_key\n    in: query\n    description: \"API key as query parameter (less secure)\"\n"
source_yaml_url: https://artifacts.apis.io/scrapingbot-io/authentication/scrapingbot-io-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Web Scraping
- API
- AI
- Data Extraction
- Automation
---
