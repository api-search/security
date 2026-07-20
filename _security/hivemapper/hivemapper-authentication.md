---
api_key_in:
- query
api_specs:
- filename: hivemapper-beemaps-openapi.yml
  format: yaml
  label: Bee Maps (Hivemapper) Developer API
  slug: bee-maps-hivemapper-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hivemapper/refs/heads/main/openapi/hivemapper-beemaps-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hivemapper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hivemapper secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hivemapper
provider_slug: hivemapper
scheme_count: 2
schemes:
- description: 'HTTP Basic authentication. Send Authorization: Basic <base64(username:api-key)>. The hive-py SDK expects a base64-encoded "username:api-key" string as the Basic credential.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/hivemapper-beemaps-openapi.yml
  - https://github.com/Hivemapper/hive-py
  type: http
- description: API key passed as the apiKey query parameter. Also used to authenticate the MCP endpoint (POST /api/developer/mcp).
  in: query
  name: apiKeyQuery
  param: apiKey
  sources:
  - https://docs.beemaps.com/api-reference
  type: apiKey
slug: hivemapper-authentication
source_filename: hivemapper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.beemaps.com/api-reference\ndocs: https://docs.beemaps.com/api-reference\nsummary:\n  types: [http, apiKey]\n  http_schemes: [basic]\n  api_key_in: [query]\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. Send Authorization: Basic <base64(username:api-key)>.\n      The hive-py SDK expects a base64-encoded \"username:api-key\" string as the\n      Basic credential.\n    sources: [openapi/hivemapper-beemaps-openapi.yml, https://github.com/Hivemapper/hive-py]\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    param: apiKey\n    description: >-\n      API key passed as the apiKey query parameter. Also used to authenticate the\n      MCP endpoint (POST /api/developer/mcp).\n    sources: [https://docs.beemaps.com/api-reference]\nnotes: >-\n  API keys are issued from the Bee Maps developer dashboard\n  (https://beemaps.com/developers). No\
  \ OAuth2 / OpenID Connect surface is\n  documented, so no scopes/ artifact applies.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hivemapper/refs/heads/main/authentication/hivemapper-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Logistics
- Mapping
- Geospatial
- Imagery
- Location
- Street View
- Mobility
- Machine Learning
- Web3
---
