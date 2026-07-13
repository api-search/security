---
api_key_in: []
api_specs:
- filename: aladdin-studio-graph-openapi.yaml
  format: yaml
  label: Aladdin Graph API
  slug: graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-graph-openapi.yaml
- filename: aladdin-studio-data-cloud-openapi.yaml
  format: yaml
  label: Aladdin Data Cloud API
  slug: data-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-data-cloud-openapi.yaml
- filename: aladdin-studio-trading-openapi.yaml
  format: yaml
  label: Aladdin Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-trading-openapi.yaml
- filename: aladdin-studio-investment-research-openapi.yaml
  format: yaml
  label: Aladdin Investment Research API
  slug: investment-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-investment-research-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aladdin Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Aladdin Studio secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Aladdin Studio
provider_slug: aladdin-studio
scheme_count: 4
schemes:
- description: OAuth 2.0 with access tokens for Data Cloud authentication
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.blackrock.com/oauth/token
  name: OAuth2
  sources:
  - openapi/aladdin-studio-data-cloud-openapi.yaml
  - openapi/aladdin-studio-investment-research-openapi.yaml
  - openapi/aladdin-studio-trading-openapi.yaml
  type: oauth2
- bearerFormat: JWT
  description: Snowflake JWT authentication using RSA key pairs for Data Cloud
  name: SnowflakeJWT
  scheme: bearer
  sources:
  - openapi/aladdin-studio-data-cloud-openapi.yaml
  type: http
- description: OAuth 2.0 authentication supporting client_credentials and refresh_token flows
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://api.blackrock.com/oauth/token
  - authorizationUrl: https://api.blackrock.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.blackrock.com/oauth/token
  name: OAuth2
  sources:
  - openapi/aladdin-studio-graph-openapi.yaml
  type: oauth2
- description: Basic authentication using API token and user credentials
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/aladdin-studio-graph-openapi.yaml
  type: http
slug: aladdin-studio-authentication
source_filename: aladdin-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aladdin-studio-data-cloud-openapi.yaml, openapi/aladdin-studio-graph-openapi.yaml,\n  openapi/aladdin-studio-investment-research-openapi.yaml, openapi/aladdin-studio-trading-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blackrock.com/oauth/token\n    scopes: 1\n  description: OAuth 2.0 with access tokens for Data Cloud authentication\n  sources:\n  - openapi/aladdin-studio-data-cloud-openapi.yaml\n  - openapi/aladdin-studio-investment-research-openapi.yaml\n  - openapi/aladdin-studio-trading-openapi.yaml\n- name: SnowflakeJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Snowflake JWT authentication using RSA key pairs for Data Cloud\n  sources:\n  - openapi/aladdin-studio-data-cloud-openapi.yaml\n- name: OAuth2\n  type:\
  \ oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blackrock.com/oauth/token\n    scopes: 4\n  - flow: authorizationCode\n    authorizationUrl: https://api.blackrock.com/oauth/authorize\n    tokenUrl: https://api.blackrock.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 authentication supporting client_credentials and refresh_token flows\n  sources:\n  - openapi/aladdin-studio-graph-openapi.yaml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using API token and user credentials\n  sources:\n  - openapi/aladdin-studio-graph-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/authentication/aladdin-studio-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
---
