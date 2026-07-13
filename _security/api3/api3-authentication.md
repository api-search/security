---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Api3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: API3 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: API3
provider_slug: api3
scheme_count: 1
schemes:
- description: Bearer token configured in the Signed API's allowedAirnodes or endpoint authTokens list. Required on endpoints or Airnode addresses configured with non-null authTokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/api3-signed-api-openapi.yml
  type: http
slug: api3-authentication
source_filename: api3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/api3-signed-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token configured in the Signed API's allowedAirnodes or endpoint authTokens\n    list. Required on endpoints or Airnode addresses configured with non-null authTokens.\n  sources:\n  - openapi/api3-signed-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api3/refs/heads/main/authentication/api3-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Oracle
- Decentralized
- Data Feeds
- Price Feeds
- Web3
- DeFi
- Smart Contracts
- OEV
- dAPI
---
