---
api_key_in: []
api_specs:
- filename: garner-health-openapi-original.yml
  format: yaml
  label: Garner Health API
  slug: garner-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/garner-health/refs/heads/main/openapi/garner-health-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Garner Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Garner Health secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Garner Health
provider_slug: garner-health
scheme_count: 2
schemes:
- bearerFormat: API_TOKEN
  name: ApiToken
  scheme: bearer
  sources:
  - openapi/garner-health-openapi-original.yml
  type: http
- flow: clientCredentials
  name: OAuth2ClientCredentials
  scopes: []
  source: https://garnerhealth.redoc.ly/#section/Authentication:/OAuth2.0
  tokenUrl: https://api.getgarner.com/oauth2/token
  token_lifetime_seconds: 900
  type: oauth2
slug: garner-health-authentication
source_filename: garner-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/garner-health-openapi-original.yml\ndocs: 'https://garnerhealth.redoc.ly/#section/Authentication:'\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  The published OpenAPI declares a single http bearer scheme (ApiToken, bearerFormat\n  API_TOKEN). The Garner developer docs document the primary mechanism as OAuth 2.0\n  client-credentials: exchange an API client_id + client_secret at POST\n  https://api.getgarner.com/oauth2/token (grant_type=client_credentials) for a Bearer\n  access_token valid 15 minutes, then send it as Authorization: Bearer <token>. A legacy\n  path issues a long-lived JWT at account setup used directly as the bearer token. All\n  credentials are provisioned during account setup by a Garner account manager.\nschemes:\n- name: ApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: API_TOKEN\n  sources:\n  - openapi/garner-health-openapi-original.yml\n\
  - name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.getgarner.com/oauth2/token\n  token_lifetime_seconds: 900\n  source: 'https://garnerhealth.redoc.ly/#section/Authentication:/OAuth2.0'\n  scopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garner-health/refs/heads/main/authentication/garner-health-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health Data
- Provider Directory
- Care Navigation
- Claims Analytics
- Health Plans
- Employee Benefits
---
