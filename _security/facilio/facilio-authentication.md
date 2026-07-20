---
api_key_in:
- header
api_specs:
- filename: facilio-openapi-original.yaml
  format: yaml
  label: Facilio REST API v5
  slug: facilio-rest-api-v5
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facilio/refs/heads/main/openapi/facilio-openapi-original.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Facilio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Facilio secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Facilio
provider_slug: facilio
scheme_count: 2
schemes:
- description: Personal access token
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/facilio-openapi-original.yaml
  type: apiKey
- description: Supports authorization_code and password grant types
  flows:
  - authorizationUrl: https://us.facilioapis.com/identity/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://us.facilioapis.com/identity/oauth2/token
  - flow: password
    scopes: 0
    tokenUrl: https://us.facilioapis.com/identity/oauth2/token
  name: oauth2
  sources:
  - openapi/facilio-openapi-original.yaml
  type: oauth2
slug: facilio-authentication
source_filename: facilio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/facilio-openapi-original.yaml\ndocs: https://facilio.com/developers/docs/api-reference/\nnotes: >-\n  Two auth models. API-key requests use the 'maintenance' app on the regional\n  host (x-api-key header). OAuth2 requests use the 'developer' app. Host template\n  is https://{region}.facilioapis.com/{app_name}/api/v5 with region in\n  [us, au, ae, uk, us-azure, sa]. OAuth2 identity endpoints are region-scoped\n  (e.g. https://us.facilioapis.com/identity/oauth2/...). The hosted MCP server\n  (mcp.facilio.com) is a separate OAuth 2.0 authorization server with granular\n  scopes — see scopes/facilio-scopes.yml.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Personal access token\n  sources:\n  - openapi/facilio-openapi-original.yaml\n- name: oauth2\n\
  \  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.facilioapis.com/identity/oauth2/authorize\n    tokenUrl: https://us.facilioapis.com/identity/oauth2/token\n    scopes: 0\n  - flow: password\n    tokenUrl: https://us.facilioapis.com/identity/oauth2/token\n    scopes: 0\n  description: Supports authorization_code and password grant types\n  sources:\n  - openapi/facilio-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facilio/refs/heads/main/authentication/facilio-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Ai
- Facility Management
- CMMS
- Property Operations
- Maintenance
- Asset Management
- Real Estate
- IoT
- Buildings
---
