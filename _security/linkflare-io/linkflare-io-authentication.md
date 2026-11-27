---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Linkflare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Linkflare secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Linkflare
provider_slug: linkflare-io
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Clerk session token or personal API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/linkflare-io-openapi.json
  type: http
- description: Personal API key generated in app settings.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/linkflare-io-openapi.json
  type: apiKey
slug: linkflare-io-authentication
source_filename: linkflare-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/linkflare-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Clerk session token or personal API key.\n  sources:\n  - openapi/linkflare-io-openapi.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Personal API key generated in app settings.\n  sources:\n  - openapi/linkflare-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linkflare-io/authentication/linkflare-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Bookmark manager
- Knowledge Base
- Wishlist
- Reading
- Privacy
---
