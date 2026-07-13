---
api_key_in:
- header
api_specs:
- filename: ncr-voyix-platform-openapi.yml
  format: yaml
  label: NCR Voyix Commerce Platform APIs (Aloha)
  slug: ncr-voyix-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aloha-pos/refs/heads/main/openapi/ncr-voyix-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aloha Pos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aloha POS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aloha POS
provider_slug: aloha-pos
scheme_count: 1
schemes:
- description: HMAC authentication. The Authorization header carries "AccessKey {sharedKey}:{signature}", where the signature is a Base64 SHA-512 HMAC computed over the HTTP method, path and query, Content-Type, nep-correlation-id, and nep-organization, keyed by the secret key concatenated with the ISO-8601 request date. See the ncr-bsp-hmac repository for reference implementations.
  in: header
  name: hmacAccessKey
  parameter: Authorization
  sources:
  - openapi/ncr-voyix-platform-openapi.yml
  type: apiKey
slug: aloha-pos-authentication
source_filename: aloha-pos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ncr-voyix-platform-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmacAccessKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC authentication. The Authorization header carries \"AccessKey {sharedKey}:{signature}\",\n    where the signature is a Base64 SHA-512 HMAC computed over the HTTP method, path and query,\n    Content-Type, nep-correlation-id, and nep-organization, keyed by the secret key concatenated\n    with the ISO-8601 request date. See the ncr-bsp-hmac repository for reference implementations.\n  sources:\n  - openapi/ncr-voyix-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aloha-pos/refs/heads/main/authentication/aloha-pos-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- POS
- Restaurant
- Hospitality
- NCR
---
