---
api_key_in:
- header
api_specs:
- filename: bitpowr-technologies-inc-openapi.yml
  format: yaml
  label: Bitpowr Developer API
  slug: bitpowr-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpowr-technologies-inc/refs/heads/main/openapi/bitpowr-technologies-inc-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bitpowr Technologies Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: BitPowr Technologies, Inc. secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BitPowr Technologies, Inc.
provider_slug: bitpowr-technologies-inc
scheme_count: 2
schemes:
- description: 'Bearer token formed by base64-encoding the concatenation `{public_key}:{secret_key}` and sending it as `Authorization: Bearer <token>`. This grants admin access to all accounts. (The older raw encoded-token form is documented as deprecated.)'
  docs: https://docs.bitpowr.com/docs/authentication
  name: bearer
  scheme: bearer
  sources:
  - openapi/bitpowr-technologies-inc-openapi.yml
  type: http
- description: 'Dashboard-created API key with configurable restrictions, sent as `Authorization: Basic <API_KEY>`. Preferred over full public/secret access for scoped/least-privilege usage.'
  docs: https://docs.bitpowr.com/docs/get-your-api-key
  in: header
  name: apiKey
  parameter_name: Authorization
  scheme: Basic
  type: apiKey
slug: bitpowr-technologies-inc-authentication
source_filename: bitpowr-technologies-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bitpowr-technologies-inc-openapi.yml\ndocs: https://docs.bitpowr.com/docs/authentication\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  notes: >-\n    Every request requires an Authorization header over HTTPS; unauthenticated\n    requests are rejected. Bitpowr documents two credential styles. Keys are\n    environment-scoped: test keys carry a `test_` prefix.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token formed by base64-encoding the concatenation\n    `{public_key}:{secret_key}` and sending it as `Authorization: Bearer <token>`.\n    This grants admin access to all accounts. (The older raw encoded-token form is\n    documented as deprecated.)\n  sources:\n  - openapi/bitpowr-technologies-inc-openapi.yml\n  docs: https://docs.bitpowr.com/docs/authentication\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n\
  \  scheme: Basic\n  description: >-\n    Dashboard-created API key with configurable restrictions, sent as\n    `Authorization: Basic <API_KEY>`. Preferred over full public/secret access for\n    scoped/least-privilege usage.\n  docs: https://docs.bitpowr.com/docs/get-your-api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpowr-technologies-inc/refs/heads/main/authentication/bitpowr-technologies-inc-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Cryptocurrency
- Blockchain
- Digital Assets
- Wallet Infrastructure
- Wallet as a Service
- Custody
- Treasury Management
- Tokenization
- Compliance
- Web3
- Payments
---
