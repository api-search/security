---
api_key_in: []
api_specs:
- filename: crayon-agreements-api-openapi.yml
  format: yaml
  label: Crayon Agreements API
  slug: crayon-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-agreements-api-openapi.yml
- filename: crayon-authentication-api-openapi.yml
  format: yaml
  label: Crayon Authentication API
  slug: crayon-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-authentication-api-openapi.yml
- filename: crayon-billing-api-openapi.yml
  format: yaml
  label: Crayon Billing API
  slug: crayon-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-billing-api-openapi.yml
- filename: crayon-clients-api-openapi.yml
  format: yaml
  label: Crayon Clients API
  slug: crayon-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-clients-api-openapi.yml
- filename: crayon-customertenants-api-openapi.yml
  format: yaml
  label: Crayon CustomerTenants API
  slug: crayon-customertenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-customertenants-api-openapi.yml
- filename: crayon-organizations-api-openapi.yml
  format: yaml
  label: Crayon Organizations API
  slug: crayon-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-organizations-api-openapi.yml
- filename: crayon-subscriptions-api-openapi.yml
  format: yaml
  label: Crayon Subscriptions API
  slug: crayon-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-subscriptions-api-openapi.yml
- filename: crayon-users-api-openapi.yml
  format: yaml
  label: Crayon Users API
  slug: crayon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/openapi/crayon-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Crayon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Crayon secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Crayon
provider_slug: crayon
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.crayon.com/api/v1/connect/token
  name: OAuth2
  sources:
  - openapi/crayon-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/crayon-openapi.yml
  type: http
slug: crayon-authentication
source_filename: crayon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crayon-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.crayon.com/api/v1/connect/token\n    scopes: 0\n  sources:\n  - openapi/crayon-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/crayon-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/authentication/crayon-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- AI
- MCP
---
