---
api_key_in: []
api_specs:
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Users & KYC API
  slug: pomelo-users-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Cards API
  slug: pomelo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Card Accounts API
  slug: pomelo-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Transactions API
  slug: pomelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Authorizations API
  slug: pomelo-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Transfers API
  slug: pomelo-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
- filename: pomelo-openapi.yml
  format: yaml
  label: Pomelo Webhooks API
  slug: pomelo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pomelo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pomelo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pomelo
provider_slug: pomelo
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 client-credentials access token issued by /oauth/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pomelo-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  sources:
  - openapi/pomelo-openapi.yml
  type: oauth2
slug: pomelo-authentication
source_filename: pomelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pomelo-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 client-credentials access token issued by /oauth/token.\n  sources:\n  - openapi/pomelo-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\n    scopes: 0\n  sources:\n  - openapi/pomelo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/authentication/pomelo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fintech
- Card Issuing
- Embedded Finance
- Payments
- Latin America
---
