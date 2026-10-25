---
anonymous_access: false
api_key_in: []
api_specs:
- filename: carta-openapi-generated.yml
  format: yaml
  label: Carta API
  slug: carta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carta/refs/heads/main/openapi/_ae-authored/carta-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Carta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carta declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Carta
provider_slug: carta
scheme_count: 2
schemes:
- authorization_code_ttl: valid for 60 seconds
  description: Carta's API uses the OAuth 2.0 open specification ... supports AUTHORIZATION_CODE and CLIENT_CREDENTIALS grant types.
  flows:
  - authorizationCode
  - clientCredentials
  token_lifetime: An access token is valid for one hour
  type: oauth2
- docs: https://docs.carta.com/api-platform/guides/references/using-openid-connect
  note: Playground supports API access using OAuth 2.0 and OpenID Connect.
  type: openIdConnect
slug: carta-authentication
source_filename: carta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Carta authentication\ngenerated: '2026-10-20'\nmethod: searched\nsource: https://docs.carta.com/api-platform/guides/guides/authorization\ndocs: https://docs.carta.com/api-platform/guides/guides/authorization\nschemes:\n- type: oauth2\n  flows:\n  - authorizationCode\n  - clientCredentials\n  description: Carta's API uses the OAuth 2.0 open specification ... supports AUTHORIZATION_CODE and CLIENT_CREDENTIALS grant\n    types.\n  token_lifetime: An access token is valid for one hour\n  authorization_code_ttl: valid for 60 seconds\n- type: openIdConnect\n  docs: https://docs.carta.com/api-platform/guides/references/using-openid-connect\n  note: Playground supports API access using OAuth 2.0 and OpenID Connect.\nscope_example: read_investor_firms\nnote: Production OAuth apps are immutable once deployed; new scopes go through the playground-to-production flow (https://docs.carta.com/api-platform/guides/guides/adding-new-oauth-scopes).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carta/refs/heads/main/authentication/carta-authentication.yml
summary_line: 2 schemes
tags:
- Equity Management
- Cap Table
- 409A Valuations
- Fund Administration
- Employee Equity
- Investor Portfolio
- Private Markets
- Fintech
- Startups
---
