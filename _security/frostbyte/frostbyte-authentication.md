---
api_key_in:
- header
- query
api_specs:
- filename: frostbyte-ip-geolocation-openapi.yml
  format: yaml
  label: Frostbyte IP Geolocation API
  slug: ip-geolocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-ip-geolocation-openapi.yml
- filename: frostbyte-crypto-prices-openapi.yml
  format: yaml
  label: Frostbyte Crypto Prices API
  slug: crypto-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-crypto-prices-openapi.yml
- filename: frostbyte-screenshot-openapi.yml
  format: yaml
  label: Frostbyte Screenshot API
  slug: screenshot
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-screenshot-openapi.yml
- filename: frostbyte-dns-lookup-openapi.yml
  format: yaml
  label: Frostbyte DNS Lookup API
  slug: dns-lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-dns-lookup-openapi.yml
- filename: frostbyte-web-scraper-openapi.yml
  format: yaml
  label: Frostbyte Web Scraper API
  slug: web-scraper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-web-scraper-openapi.yml
- filename: frostbyte-code-execution-openapi.yml
  format: yaml
  label: Frostbyte Code Execution API
  slug: code-execution
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-code-execution-openapi.yml
- filename: frostbyte-agent-gateway-openapi.yml
  format: yaml
  label: Frostbyte Agent Gateway (Full API)
  slug: agent-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/openapi/frostbyte-agent-gateway-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Frostbyte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frostbyte secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Frostbyte
provider_slug: frostbyte
scheme_count: 2
schemes:
- description: API key passed in header
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/frostbyte-agent-gateway-openapi.yml
  - openapi/frostbyte-code-execution-openapi.yml
  - openapi/frostbyte-crypto-prices-openapi.yml
  - openapi/frostbyte-dns-lookup-openapi.yml
  - openapi/frostbyte-ip-geolocation-openapi.yml
  - openapi/frostbyte-screenshot-openapi.yml
  - openapi/frostbyte-web-scraper-openapi.yml
  type: apiKey
- description: API key passed as query parameter
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/frostbyte-agent-gateway-openapi.yml
  - openapi/frostbyte-code-execution-openapi.yml
  - openapi/frostbyte-dns-lookup-openapi.yml
  - openapi/frostbyte-screenshot-openapi.yml
  - openapi/frostbyte-web-scraper-openapi.yml
  type: apiKey
slug: frostbyte-authentication
source_filename: frostbyte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/frostbyte-agent-gateway-openapi.yml, openapi/frostbyte-code-execution-openapi.yml,\n  openapi/frostbyte-crypto-prices-openapi.yml, openapi/frostbyte-dns-lookup-openapi.yml, openapi/frostbyte-ip-geolocation-openapi.yml,\n  openapi/frostbyte-screenshot-openapi.yml, openapi/frostbyte-web-scraper-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key passed in header\n  sources:\n  - openapi/frostbyte-agent-gateway-openapi.yml\n  - openapi/frostbyte-code-execution-openapi.yml\n  - openapi/frostbyte-crypto-prices-openapi.yml\n  - openapi/frostbyte-dns-lookup-openapi.yml\n  - openapi/frostbyte-ip-geolocation-openapi.yml\n  - openapi/frostbyte-screenshot-openapi.yml\n  - openapi/frostbyte-web-scraper-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description:\
  \ API key passed as query parameter\n  sources:\n  - openapi/frostbyte-agent-gateway-openapi.yml\n  - openapi/frostbyte-code-execution-openapi.yml\n  - openapi/frostbyte-dns-lookup-openapi.yml\n  - openapi/frostbyte-screenshot-openapi.yml\n  - openapi/frostbyte-web-scraper-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frostbyte/refs/heads/main/authentication/frostbyte-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Developer Tools
- Utility APIs
- Geolocation
- Cryptocurrency
- Screenshots
- DNS
- Scraping
- AI Agents
---
