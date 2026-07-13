---
api_key_in:
- cookie
api_specs:
- filename: openapi-public.yaml
  format: yaml
  label: Hanko Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-public.yaml
- filename: openapi-admin.yaml
  format: yaml
  label: Hanko Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-admin.yaml
- filename: openapi-passkeys.yaml
  format: yaml
  label: Hanko Passkey API
  slug: passkey-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-passkeys.yaml
- filename: openapi-flow.yaml
  format: yaml
  label: Hanko Flow API
  slug: flow-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-flow.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hanko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hanko secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hanko
provider_slug: hanko
scheme_count: 2
schemes:
- bearerFormat: API Key
  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is your API key. Must only be used when using Hanko Cloud.
  name: BearerApiKeyAuth
  scheme: bearer
  sources:
  - openapi/hanko-admin-api-openapi.yml
  - openapi/hanko-flow-api-openapi.yml
  - openapi/hanko-public-api-openapi.yml
  type: http
- in: cookie
  name: CookieAuth
  parameter: hanko
  sources:
  - openapi/hanko-flow-api-openapi.yml
  - openapi/hanko-public-api-openapi.yml
  type: apiKey
slug: hanko-authentication
source_filename: hanko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hanko-admin-api-openapi.yml, openapi/hanko-flow-api-openapi.yml, openapi/hanko-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: BearerApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Bearer authentication header of the form `Bearer <token>`, where `<token>` is\n    your API key. Must only be used when using Hanko Cloud.\n  sources:\n  - openapi/hanko-admin-api-openapi.yml\n  - openapi/hanko-flow-api-openapi.yml\n  - openapi/hanko-public-api-openapi.yml\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: hanko\n  sources:\n  - openapi/hanko-flow-api-openapi.yml\n  - openapi/hanko-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanko/refs/heads/main/authentication/hanko-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Authentication
- Passkeys
- WebAuthn
- FIDO2
- Identity
- OAuth
- SAML
- Passwordless
- Open Source
---
