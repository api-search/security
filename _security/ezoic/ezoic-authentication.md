---
api_key_in:
- query
- header
api_specs:
- filename: ezoic-subscriptions-openapi.yml
  format: yaml
  label: Ezoic Subscriptions Server-to-Server REST API
  slug: ezoic-subscriptions-server-to-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-subscriptions-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ezoic Authentication
name_suffix: Authentication
oauth_flows: []
overview: ezoic secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ezoic
provider_slug: ezoic
scheme_count: 3
schemes:
- description: Your Ezoic API (developer) key, passed as a query parameter alongside the account-owned domain.
  in: query
  name: developerKey
  parameter: developerKey
  sources:
  - openapi/ezoic-subscriptions-openapi.yml
  type: apiKey
- description: Reader identity — the reader's email address. Exactly one reader identity header (email OR token) must be supplied; reader identity must never be in the query string.
  in: header
  name: X-Ezoic-Reader-Email
  parameter: X-Ezoic-Reader-Email
  sources:
  - https://docs.ezoic.com/docs/subscriptions/rest-api/
  type: apiKey
- description: Reader identity — the reader's Ezoic Subscriptions session JWT (visitor-account sites). Alternative to the email header; supply exactly one.
  in: header
  name: X-Ezoic-Reader-Token
  parameter: X-Ezoic-Reader-Token
  sources:
  - https://docs.ezoic.com/docs/subscriptions/rest-api/
  type: apiKey
slug: ezoic-authentication
source_filename: ezoic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.ezoic.com/docs/subscriptions/rest-api/\ndocs: https://docs.ezoic.com/docs/subscriptions/rest-api/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\nschemes:\n- name: developerKey\n  type: apiKey\n  in: query\n  parameter: developerKey\n  description: Your Ezoic API (developer) key, passed as a query parameter alongside the account-owned domain.\n  sources:\n  - openapi/ezoic-subscriptions-openapi.yml\n- name: X-Ezoic-Reader-Email\n  type: apiKey\n  in: header\n  parameter: X-Ezoic-Reader-Email\n  description: >-\n    Reader identity — the reader's email address. Exactly one reader identity header\n    (email OR token) must be supplied; reader identity must never be in the query string.\n  sources:\n  - https://docs.ezoic.com/docs/subscriptions/rest-api/\n- name: X-Ezoic-Reader-Token\n  type: apiKey\n  in: header\n  parameter: X-Ezoic-Reader-Token\n  description: >-\n    Reader identity — the\
  \ reader's Ezoic Subscriptions session JWT (visitor-account sites).\n    Alternative to the email header; supply exactly one.\n  sources:\n  - https://docs.ezoic.com/docs/subscriptions/rest-api/\noauth:\n  note: >-\n    The Ezoic Analytics MCP server (analytics-mcp.ezoic.com/mcp) authenticates separately\n    via OAuth 2.0 with a scoped access token — see mcp/ezoic-mcp.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/authentication/ezoic-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Advertising
- AdTech
- Publisher Monetization
- Analytics
- Subscriptions
- Identity
- MCP
---
