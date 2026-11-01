---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Docsautomator Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: docsautomator-co declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: docsautomator-co
provider_slug: docsautomator-co
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token authentication via Authorization header.
  scheme: bearer
  type: http
- description: API key passed in X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
slug: docsautomator-co-authentication
source_filename: docsautomator-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: \"https://docsautomator.co/docs/api-reference/introduction.md\"\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Bearer token authentication via Authorization header.\"\n    bearerFormat: JWT\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: \"API key passed in X-API-Key header.\"\n"
source_yaml_url: https://artifacts.apis.io/docsautomator-co/authentication/docsautomator-co-authentication.yml
summary_line: 2 schemes
tags:
- DocumentAutomation
- NoCode
- AI
- ESignature
- Integration
---
