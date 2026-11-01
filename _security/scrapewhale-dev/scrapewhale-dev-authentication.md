---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scrapewhale-dev-openapi.json
  format: json
  label: ScrapeWhale API
  slug: scrapewhale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapewhale-dev/openapi/scrapewhale-dev-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Scrapewhale Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: scrapewhale-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: scrapewhale-dev
provider_slug: scrapewhale-dev
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: API key from /settings/apikeys.
  scheme: bearer
  type: http
- description: API key from /settings/apikeys (alternative header).
  in: header
  name: x-api-key
  type: apiKey
slug: scrapewhale-dev-authentication
source_filename: scrapewhale-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://scrapewhale.dev/openapi.json\nname: ScrapeWhale authentication\nschemes:\n  - type: http\n    scheme: bearer\n    description: API key from /settings/apikeys.\n    bearerFormat: JWT\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: API key from /settings/apikeys (alternative header)."
source_yaml_url: https://artifacts.apis.io/scrapewhale-dev/authentication/scrapewhale-dev-authentication.yml
summary_line: 2 schemes
tags:
- Data
- Marketing
- API
- WebScraping
- AI
---
