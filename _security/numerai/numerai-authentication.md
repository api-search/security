---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Numerai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numerai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Numerai
provider_slug: numerai
scheme_count: 1
schemes:
- description: Public API id + secret key pair created per model/account with a selectable scope set.
  in: header
  key_headers:
  - x-public-id
  - x-secret-key
  name: ApiToken
  scopes_ref: scopes/numerai-scopes.yml
  sources:
  - https://api-tournament.numer.ai
  type: apiKey
slug: numerai-authentication
source_filename: numerai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api-tournament.numer.ai (live introspection) + https://docs.numer.ai\ndocs: https://docs.numer.ai/numerai-tournament/automation\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  model: >-\n    Numerai issues API token pairs (a public id + a secret key) scoped per token. Tokens are created\n    in Account > Settings and passed to the single GraphQL endpoint as request headers. Interactive\n    web sessions use password/MFA login and Privy/SSO, but programmatic access is exclusively the\n    public-id/secret-key token pair.\nschemes:\n  - name: ApiToken\n    type: apiKey\n    in: header\n    key_headers:\n      - x-public-id\n      - x-secret-key\n    description: Public API id + secret key pair created per model/account with a selectable scope set.\n    scopes_ref: scopes/numerai-scopes.yml\n    sources:\n      - https://api-tournament.numer.ai\nendpoint:\n  graphql: https://api-tournament.numer.ai\n\
  \  method: POST\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numerai/refs/heads/main/authentication/numerai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Machine Learning
- Data Science
- Hedge Fund
- GraphQL
- Crypto
- Quantitative Finance
- Tournament
- API
---
