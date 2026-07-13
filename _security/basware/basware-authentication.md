---
api_key_in: []
api_specs:
- filename: api-reference
  format: yaml
  label: Basware P2P API
  slug: basware-p2p-api
  spec_type: OpenAPI
  url: https://developer.basware.com/en/api/basware/api-reference
- filename: api-reference
  format: yaml
  label: Basware Network API
  slug: basware-network-api
  spec_type: OpenAPI
  url: https://developer.basware.com/en/api/network/api-reference
- filename: basware-vault-openapi.yaml
  format: yaml
  label: Basware Vault API
  slug: basware-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basware/refs/heads/main/openapi/basware-vault-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Basware Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Basware secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Basware
provider_slug: basware
scheme_count: 3
schemes:
- name: HTTPBasic
  scheme: basic
  sources:
  - openapi/basware-authentication-openapi.json
  - openapi/basware-directory-openapi.json
  - openapi/basware-p2p-openapi.json
  - openapi/basware-user-permission-openapi.json
  - openapi/basware-vault-openapi.yaml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/basware-directory-openapi.json
  type: http
- description: Oauth2 client credentials flow.
  flows:
  - flow: clientCredentials
    scopes: 80
    tokenUrl: https://api.basware.com/v1/tokens
  name: oauth2authentication
  sources:
  - openapi/basware-p2p-openapi.json
  - openapi/basware-user-permission-openapi.json
  type: oauth2
slug: basware-authentication
source_filename: basware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basware-authentication-openapi.json, openapi/basware-directory-openapi.json,\n  openapi/basware-p2p-openapi.json, openapi/basware-user-permission-openapi.json, openapi/basware-vault-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: HTTPBasic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/basware-authentication-openapi.json\n  - openapi/basware-directory-openapi.json\n  - openapi/basware-p2p-openapi.json\n  - openapi/basware-user-permission-openapi.json\n  - openapi/basware-vault-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/basware-directory-openapi.json\n- name: oauth2authentication\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.basware.com/v1/tokens\n    scopes: 80\n  description: Oauth2 client credentials flow.\n  sources:\n  - openapi/basware-p2p-openapi.json\n\
  \  - openapi/basware-user-permission-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basware/refs/heads/main/authentication/basware-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- E-Invoicing
- Purchase-to-Pay
- Accounts Payable
- Procurement
- Electronic Invoicing
- Finance Automation
- B2B Payments
---
