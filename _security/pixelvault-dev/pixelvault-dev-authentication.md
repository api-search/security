---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pixelvault Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: pixelvault-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pixelvault-dev
provider_slug: pixelvault-dev
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: All API requests (except registration) require a Bearer token. Production keys start with pv_live_, test keys with pv_test_.
  scheme: bearer
  type: http
slug: pixelvault-dev-authentication
source_filename: pixelvault-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://pixelvault.dev/docs.md\nschemes:\n  - type: \"http\"\n    scheme: \"bearer\"\n    bearerFormat: \"JWT\"\n    description: \"All API requests (except registration) require a Bearer token. Production keys start with pv_live_, test keys with pv_test_.\"\n"
source_yaml_url: https://artifacts.apis.io/pixelvault-dev/authentication/pixelvault-dev-authentication.yml
summary_line: 1 scheme
tags:
- Image Hosting
- CDN
- API
- AI Agents
- Developer Tools
---
