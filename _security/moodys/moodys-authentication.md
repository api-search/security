---
api_key_in: []
api_specs:
- filename: moodys-series-api-openapi.yml
  format: yaml
  label: Moody's Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-series-api-openapi.yml
- filename: moodys-audit-api-openapi.yml
  format: yaml
  label: Moody's Audit API
  slug: moodys-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-audit-api-openapi.yml
- filename: moodys-dataseries-api-openapi.yml
  format: yaml
  label: Moody's Data Series API
  slug: moodys-dataseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-dataseries-api-openapi.yml
- filename: moodys-forecast-api-openapi.yml
  format: yaml
  label: Moody's Forecast API
  slug: moodys-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-forecast-api-openapi.yml
- filename: moodys-healthcheck-api-openapi.yml
  format: yaml
  label: Moody's Health Check API
  slug: moodys-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-healthcheck-api-openapi.yml
- filename: moodys-interpolation-api-openapi.yml
  format: yaml
  label: Moody's Interpolation API
  slug: moodys-interpolation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-interpolation-api-openapi.yml
- filename: moodys-order-api-openapi.yml
  format: yaml
  label: Moody's Order API
  slug: moodys-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-order-api-openapi.yml
- filename: moodys-project-api-openapi.yml
  format: yaml
  label: Moody's Project API
  slug: moodys-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-project-api-openapi.yml
- filename: moodys-scenario-api-openapi.yml
  format: yaml
  label: Moody's Scenario API
  slug: moodys-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-scenario-api-openapi.yml
- filename: moodys-seriessearch-api-openapi.yml
  format: yaml
  label: Moody's Series Search API
  slug: moodys-seriessearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-seriessearch-api-openapi.yml
- filename: moodys-universe-api-openapi.yml
  format: yaml
  label: Moody's Universe API
  slug: moodys-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-universe-api-openapi.yml
- filename: moodys-vin-api-openapi.yml
  format: yaml
  label: Moody's Vin API
  slug: moodys-vin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-vin-api-openapi.yml
- filename: moodys-filetypes-api-openapi.yml
  format: yaml
  label: Moody's File Types API
  slug: moodys-filetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-filetypes-api-openapi.yml
- filename: moodys-frequency-api-openapi.yml
  format: yaml
  label: Moody's Frequency API
  slug: moodys-frequency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-frequency-api-openapi.yml
- filename: moodys-multiseries-api-openapi.yml
  format: yaml
  label: Moody's Multi Series API
  slug: moodys-multiseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-multiseries-api-openapi.yml
- filename: moodys-vintage-api-openapi.yml
  format: yaml
  label: Moody's Vintage API
  slug: moodys-vintage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-vintage-api-openapi.yml
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
