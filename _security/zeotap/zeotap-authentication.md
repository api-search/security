---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zeotap-openapi.yml
  format: yaml
  label: Zeotap Profile API
  slug: zeotap-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zeotap/openapi/zeotap-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zeotap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeotap declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zeotap
provider_slug: zeotap
scheme_count: 2
schemes:
- description: API Key authentication, provided by Zeotap organization.
  in: header
  name: apikey
  type: apiKey
- bearerFormat: JWT
  description: Okta JWT authentication (mentioned in OpenAPI, not documented here).
  scheme: bearer
  type: http
slug: zeotap-authentication
source_filename: zeotap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.zeotap.com/profile-api/profileapi.md\nschemes:\n  - type: apiKey\n    name: apikey\n    in: header\n    description: API Key authentication, provided by Zeotap organization.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Okta JWT authentication (mentioned in OpenAPI, not documented here).\n"
source_yaml_url: https://artifacts.apis.io/zeotap/authentication/zeotap-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Customer-Data-Platform
- Data-Integration
- Identity-Resolution
---
