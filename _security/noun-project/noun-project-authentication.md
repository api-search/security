---
api_key_in:
- header
api_specs:
- filename: noun-project-openapi.yml
  format: yaml
  label: Noun Project API V2
  slug: noun-project-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Noun Project Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noun Project secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Noun Project
provider_slug: noun-project
scheme_count: 1
schemes:
- description: OAuth 1.0a signed Authorization header constructed with the client key and secret obtained from the Noun Project developer portal. A nonce of at least 8 characters is required. Use any standards-compliant OAuth 1.0a library (requests_oauthlib, Faraday-OAuth, DotNetOpenAuth, etc.).
  in: header
  name: oauth1
  parameter: Authorization
  sources:
  - openapi/noun-project-openapi.yml
  type: apiKey
slug: noun-project-authentication
source_filename: noun-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/noun-project-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: oauth1\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: OAuth 1.0a signed Authorization header constructed with the client key and secret\n    obtained from the Noun Project developer portal. A nonce of at least 8 characters is required.\n    Use any standards-compliant OAuth 1.0a library (requests_oauthlib, Faraday-OAuth, DotNetOpenAuth,\n    etc.).\n  sources:\n  - openapi/noun-project-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/authentication/noun-project-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Art And Design
- Icons
- SVG
- Visual Language
- Design Assets
- Public APIs
---
