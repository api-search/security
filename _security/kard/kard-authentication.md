---
api_key_in: []
api_specs:
- filename: kard-api-reference-openapi.yaml
  format: yaml
  label: Kard Rewards API
  slug: kard-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-api-reference-openapi.yaml
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Kard Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Kard secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Kard
provider_slug: kard
scheme_count: 2
schemes:
- name: OAuthScheme
  notes: Bearer access token obtained via OAuth2 client_credentials at the /v2/auth/token endpoint.
  scheme: bearer
  sources:
  - openapi/kard-api-reference-openapi.yaml
  type: http
- name: bearer
  scheme: bearer
  sources:
  - openapi/kard-legacy-openapi.yaml
  type: http
slug: kard-authentication
source_filename: kard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kard-api-reference-openapi.yaml\ndocs: https://docs.getkard.com/api/integration-guides/authentication\nsummary:\n  types:\n  - oauth2\n  - http-bearer\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nflow:\n  grant_type: client_credentials\n  token_endpoint: https://{client-subdomain}.getkard.com/v2/auth/token\n  client_authentication: HTTP Basic with base64(client_id:client_secret) in the Authorization\n    header\n  request: grant_type=client_credentials in the request body\n  response: JSON with access_token used as a Bearer token on subsequent requests\n  token_lifetime_seconds: 3600\n  multi_issuer_header: X-Kard-Target-Issuer scopes the token to a specific issuer\n  deprecated: A legacy Amazon Cognito token endpoint exists but is being discontinued.\nschemes:\n- name: OAuthScheme\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kard-api-reference-openapi.yaml\n  notes: Bearer access token obtained\
  \ via OAuth2 client_credentials at the /v2/auth/token\n    endpoint.\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kard-legacy-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/authentication/kard-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- Company
- Rewards
- Card-Linked Offers
- Loyalty
- Fintech
- Commerce Media
- Advertising
- Transactions
- Cashback
- Webhooks
---
