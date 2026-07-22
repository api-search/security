---
api_key_in: []
api_specs:
- filename: total-expert-openapi.yml
  format: yaml
  label: Total Expert Public API
  slug: total-expert-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Total Expert Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Total Expert secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Total Expert
provider_slug: total-expert
scheme_count: 1
schemes:
- description: OAuth 2.0. Obtain a token from POST /v1/token using HTTP Basic (client_id:client_secret base64-encoded) plus a grant_type body. Access tokens are bearer tokens, expires_in 3600.
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://public.totalexpert.net/v1/token
  - authorizationUrl: https://public.totalexpert.net/v1/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://public.totalexpert.net/v1/token
  name: oauth2
  sources:
  - openapi/total-expert-openapi.yml
  type: oauth2
slug: total-expert-authentication
source_filename: total-expert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/total-expert-openapi.yml\ndocs: https://public.totalexpert.net/v1/docs/OAuth+Authorization+Guide.pdf\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://public.totalexpert.net/v1/token\n    scopes: 5\n  - flow: authorizationCode\n    authorizationUrl: https://public.totalexpert.net/v1/authorize\n    tokenUrl: https://public.totalexpert.net/v1/token\n    scopes: 5\n  description: >-\n    OAuth 2.0. Obtain a token from POST /v1/token using HTTP Basic\n    (client_id:client_secret base64-encoded) plus a grant_type body. Access\n    tokens are bearer tokens, expires_in 3600.\n  sources:\n  - openapi/total-expert-openapi.yml\nnotes:\n  token_request_auth: >-\n    All /v1/token requests carry an Authorization header implementing HTTP Basic:\n    base64(\"clientId:clientSecret\"\
  ), per the Vendor OAuth Integration Guide.\n  grant_types: [client_credentials, authorization_code, refresh_token]\n  access_token_ttl: 3600 seconds (1 hour); best practice is to cache the token since the token endpoint is rate limited to 2 requests per hour.\n  refresh_token_ttl: up to 2 weeks (Getting Started guide)\n  admin_vs_user: >-\n    Client-credentials tokens make calls \"As Admin\"; authorization-code (user\n    login) tokens make calls \"As User\". Many endpoints document both request\n    shapes.\n  environments: >-\n    Production tokens come from public.totalexpert.net; the isolated\n    development/sandbox domain public.vt.totalexpert.net exposes the same\n    /v1/authorize and /v1/token endpoints with separate credentials.\n  redirect_uri: Must be preregistered with Total Expert and associated with the client ID/secret.\n  developer_portal: https://developer.totalexpert.net (credentials are issued and listed under /credentials)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/authentication/total-expert-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- CRM
- Marketing Automation
- Mortgage
- Banking
- Lending
- Customer Engagement
---
