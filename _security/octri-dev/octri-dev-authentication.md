---
anonymous_access: false
api_key_in: []
api_specs:
- filename: octri-dev-openapi-generated.yml
  format: yaml
  label: Octri API
  slug: octri-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octri-dev/openapi/_ae-authored/octri-dev-openapi-generated.yml
auth_types: []
description: Octri authentication schemes as described in the documentation.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Octri Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octri declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Octri
provider_slug: octri-dev
scheme_count: 4
schemes:
- evidence: apiKey A key in a header
  location: header
  name: apiKey
  type: apiKey
- evidence: 'basic Authorization: Basic <base64 user:pass>'
  header: Authorization
  location: header
  name: basic
  type: http-basic
- evidence: 'bearer Authorization: Bearer <token>'
  header: Authorization
  location: header
  name: bearer
  type: http-bearer
- evidence: oauth2 A bearer token obtained through an OAuth2 flow
  name: oauth2
  type: oauth2
slug: octri-dev-authentication
source_filename: octri-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://octri.dev/blog/api-playground-credential-path
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://octri.dev/blog/api-playground-credential-path\nsources:\n- https://octri.dev/blog/api-playground-credential-path\n- https://octri.dev/developers/guides/sdks/authentication\n- https://octri.dev/developers/guides/monitoring/setup\n- https://octri.dev/developers/guides/cli/ci\ndescription: Octri authentication schemes as described in the documentation.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: apiKey A key in a header\n  location: header\n- type: http-basic\n  name: basic\n  evidence: 'basic Authorization: Basic <base64 user:pass>'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: bearer\n  evidence: 'bearer Authorization: Bearer <token>'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: oauth2\n  evidence: oauth2 A bearer token obtained through an OAuth2 flow\ndocs: https://octri.dev/blog/api-playground-credential-path\n"
source_yaml_url: https://artifacts.apis.io/octri-dev/authentication/octri-dev-authentication.yml
summary_line: 4 schemes
tags:
- Company
- API
- Documentation
- SDK
- Monitoring
- MCP
---
