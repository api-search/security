---
api_key_in: []
api_specs:
- filename: linear-graphql-openapi.yml
  format: yaml
  label: Linear GraphQL API
  slug: linear-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/openapi/linear-graphql-openapi.yml
- filename: linear-webhooks-asyncapi.yml
  format: yaml
  label: Linear Webhooks API
  slug: linear-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/asyncapi/linear-webhooks-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Linear Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: linear secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: linear
provider_slug: linear
scheme_count: 2
schemes:
- description: Personal API key obtained from Linear settings
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/linear-graphql-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow
  flows:
  - authorizationUrl: https://linear.app/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.linear.app/oauth/token
  name: OAuth2
  sources:
  - openapi/linear-graphql-openapi.yml
  type: oauth2
slug: linear-authentication
source_filename: linear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linear-graphql-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal API key obtained from Linear settings\n  sources:\n  - openapi/linear-graphql-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://linear.app/oauth/authorize\n    tokenUrl: https://api.linear.app/oauth/token\n    scopes: 4\n  description: OAuth 2.0 authorization code flow\n  sources:\n  - openapi/linear-graphql-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linear/refs/heads/main/authentication/linear-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---
