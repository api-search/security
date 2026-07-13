---
api_key_in: []
api_specs:
- filename: app-store-connect-openapi-specification.zip
  format: yaml
  label: App Store Connect API
  slug: app-store-connect-api
  spec_type: OpenAPI
  url: https://developer.apple.com/sample-code/app-store-connect/app-store-connect-openapi-specification.zip
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apple Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apple secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apple
provider_slug: apple
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: App Store Connect API uses JSON Web Tokens (JWT) for authentication. Generate a token using your API key from App Store Connect. The token must include the issuer ID, key ID, and be signed with the ES256 algorithm using your private key. Tokens expire after 20 minutes.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/app-store-connect-api.yml
  type: http
slug: apple-authentication
source_filename: apple-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/app-store-connect-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: App Store Connect API uses JSON Web Tokens (JWT) for authentication. Generate\n    a token using your API key from App Store Connect. The token must include the issuer ID,\n    key ID, and be signed with the ES256 algorithm using your private key. Tokens expire after\n    20 minutes.\n  sources:\n  - openapi/app-store-connect-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple/refs/heads/main/authentication/apple-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer
- iOS
- macOS
- Mobile
- Technology
- Fortune 100
---
