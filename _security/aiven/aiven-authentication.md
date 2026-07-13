---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Aiven REST API
  slug: aiven-api
  spec_type: OpenAPI
  url: https://api.aiven.io/doc/
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Aiven Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Aiven secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Aiven
provider_slug: aiven
scheme_count: 2
schemes:
- description: 'Header should be of the format `authorization: aivenv1 <TOKEN>`. Tokens can be obtained from [your Aiven profile page](https://console.aiven.io/profile/auth)'
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/aiven-aiven-api-openapi.yml
  type: http
- description: OAuth2 security scheme
  flows:
  - authorizationUrl: https://console.aiven.io/oauth/authorize
    flow: authorizationCode
    scopes: 34
    tokenUrl: https://api.aiven.io/v1/oauth2/token
  name: oauth2
  sources:
  - openapi/aiven-aiven-api-openapi.yml
  type: oauth2
slug: aiven-authentication
source_filename: aiven-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aiven-aiven-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  description: 'Header should be of the format `authorization: aivenv1 <TOKEN>`. Tokens can\n    be obtained from [your Aiven profile page](https://console.aiven.io/profile/auth)'\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.aiven.io/oauth/authorize\n    tokenUrl: https://api.aiven.io/v1/oauth2/token\n    scopes: 34\n  description: OAuth2 security scheme\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiven/refs/heads/main/authentication/aiven-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Managed Data Infrastructure
- Apache Kafka
- PostgreSQL
- OpenSearch
- ClickHouse
- Redis
- MySQL
- Open Source
- Cloud Database
- DBaaS
- Data Streaming
- Data Platform
---
