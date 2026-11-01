---
anonymous_access: false
api_key_in: []
api_specs:
- filename: readwise-openapi-generated.yml
  format: yaml
  label: Readwise API
  slug: readwise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/readwise/openapi/_ae-authored/readwise-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Readwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Readwise declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Readwise
provider_slug: readwise
scheme_count: 1
schemes:
- authorizationUrl: https://readwise.io/accounts/login/
  description: Login command opens browser for OAuth flow.
  flow: authorization_code
  scopes: []
  tokenUrl: https://readwise.io/accounts/login/
  type: oauth2
slug: readwise-authentication
source_filename: readwise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.readwise.io/tools/cli\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: \"https://readwise.io/accounts/login/\"\n    tokenUrl: \"https://readwise.io/accounts/login/\"\n    scopes: []\n    description: \"Login command opens browser for OAuth flow.\"\n"
source_yaml_url: https://artifacts.apis.io/readwise/authentication/readwise-authentication.yml
summary_line: 1 scheme
tags:
- Reading
- Productivity
- Knowledge Management
- SaaS
- API
---
