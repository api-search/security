---
api_key_in:
- header
api_specs:
- filename: openwallet-foundation-openapi.yml
  format: yaml
  label: ACA-Py Admin API
  slug: aca-py-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openwallet-foundation/refs/heads/main/openapi/openwallet-foundation-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openwallet Foundation Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenWallet Foundation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenWallet Foundation
provider_slug: openwallet-foundation
scheme_count: 1
schemes:
- description: Admin API key configured at agent startup via --admin-api-key.
  in: header
  name: AdminApiKey
  parameter: X-API-Key
  sources:
  - openapi/openwallet-foundation-openapi.yml
  type: apiKey
slug: openwallet-foundation-authentication
source_filename: openwallet-foundation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openwallet-foundation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AdminApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Admin API key configured at agent startup via --admin-api-key.\n  sources:\n  - openapi/openwallet-foundation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openwallet-foundation/refs/heads/main/authentication/openwallet-foundation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Credentials
- Digital Wallet
- Identity
- Linux Foundation
---
