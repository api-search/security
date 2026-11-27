---
anonymous_access: false
api_key_in: []
api_specs:
- filename: liqaa-io-conversations-api-openapi.yml
  format: yaml
  label: LIQAA Conversations API
  slug: liqaa-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqaa-io/openapi/liqaa-io-conversations-api-openapi.yml
- filename: liqaa-io-tokens-api-openapi.yml
  format: yaml
  label: LIQAA Tokens API
  slug: liqaa-io-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqaa-io/openapi/liqaa-io-tokens-api-openapi.yml
- filename: liqaa-io-webhooks-api-openapi.yml
  format: yaml
  label: LIQAA Webhooks API
  slug: liqaa-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/liqaa-io/openapi/liqaa-io-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LIQAA Authentication
name_suffix: Authentication
oauth_flows: []
overview: LIQAA secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LIQAA
provider_slug: liqaa-io
scheme_count: 1
schemes:
- bearerFormat: sk_live_…
  description: 'Pass your `sk_live_…` secret key as a bearer token.

    The browser must never see this value.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/liqaa-io-openapi.yaml
  type: http
slug: liqaa-io-authentication
source_filename: liqaa-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/liqaa-io-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_live_…\n  description: |-\n    Pass your `sk_live_…` secret key as a bearer token.\n    The browser must never see this value.\n  sources:\n  - openapi/liqaa-io-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/liqaa-io/authentication/liqaa-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Messaging
- SDK
- Real-Time
- Algeria
- Company
---
