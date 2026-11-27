---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aaly-io-openapi-generated.yml
  format: yaml
  label: Aaly API
  slug: aaly-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aaly-io/openapi/_ae-authored/aaly-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aaly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aaly declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Aaly
provider_slug: aaly-io
scheme_count: 3
schemes:
- description: aaly_<id>_<secret> for CI and server-to-server calls
  header: Authorization
  in: header
  name: API Key
  type: apiKey
- bearerFormat: JWT
  description: JWT returned by signup/signin, valid 1 hour
  scheme: bearer
  type: http
- authorizationUrl: https://aaly.io/docs/auth#google-sign-in
  description: Google OAuth sign-in
  flow: authorizationCode
  scopes: {}
  type: oauth2
slug: aaly-io-authentication
source_filename: aaly-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://aaly.io/docs/auth\nschemes:\n  - type: apiKey\n    name: API Key\n    description: \"aaly_<id>_<secret> for CI and server-to-server calls\"\n    in: header\n    header: Authorization\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"JWT returned by signup/signin, valid 1 hour\"\n  - type: oauth2\n    flow: authorizationCode\n    description: \"Google OAuth sign-in\"\n    authorizationUrl: https://aaly.io/docs/auth#google-sign-in\n    scopes: {}\n"
source_yaml_url: https://artifacts.apis.io/aaly-io/authentication/aaly-io-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Backend
- Multi-Tenant
- Software-as-a-Service
- Platform
---
