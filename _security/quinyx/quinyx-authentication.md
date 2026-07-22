---
api_key_in:
- header
api_specs:
- filename: quinyx-api-v3-openapi.yml
  format: yaml
  label: Quinyx API v3
  slug: quinyx-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-api-v3-openapi.yml
- filename: quinyx-api-v2-openapi.yml
  format: yaml
  label: Quinyx API v2
  slug: quinyx-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-api-v2-openapi.yml
- filename: quinyx-userapi-v2-openapi.yml
  format: yaml
  label: Quinyx User API v2
  slug: quinyx-user-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-userapi-v2-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Quinyx Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Quinyx secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Quinyx
provider_slug: quinyx
scheme_count: 2
schemes:
- description: OAuth2 Client Credentials flow. See https://developer.quinyx.com/api/authentication
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: /oauth/v3/token
  name: employee_OAuth2ClientCredentials
  sources:
  - openapi/quinyx-api-v2-openapi.yml
  - openapi/quinyx-api-v3-openapi.yml
  type: oauth2
- in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/quinyx-userapi-v2-openapi.yml
  type: apiKey
slug: quinyx-authentication
source_filename: quinyx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/quinyx-api-v2-openapi.yml, openapi/quinyx-api-v3-openapi.yml, openapi/quinyx-userapi-v2-openapi.yml\ndocs: https://developer.quinyx.com/api/v3/authentication\nnotes: >-\n  Quinyx API v2/v3 use OAuth 2.0 client-credentials. Obtain Client ID + Client\n  Secret from Account Settings > Integration credentials, then POST\n  grant_type=client_credentials with the requested scopes to the regional token\n  endpoint (https://api.eu.quinyx.com/oauth/v3/token or api.na...). Tokens are\n  bearer, expire after ~3600s. The legacy User API (v2) uses a bearer token\n  passed in the Authorization header.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: employee_OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/v3/token\n    scopes: 4\n  description: OAuth2 Client Credentials flow. See https://developer.quinyx.com/api/authentication\n\
  \  sources:\n  - openapi/quinyx-api-v2-openapi.yml\n  - openapi/quinyx-api-v3-openapi.yml\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/quinyx-userapi-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/authentication/quinyx-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Workforce Management
- Scheduling
- Human Resources
- Time Tracking
- Forecasting
- Employee Engagement
- Retail
- Hospitality
- Company
---
