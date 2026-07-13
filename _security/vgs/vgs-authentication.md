---
api_key_in: []
api_specs:
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Vault Tokenization API
  slug: vgs-vault-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Accounts Management API
  slug: vgs-accounts-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Routes & Proxy API
  slug: vgs-routes-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Functions API
  slug: vgs-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Organizations API
  slug: vgs-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vgs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Very Good Security secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Very Good Security
provider_slug: vgs
scheme_count: 2
schemes:
- description: HTTP Basic authentication used by the VGS Vault HTTP API. Username and password are the vault access credentials generated in the VGS dashboard.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vgs-openapi.yml
  type: http
- bearerFormat: JWT
  description: 'Bearer access token used by the VGS Accounts API. Obtain the token from the OAuth2 client-credentials endpoint at https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token using a service-account client id and secret, then pass it as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vgs-openapi.yml
  type: http
slug: vgs-authentication
source_filename: vgs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vgs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication used by the VGS Vault HTTP API. Username and password\n    are the vault access credentials generated in the VGS dashboard.\n  sources:\n  - openapi/vgs-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Bearer access token used by the VGS Accounts API. Obtain the token from the\n    OAuth2 client-credentials endpoint at https://auth.verygoodsecurity.com/auth/realms/vgs/protocol/openid-connect/token\n    using a service-account client id and secret, then pass it as Authorization: Bearer <token>.'\n  sources:\n  - openapi/vgs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/authentication/vgs-authentication.yml
summary_line: http · 2 schemes
tags:
- Security
- Tokenization
- Data Privacy
- PCI Compliance
- Vault
---
