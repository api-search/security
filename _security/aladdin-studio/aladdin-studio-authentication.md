---
api_key_in: []
api_specs:
- filename: aladdin-studio-analytics-api-openapi.yml
  format: yaml
  label: Aladdin Studio Analytics API
  slug: aladdin-studio-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-analytics-api-openapi.yml
- filename: aladdin-studio-connections-api-openapi.yml
  format: yaml
  label: Aladdin Studio Connections API
  slug: aladdin-studio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-connections-api-openapi.yml
- filename: aladdin-studio-datasets-api-openapi.yml
  format: yaml
  label: Aladdin Studio Datasets API
  slug: aladdin-studio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-datasets-api-openapi.yml
- filename: aladdin-studio-orders-api-openapi.yml
  format: yaml
  label: Aladdin Studio Orders API
  slug: aladdin-studio-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-orders-api-openapi.yml
- filename: aladdin-studio-portfolios-api-openapi.yml
  format: yaml
  label: Aladdin Studio Portfolios API
  slug: aladdin-studio-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-portfolios-api-openapi.yml
- filename: aladdin-studio-positions-api-openapi.yml
  format: yaml
  label: Aladdin Studio Positions API
  slug: aladdin-studio-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-positions-api-openapi.yml
- filename: aladdin-studio-queries-api-openapi.yml
  format: yaml
  label: Aladdin Studio Queries API
  slug: aladdin-studio-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-queries-api-openapi.yml
- filename: aladdin-studio-research-api-openapi.yml
  format: yaml
  label: Aladdin Studio Research API
  slug: aladdin-studio-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-research-api-openapi.yml
- filename: aladdin-studio-risk-api-openapi.yml
  format: yaml
  label: Aladdin Studio Risk API
  slug: aladdin-studio-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-risk-api-openapi.yml
- filename: aladdin-studio-securities-api-openapi.yml
  format: yaml
  label: Aladdin Studio Securities API
  slug: aladdin-studio-securities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/openapi/aladdin-studio-securities-api-openapi.yml
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
