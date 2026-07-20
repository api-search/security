---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Human Interest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Human Interest secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Human Interest
provider_slug: human-interest
scheme_count: 2
schemes:
- description: Partner API credentials exchanged for an access token; token presented as a bearer token to https://api.humaninterest.com/v1/graphql.
  name: apiCredentials
  source: https://docs.humaninterest.com/docs/getting-started/authentication
  transport: bearer
  type: oauth2
- description: OpenID Connect single sign-on so a partner platform's users can sign in to Human Interest with their identity from the partner platform.
  name: sso
  source: https://docs.humaninterest.com/docs/sso/login
  type: openIdConnect
slug: human-interest-authentication
source_filename: human-interest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.humaninterest.com/docs/getting-started/authentication\ndocs: https://docs.humaninterest.com/docs/getting-started/authentication\napi: https://api.humaninterest.com/v1/graphql\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  transport: bearer-token\n  notes: >-\n    Human Interest's GraphQL API is authenticated with partner-issued API\n    credentials that are exchanged for an access token, sent as a bearer token\n    on requests to the GraphQL endpoint. Separately, partner platforms can let\n    their users sign in to Human Interest via OpenID Connect (SSO). Exact token\n    URLs, grant type, and scope names are documented behind the client-rendered\n    docs and were not machine-readable at capture time.\nschemes:\n- name: apiCredentials\n  type: oauth2\n  transport: bearer\n  description: >-\n    Partner API credentials exchanged for an access token; token presented as a\n    bearer token to https://api.humaninterest.com/v1/graphql.\n\
  \  source: https://docs.humaninterest.com/docs/getting-started/authentication\n- name: sso\n  type: openIdConnect\n  description: >-\n    OpenID Connect single sign-on so a partner platform's users can sign in to\n    Human Interest with their identity from the partner platform.\n  source: https://docs.humaninterest.com/docs/sso/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/human-interest/refs/heads/main/authentication/human-interest-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Fintech
- Retirement
- 401(k)
- Employee Benefits
- Payroll
- GraphQL
- API
---
