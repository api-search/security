---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alium-openapi-generated.yml
  format: yaml
  label: Alium API
  slug: alium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alium/refs/heads/main/openapi/_ae-authored/alium-openapi-generated.yml
auth_types: []
description: 'All API requests authenticate with an API key, passed in the Authorization header as "Authorization: Token YOUR_API_KEY".'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Alium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alium declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Alium
provider_slug: alium
scheme_count: 1
schemes:
- evidence: All API requests authenticate with an API key , and every API key belongs to an agent seat (a machine identity — see below).
  header: Authorization
  how_to_obtain: Created and rotated per agent seat under Account → Agent Seats by a customer admin.
  location: header
  name: API key
  type: apiKey
slug: alium-authentication
source_filename: alium-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.alium.io/api/authentication/
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.alium.io/api/authentication/\nsources:\n- https://docs.alium.io/api/authentication/\ndescription: 'All API requests authenticate with an API key, passed in the Authorization header as \"Authorization: Token YOUR_API_KEY\".'\nschemes:\n- type: apiKey\n  name: API key\n  evidence: All API requests authenticate with an API key , and every API key belongs to an agent seat (a machine identity — see below).\n  location: header\n  header: Authorization\n  how_to_obtain: Created and rotated per agent seat under Account → Agent Seats by a customer admin.\ndocs: https://docs.alium.io/api/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alium/refs/heads/main/authentication/alium-authentication.yml
summary_line: 1 scheme
tags:
- Vendor research
- Marketing intelligence
- E‑commerce
- Enterprise tech
---
