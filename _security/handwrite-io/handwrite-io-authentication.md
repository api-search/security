---
api_key_in:
- header
api_specs:
- filename: handwrite-io-handwriting-api-openapi.yml
  format: yaml
  label: Handwrite IO Handwriting API
  slug: handwrite-io-handwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/openapi/handwrite-io-handwriting-api-openapi.yml
- filename: handwrite-io-orders-api-openapi.yml
  format: yaml
  label: Handwrite IO Orders API
  slug: handwrite-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/openapi/handwrite-io-orders-api-openapi.yml
- filename: handwrite-io-send-api-openapi.yml
  format: yaml
  label: Handwrite IO Send API
  slug: handwrite-io-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/openapi/handwrite-io-send-api-openapi.yml
- filename: handwrite-io-stationery-api-openapi.yml
  format: yaml
  label: Handwrite IO Stationery API
  slug: handwrite-io-stationery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/openapi/handwrite-io-stationery-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Handwrite Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Handwrite IO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Handwrite IO
provider_slug: handwrite-io
scheme_count: 1
schemes:
- applied_to:
  - getHandwritings
  - getStationery
  - sendLetter
  - getOrder
  bearer: false
  description: 'The raw API key is sent as the ENTIRE value of the Authorization header, with no "Bearer " or other scheme prefix — e.g. `Authorization: live_hw_...`. Content-Type must be application/json. Handwrite explicitly forbids calling the API from a browser, and issues no publishable/CORS-safe key, so every call must be server-side.'
  expiry: none published (static key)
  in: header
  key_format: <mode>_hw_<random>
  key_modes:
    live:
      billed: true
      mails: true
      prefix: live_hw
    test:
      billed: false
      mails: false
      prefix: test_hw
  name: ApiKeyAuth
  parameter: Authorization
  provisioning:
    dashboard: https://app.handwrite.io/integrations/api
    requires_account: true
    self_serve: true
    signup: https://app.handwrite.io/signup
  rotation_policy: not published
  scheme_prefix: none
  scopes: none — the key is all-or-nothing across all four operations
  sources:
  - https://documentation.handwrite.io/#getting-started
  - openapi/handwrite-io-handwriting-api-openapi.yml
  - openapi/handwrite-io-orders-api-openapi.yml
  - openapi/handwrite-io-send-api-openapi.yml
  - openapi/handwrite-io-stationery-api-openapi.yml
  type: apiKey
slug: handwrite-io-authentication
source_filename: handwrite-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://documentation.handwrite.io/#getting-started ;\n  https://raw.githubusercontent.com/handwriteio/API-Docs/master/source/includes/_intro.md ;\n  live 401 observed from https://api.handwrite.io/v1/handwriting on 2026-08-13 ; baseline\n  derived from openapi/handwrite-io-*-openapi.yml\ndocs: https://documentation.handwrite.io/#getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_prefix: none\n  bearer: false\n  description: >-\n    The raw API key is sent as the ENTIRE value of the Authorization header, with no \"Bearer \"\n    or other scheme prefix — e.g. `Authorization: live_hw_...`. Content-Type must be\n    application/json. Handwrite explicitly forbids calling the API from a browser, and issues no\n    publishable/CORS-safe key, so\
  \ every call must be server-side.\n  key_format: '<mode>_hw_<random>'\n  key_modes:\n    test:\n      prefix: test_hw\n      billed: false\n      mails: false\n    live:\n      prefix: live_hw\n      billed: true\n      mails: true\n  provisioning:\n    self_serve: true\n    requires_account: true\n    dashboard: https://app.handwrite.io/integrations/api\n    signup: https://app.handwrite.io/signup\n  rotation_policy: not published\n  expiry: none published (static key)\n  scopes: none — the key is all-or-nothing across all four operations\n  applied_to:\n    - getHandwritings\n    - getStationery\n    - sendLetter\n    - getOrder\n  sources:\n  - https://documentation.handwrite.io/#getting-started\n  - openapi/handwrite-io-handwriting-api-openapi.yml\n  - openapi/handwrite-io-orders-api-openapi.yml\n  - openapi/handwrite-io-send-api-openapi.yml\n  - openapi/handwrite-io-stationery-api-openapi.yml\nfailure_behavior:\n  status: 401\n  observed: '2026-08-13'\n  probe_url: https://api.handwrite.io/v1/handwriting\n\
  \  body: >-\n    {\"message\":\"No token provided. Please make sure to include it in your headers, e.g.\n    Authorization: test_HW_...\"}\n  note: >-\n    The API distinguishes a missing token from a wrong one in the human-readable message only;\n    both are 401 and neither carries a machine-readable error code.\noauth:\n  supported: false\n  discovery_probed:\n    - path: /.well-known/oauth-authorization-server\n      status: 404\n    - path: /.well-known/openid-configuration\n      status: 404\n  hosts_probed: api.handwrite.io, handwrite.io, www.handwrite.io, documentation.handwrite.io\nobservations:\n  - >-\n    A single static, unscoped key that can mail physical billed cards is a meaningful blast\n    radius. There is no way to issue a read-only credential for the two list operations or the\n    order lookup, so any integration that only needs to check order status still holds a key\n    that can spend money.\n  - >-\n    Test-mode isolation is the one mitigating control: a test_hw\
  \ key exercises the same\n    endpoints without billing or mailing. Grant test keys to anything that does not need to send.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handwrite-io/refs/heads/main/authentication/handwrite-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Direct Mail
- Handwritten
- Handwritten Notes
- Cards
- Marketing
- Notes
- Print
- Fulfillment
- Customer Engagement
---
