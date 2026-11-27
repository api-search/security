---
anonymous_access: false
api_key_in: []
api_specs:
- filename: numberbroom-com-credits-api-openapi.yml
  format: yaml
  label: NumberBroom Credits API
  slug: numberbroom-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberbroom-com/openapi/numberbroom-com-credits-api-openapi.yml
- filename: numberbroom-com-lists-api-openapi.yml
  format: yaml
  label: NumberBroom Lists API
  slug: numberbroom-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberbroom-com/openapi/numberbroom-com-lists-api-openapi.yml
- filename: numberbroom-com-verify-api-openapi.yml
  format: yaml
  label: NumberBroom Verify API
  slug: numberbroom-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberbroom-com/openapi/numberbroom-com-verify-api-openapi.yml
auth_types: []
description: 'NumberBroom uses a single credential: an API key sent as a Bearer token in the Authorization header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NumberBroom Authentication
name_suffix: Authentication
oauth_flows: []
overview: NumberBroom declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NumberBroom
provider_slug: numberbroom-com
scheme_count: 1
schemes:
- evidence: 'There is one credential: an API key, sent as a Bearer token.'
  header: Authorization
  how_to_obtain: Create an API key in Settings after signing in at https://numberbroom.com/login; the key starts with `nb_live_`.
  location: header
  name: Bearer
  type: http-bearer
slug: numberbroom-com-authentication
source_filename: numberbroom-com-authentication.yml
source_heading: Authentication Profile
source_url: https://numberbroom.com/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://numberbroom.com/auth.md\nsources:\n- https://numberbroom.com/auth.md\ndescription: 'NumberBroom uses a single credential: an API key sent as a Bearer token in the Authorization header.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'There is one credential: an API key, sent as a Bearer token.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings after signing in at https://numberbroom.com/login; the key starts with `nb_live_`.\ndocs: https://numberbroom.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/numberbroom-com/authentication/numberbroom-com-authentication.yml
summary_line: 1 scheme
tags:
- Phone
- Data
- Validation
- Scrubbing
- Real Estate
---
