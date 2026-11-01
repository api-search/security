---
anonymous_access: false
api_key_in: []
api_specs:
- filename: stract-api-my-user-api-openapi.yml
  format: yaml
  label: Stract API My User API
  slug: stract-api-my-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stract-api/openapi/stract-api-my-user-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Stract Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stract API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Stract API
provider_slug: stract-api
scheme_count: 1
schemes:
- evidence: '-H "authorization: bearer API_KEY"'
  header: authorization
  how_to_obtain: Obtain your API key by going to Account on the navigation bar → API Keys → Generate New API Key.
  location: header
  name: Bearer
  type: http-bearer
slug: stract-api-authentication
source_filename: stract-api-authentication.yml
source_heading: Authentication Profile
source_url: https://stract-api.com/guide/quick-start-api/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://stract-api.com/guide/quick-start-api/\nsources:\n- https://stract-api.com/guide/quick-start-api/\n- https://stract-api.com/guide/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"authorization: bearer API_KEY\"'\n  location: header\n  header: authorization\n  how_to_obtain: Obtain your API key by going to Account on the navigation bar → API Keys → Generate New API Key.\ndocs: https://stract-api.com/guide/quick-start-api/\n"
source_yaml_url: https://artifacts.apis.io/stract-api/authentication/stract-api-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Document-Processing
- Data-Extraction
- SaaS
---
