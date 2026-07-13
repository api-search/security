---
api_key_in: []
api_specs:
- filename: civic-pass-customer-api.yaml
  format: yaml
  label: Civic Pass API
  slug: civic-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/openapi/civic-pass-customer-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Civic Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Civic secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Civic
provider_slug: civic
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth0.civic.com/oauth/token
  name: pass_auth
  sources:
  - openapi/civic-pass-customer-api.yaml
  type: oauth2
slug: civic-authentication
source_filename: civic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/civic-pass-customer-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: pass_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth0.civic.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/civic-pass-customer-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/authentication/civic-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI Agents
- Authentication
- Digital Identity
- Identity Verification
- KYC
- MCP
- OAuth
- Security
- Solana
- Web3
- Wallets
---
