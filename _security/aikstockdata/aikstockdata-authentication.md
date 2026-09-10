---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: 한국주식데이터 공개 데이터 API
  slug: 한국주식데이터-공개-데이터-api
  spec_type: OpenAPI
  url: https://aikstockdata.com/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Aikstockdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: 한국주식데이터 (aikstockdata) declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: 한국주식데이터 (aikstockdata)
provider_slug: aikstockdata
scheme_count: 0
schemes: []
slug: aikstockdata-authentication
source_filename: aikstockdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: 'generated: ''2026-09-10''

  method: searched

  source: https://aikstockdata.com/ai + openapi/aikstockdata-openapi.json (no securitySchemes)

  summary: No authentication. Fully public, keyless, unauthenticated REST/static-file API with CORS fully open. The OpenAPI declares no securitySchemes and no security requirement; the provider states no signup and no API key issuance.

  schemes: []

  auth_required: false

  cors: ''open (Access-Control-Allow-Origin: *)''

  notes: ''MCP server at https://mcp.aikstockdata.com/mcp is also unauthenticated (authentication: none) with no session header required.''

  '
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikstockdata/refs/heads/main/authentication/aikstockdata-authentication.yml
summary_line: 0 schemes
tags:
- korea
- stock-market
- financial-data
- open-data
- dart
- kospi
- kosdaq
- konex
- filings
- equities
- mcp
- llms-txt
- openapi
---
