---
anonymous_access: false
api_key_in: []
api_specs:
- filename: offnadir-delta-com-openapi-generated.yml
  format: yaml
  label: Off-Nadir Delta API
  slug: offnadir-delta-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/offnadir-delta-com/openapi/_ae-authored/offnadir-delta-com-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Off-Nadir Delta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Off-Nadir Delta declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Off-Nadir Delta
provider_slug: offnadir-delta-com
scheme_count: 1
schemes:
- evidence: 'Authenticate with Authorization: Bearer ond_… (create a key at /account/api ).'
  header: Authorization
  how_to_obtain: Create an API key at /account/api and use the key prefixed with "ond_" as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: offnadir-delta-com-authentication
source_filename: offnadir-delta-com-authentication.yml
source_heading: Authentication Profile
source_url: https://offnadir-delta.com/docs/recipes/first-signals-query
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://offnadir-delta.com/docs/recipes/first-signals-query\nsources:\n- https://offnadir-delta.com/docs/recipes/first-signals-query\n- https://offnadir-delta.com/token-guide\n- https://offnadir-delta.com/guide\n- https://offnadir-delta.com/blog/getting-started-sentinel-1-sar\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authenticate with Authorization: Bearer ond_… (create a key at /account/api ).'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key at /account/api and use the key prefixed with \"ond_\" as the Bearer token.\ndocs: https://offnadir-delta.com/docs/recipes/first-signals-query\n"
source_yaml_url: https://artifacts.apis.io/offnadir-delta-com/authentication/offnadir-delta-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- GEOINT
- OSINT
- Satellite
- Event Intelligence
---
