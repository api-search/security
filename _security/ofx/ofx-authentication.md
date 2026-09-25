---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ofx-aisp-openapi-generated.yml
  format: yaml
  label: OFX AISP API
  slug: aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-aisp-openapi-generated.yml
- filename: ofx-ncp-openapi-generated.yml
  format: yaml
  label: OFX NCP API
  slug: ncp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-ncp-openapi-generated.yml
- filename: ofx-pisp-openapi-generated.yml
  format: yaml
  label: OFX PISP API
  slug: pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-pisp-openapi-generated.yml
- filename: ofx-rates-openapi-generated.yml
  format: yaml
  label: OFX Rates API
  slug: rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-rates-openapi-generated.yml
auth_types: []
description: OAuth 2.0 authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ofx Authentication
name_suffix: Authentication
oauth_flows: []
overview: OFX declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OFX
provider_slug: ofx
scheme_count: 1
schemes:
- authorize_url: https://sandbox.api.ofx.com/v1/oauth/authorize
  evidence: OFX Payments API is protected by the industry standard OAuth2.0 protocol
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: After registering your app you will receive a client_id and client_secret.
  name: OAuth 2.0
  scopes:
  - payments
  token_url: https://sandbox.api.ofx.com/v1/oauth/token
  type: oauth2
slug: ofx-authentication
source_filename: ofx-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.ofx.com/docs/aisp-api/ZG9jOjExNjE2NDU1-authentication
source_yaml: "generated: '2026-09-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.ofx.com/docs/aisp-api/ZG9jOjExNjE2NDU1-authentication\nsources:\n- https://api-docs.ofx.com/docs/aisp-api/ZG9jOjExNjE2NDU1-authentication\n- https://api-docs.ofx.com/docs/ofx-ncp-apis/mglx0acynko37-o-auth-2-0-setup-guide\n- https://api-docs.ofx.com/docs/payments-api/c338b3f76411d-introduction\ndescription: OAuth 2.0 authentication\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OFX Payments API is protected by the industry standard OAuth2.0 protocol\n  flows:\n  - client_credentials\n  - authorization_code\n  token_url: https://sandbox.api.ofx.com/v1/oauth/token\n  authorize_url: https://sandbox.api.ofx.com/v1/oauth/authorize\n  scopes:\n  - payments\n  how_to_obtain: After registering your app you will receive a client_id and client_secret.\ndocs: https://api-docs.ofx.com/docs/aisp-api/ZG9jOjExNjE2NDU1-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/authentication/ofx-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Money Transfer
- Fintech
- Banking
---
