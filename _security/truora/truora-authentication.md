---
api_key_in: []
api_specs:
- filename: truora-openapi.yml
  format: yaml
  label: Truora Checks API
  slug: truora-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Validators API
  slug: truora-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Digital Identity API
  slug: truora-digital-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Account API
  slug: truora-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Truora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truora secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truora
provider_slug: truora
scheme_count: 1
schemes:
- format: JWT
  headerName: Truora-API-Key
  in: header
  name: TruoraApiKey
  notes: Every request across all four hosts (api.checks, api.validations, api.identity, api.account) authenticates with a Truora-API-Key request header. The value is a JWT issued from the Truora dashboard or the POST /v1/api-keys endpoint. Backend keys (key_type=backend) authenticate server-to-server calls; web keys (key_type=web) are short-lived tokens that launch browser / WhatsApp Digital Identity flows. The JWT is shown only once at creation and must be stored securely.
  sources:
  - https://dev.truora.com/validators/authentication/
  - https://dev.truora.com/guides/web_integration_token/
  - openapi/truora-openapi.yml
  type: apiKey
slug: truora-authentication
source_filename: truora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/truora-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: TruoraApiKey\n  type: apiKey\n  in: header\n  headerName: Truora-API-Key\n  format: JWT\n  notes: >-\n    Every request across all four hosts (api.checks, api.validations,\n    api.identity, api.account) authenticates with a Truora-API-Key request\n    header. The value is a JWT issued from the Truora dashboard or the\n    POST /v1/api-keys endpoint. Backend keys (key_type=backend) authenticate\n    server-to-server calls; web keys (key_type=web) are short-lived tokens\n    that launch browser / WhatsApp Digital Identity flows. The JWT is shown\n    only once at creation and must be stored securely.\n  sources:\n  - https://dev.truora.com/validators/authentication/\n  - https://dev.truora.com/guides/web_integration_token/\n  - openapi/truora-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/authentication/truora-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity Verification
- KYC
- Background Checks
- Fraud Prevention
- LatAm
- WhatsApp
---
