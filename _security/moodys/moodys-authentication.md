---
api_key_in: []
api_specs:
- filename: moodys-series-api-openapi.yml
  format: yaml
  label: Moody's Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-series-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Moodys Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Moody's secures its APIs with oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Moody's
provider_slug: moodys
scheme_count: 4
schemes:
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  sources:
  - openapi/moodys-data-buffet-api-openapi.yml
  type: oauth2
- description: OAuth2 Client Credentials (Scenario Studio API).
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  sources:
  - openapi/moodys-scenario-studio-api-swagger.json
  type: oauth2
- description: OAuth2 Client Credentials (AutoCycle API).
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token
  name: oauth2
  sources:
  - openapi/moodys-autocycle-api-swagger.json
  type: oauth2
- description: OAuth2 Client Credentials (Muni Loss Forecast API).
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.economy.com/muni/v1/oauth2/token
  name: oauth2
  sources:
  - openapi/moodys-municipal-api-swagger.json
  type: oauth2
slug: moodys-authentication
source_filename: moodys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: derived\nsource: >-\n  openapi/moodys-data-buffet-api-openapi.yml plus the Swagger 2.0 definitions\n  harvested live from api.economy.com this round\n  (openapi/moodys-scenario-studio-api-swagger.json,\n  openapi/moodys-autocycle-api-swagger.json,\n  openapi/moodys-municipal-api-swagger.json)\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n    scopes: 0\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n  sources:\n  - openapi/moodys-data-buffet-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n    scopes: 0\n  description: OAuth2 Client Credentials (Scenario Studio\
  \ API).\n  sources:\n  - openapi/moodys-scenario-studio-api-swagger.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token\n    scopes: 0\n  description: OAuth2 Client Credentials (AutoCycle API).\n  sources:\n  - openapi/moodys-autocycle-api-swagger.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/muni/v1/oauth2/token\n    scopes: 0\n  description: OAuth2 Client Credentials (Muni Loss Forecast API).\n  sources:\n  - openapi/moodys-municipal-api-swagger.json\nnotes: >-\n  Every Moody's Analytics economy.com product API exposes its own OAuth2\n  client-credentials token endpoint under its base path; tokens are sent as\n  Bearer tokens. No scopes are defined in any flow — entitlements are\n  account-based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/authentication/moodys-authentication.yml
summary_line: oauth2 · 4 schemes
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
---
