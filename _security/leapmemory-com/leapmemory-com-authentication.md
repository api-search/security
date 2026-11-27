---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leapmemory-com-api-openapi.json
  format: json
  label: LeapMemory Api API
  slug: leapmemory-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leapmemory-com/openapi/_original/leapmemory-com-api-openapi.json
auth_types: []
description: Authentication uses a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LeapMemory Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeapMemory declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LeapMemory
provider_slug: leapmemory-com
scheme_count: 1
schemes:
- evidence: 'Every request authenticates with the same header: HTTP Copy Authorization: Bearer lm_sk_your_key_here'
  header: Authorization
  how_to_obtain: Generate an API key in the dashboard; the key is shown once when created and used as a Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: leapmemory-com-authentication
source_filename: leapmemory-com-authentication.yml
source_heading: Authentication Profile
source_url: https://leapmemory.com/docs/quickstart
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://leapmemory.com/docs/quickstart\nsources:\n- https://leapmemory.com/docs/quickstart\ndescription: Authentication uses a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request authenticates with the same header: HTTP Copy Authorization: Bearer lm_sk_your_key_here'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the dashboard; the key is shown once when created and used as a Bearer token.\ndocs: https://leapmemory.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/leapmemory-com/authentication/leapmemory-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Platform
- Developer Tools
- Tallinn
---
