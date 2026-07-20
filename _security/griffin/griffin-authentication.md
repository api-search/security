---
api_key_in:
- header
api_specs:
- filename: griffin-openapi-original.yml
  format: yaml
  label: The Griffin API
  slug: the-griffin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/griffin/refs/heads/main/openapi/griffin-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Griffin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Griffin secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Griffin
provider_slug: griffin
scheme_count: 1
schemes:
- description: 'API token authentication passed in the Authorization header.

    Format: `GriffinAPIKey g-test-MyKey-XXXXXXX`. Keys are created in the app

    (Settings > API keys), shown once, and scoped by the holder''s org role.'
  format: GriffinAPIKey $GRIFFIN_API_KEY
  in: header
  key_prefixes:
    test: g-test-
  name: api-key-auth
  parameter: Authorization
  sources:
  - openapi/griffin-openapi-original.yml
  type: apiKey
slug: griffin-authentication
source_filename: griffin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/griffin-openapi-original.yml\ndocs: https://docs.griffin.com/docs/guides/api-security-overview\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Griffin uses API-key authentication with an additional mandatory HTTP\n    message-signature layer in live mode. There is no OAuth2 surface; API-key\n    access is scoped by the organizational role attached to the key.\nschemes:\n- name: api-key-auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'GriffinAPIKey $GRIFFIN_API_KEY'\n  key_prefixes:\n    test: g-test-\n  description: |-\n    API token authentication passed in the Authorization header.\n    Format: `GriffinAPIKey g-test-MyKey-XXXXXXX`. Keys are created in the app\n    (Settings > API keys), shown once, and scoped by the holder's org role.\n  sources:\n  - openapi/griffin-openapi-original.yml\nmessage_signatures:\n  standard: HTTP Message Signatures (RFC 9421)\n  required_in:\
  \ live\n  optional_in: sandbox\n  enforce_toggle: 'Validate all requests (sandbox)'\n  docs: https://docs.griffin.com/docs/guides/how-to-create-message-signatures\n  verify_operations:\n  - GET /v0/security/message-signature/verify\n  - POST /v0/security/message-signature/verify\n  notes: >-\n    Clients register a public key (Settings > Message signatures) and sign each\n    request with the private key; multiple signatures per request are supported\n    for key rotation. The same signing process authenticates inbound webhook\n    event notifications. Reference utilities: github.com/griffinbank/http-message-signatures.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/griffin/refs/heads/main/authentication/griffin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Payments
- KYC
- Open Banking
- Bank Accounts
- Financial Services
---
