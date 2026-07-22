---
api_key_in: []
api_specs:
- filename: the-token-company-openapi.yml
  format: yaml
  label: The Token Company Compression API
  slug: the-token-company-compression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-token-company/refs/heads/main/openapi/the-token-company-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: The Token Company Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Token Company secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Token Company
provider_slug: the-token-company
scheme_count: 1
schemes:
- description: All API requests authenticate with an API key issued by The Token Company, sent in the Authorization header as a bearer token. Keys carry a ttc- prefix. In the SDK wrappers the compression key is passed as compression_api_key, separate from the downstream LLM provider key.
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/the-token-company-openapi.yml
  type: http
  value_format: Bearer ttc-...
slug: the-token-company-authentication
source_filename: the-token-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/the-token-company-openapi.yml ; https://thetokencompany.com/docs/quickstart\ndocs: https://thetokencompany.com/docs/quickstart\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_prefix: \"ttc-\"\n  key_management: Dashboard at https://app.thetokencompany.com (accounts via Clerk at accounts.thetokencompany.com)\n  access_model: invite-only\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    header: Authorization\n    value_format: \"Bearer ttc-...\"\n    description: >-\n      All API requests authenticate with an API key issued by The Token Company,\n      sent in the Authorization header as a bearer token. Keys carry a ttc- prefix.\n      In the SDK wrappers the compression key is passed as compression_api_key,\n      separate from the downstream LLM provider key.\n    sources: [openapi/the-token-company-openapi.yml]\nnotes:\n  - The API is currently invite-only; keys are provisioned\
  \ after contacting the provider.\n  - No OAuth2 / OIDC surface for the compression API itself (dashboard sign-in uses Clerk).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-token-company/refs/heads/main/authentication/the-token-company-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- LLM
- Artificial Intelligence
- Prompt Compression
- Tokens
- Cost Optimization
- Developer Tools
- Middleware
- API
---
