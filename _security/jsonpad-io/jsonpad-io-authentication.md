---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jsonpad-io-openapi-generated.yml
  format: yaml
  label: jsonpad-io API
  slug: jsonpad-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jsonpad-io/openapi/_ae-authored/jsonpad-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Jsonpad Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: jsonpad-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: jsonpad-io
provider_slug: jsonpad-io
scheme_count: 2
schemes:
- description: Token provided via dashboard for API authentication.
  in: header
  name: x-api-token
  type: apiKey
- description: OAuth2 flow for third‑party app integration.
  flows:
    authorizationCode:
      authorizationUrl: https://jsonpad.io/oauth/authorize
      scopes:
        read: Read access
        write: Write access
      tokenUrl: https://jsonpad.io/oauth/token
  type: oauth2
slug: jsonpad-io-authentication
source_filename: jsonpad-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: \"https://jsonpad.io/docs/talking-to-the-api.md\"\nschemes:\n  - type: apiKey\n    name: \"x-api-token\"\n    in: header\n    description: \"Token provided via dashboard for API authentication.\"\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://jsonpad.io/oauth/authorize\"\n        tokenUrl: \"https://jsonpad.io/oauth/token\"\n        scopes:\n          read: \"Read access\"\n          write: \"Write access\"\n    description: \"OAuth2 flow for third‑party app integration.\"\n"
source_yaml_url: https://artifacts.apis.io/jsonpad-io/authentication/jsonpad-io-authentication.yml
summary_line: 2 schemes
tags:
- JSON Storage
- REST API
- No-Code Backend
- Real-time Updates
- Versioning
---
