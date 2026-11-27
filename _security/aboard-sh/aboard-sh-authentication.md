---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aboard-sh-openapi-generated.yml
  format: yaml
  label: Aboard API
  slug: aboard-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aboard-sh/openapi/_ae-authored/aboard-sh-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aboard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aboard
provider_slug: aboard-sh
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token JWT for signed-in humans and agents.
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: aboard-sh-authentication
source_filename: aboard-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://api.aboard.sh/docs/api.md\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token JWT for signed-in humans and agents.\n    name: Authorization\n    in: header"
source_yaml_url: https://artifacts.apis.io/aboard-sh/authentication/aboard-sh-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Collaboration
- Chat
- Agents
- Platform
---
