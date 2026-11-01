---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kleinanzeigen-agent-de-ads-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Ads API
  slug: kleinanzeigen-agent-de-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-ads-api-openapi.yml
- filename: kleinanzeigen-agent-de-categories-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Categories API
  slug: kleinanzeigen-agent-de-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-categories-api-openapi.yml
- filename: kleinanzeigen-agent-de-history-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de History API
  slug: kleinanzeigen-agent-de-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-history-api-openapi.yml
- filename: kleinanzeigen-agent-de-locations-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Locations API
  slug: kleinanzeigen-agent-de-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-locations-api-openapi.yml
- filename: kleinanzeigen-agent-de-search-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Search API
  slug: kleinanzeigen-agent-de-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-search-api-openapi.yml
- filename: kleinanzeigen-agent-de-sellers-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Sellers API
  slug: kleinanzeigen-agent-de-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-sellers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kleinanzeigen Agent De Authentication
name_suffix: Authentication
oauth_flows: []
overview: kleinanzeigen-agent-de declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: kleinanzeigen-agent-de
provider_slug: kleinanzeigen-agent-de
scheme_count: 2
schemes:
- description: API key identifying your account, required for all requests.
  in: header
  name: klaz_key
  type: apiKey
- bearerFormat: JWT
  description: Optional Bearer token alternative for API key.
  scheme: bearer
  type: http
slug: kleinanzeigen-agent-de-authentication
source_filename: kleinanzeigen-agent-de-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://kleinanzeigen-agent.de/dokumentation.md\nschemes:\n  - type: apiKey\n    name: klaz_key\n    in: header\n    description: API key identifying your account, required for all requests.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Optional Bearer token alternative for API key.\n"
source_yaml_url: https://artifacts.apis.io/kleinanzeigen-agent-de/authentication/kleinanzeigen-agent-de-authentication.yml
summary_line: 2 schemes
tags:
- API
- Search
- Monitoring
- Market-Analysis
- Germany
- Kleinanzeigen
---
