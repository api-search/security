---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trueproxies-openapi.yml
  format: yaml
  label: TrueProxies Customer API
  slug: trueproxies-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/openapi/trueproxies-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Trueproxies Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrueProxies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrueProxies
provider_slug: trueproxies
scheme_count: 1
schemes:
- bearerFormat: API key
  description: 'Send Authorization: Bearer tp_api_… . Create a named, scoped key in the customer dashboard. Keys expire after 30, 90 or 365 days and can be revoked immediately.'
  name: customerAPIKey
  scheme: bearer
  sources:
  - openapi/trueproxies-openapi.yml
  type: http
slug: trueproxies-authentication
source_filename: trueproxies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: derived\nsource: openapi/trueproxies-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: customerAPIKey\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Send Authorization: Bearer tp_api_… . Create a named, scoped key in the customer\n    dashboard. Keys expire after 30, 90 or 365 days and can be revoked immediately.'\n  sources:\n  - openapi/trueproxies-openapi.yml\nkey_scopes:\n  note: Permission scopes named in the operation descriptions of the provider OpenAPI; they are API-key scopes, not OAuth scopes.\n  scopes: [services:read, proxy:read, proxy:write, billing:read, billing:write, reseller:read, reseller:purchase]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/authentication/trueproxies-authentication.yml
summary_line: http · 1 scheme
tags:
- Proxies
- Residential Proxies
- Datacenter Proxies
- Web Scraping
- Networking
- IPv6
- SOCKS5
- Data Collection
---
