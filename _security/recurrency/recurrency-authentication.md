---
api_key_in: []
api_specs:
- filename: recurrency-openapi.yml
  format: yaml
  label: Recurrency API
  slug: recurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recurrency/refs/heads/main/openapi/recurrency-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Recurrency Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Recurrency secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Recurrency
provider_slug: recurrency
scheme_count: 1
schemes:
- description: 'OAuth 2.0 client-credentials. POST to the token endpoint with grant_type=client_credentials plus client_id/client_secret to receive a Bearer access token (scope recurrency:api:tenant), valid for 7 days (604800 seconds). Send it as `authorization: Bearer {token}`.'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.recurrency.com/oauth/token
  name: oauth2
  sources:
  - openapi/recurrency-openapi.yml
  type: oauth2
slug: recurrency-authentication
source_filename: recurrency-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/recurrency-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.recurrency.com/oauth/token\n    scopes: 1\n  description: 'OAuth 2.0 client-credentials. POST to the token endpoint with grant_type=client_credentials\n    plus client_id/client_secret to receive a Bearer access token (scope recurrency:api:tenant),\n    valid for 7 days (604800 seconds). Send it as `authorization: Bearer {token}`.'\n  sources:\n  - openapi/recurrency-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recurrency/refs/heads/main/authentication/recurrency-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai Ml
- ERP
- Distribution
- Wholesale
- E-Procurement
- Supply Chain
- Orders
---
