---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firmtape-com-levels-api-openapi.yml
  format: yaml
  label: firmtape-com Levels API
  slug: firmtape-com-levels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmtape-com/openapi/firmtape-com-levels-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Firmtape Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: firmtape-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: firmtape-com
provider_slug: firmtape-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Send Authorization: Bearer <key> header. Keys have scopes and prefixes as listed.'
  scheme: bearer
  scopes:
    dataset: Access DATASET files and historic levels
    geo: Access GEO API and MCP server
    lab: Access LAB API and related MCP tools
    live: Access LIVE levels API and platform integrations
    orders: Access ORDERS API and POSITIONS API
  type: http
slug: firmtape-com-authentication
source_filename: firmtape-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://firmtape.com/docs/developers/keys\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Send Authorization: Bearer <key> header. Keys have scopes and prefixes as listed.\"\n    scopes:\n      live: \"Access LIVE levels API and platform integrations\"\n      lab: \"Access LAB API and related MCP tools\"\n      dataset: \"Access DATASET files and historic levels\"\n      orders: \"Access ORDERS API and POSITIONS API\"\n      geo: \"Access GEO API and MCP server\"\n"
source_yaml_url: https://artifacts.apis.io/firmtape-com/authentication/firmtape-com-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Data
- Analytics
- Options
- Gamma
---
