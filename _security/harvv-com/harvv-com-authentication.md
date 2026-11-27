---
anonymous_access: false
api_key_in: []
api_specs:
- filename: harvv-com-openapi-generated.yml
  format: yaml
  label: Harvv API
  slug: harvv-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/harvv-com/openapi/_ae-authored/harvv-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Harvv REST API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Harvv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harvv declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Harvv
provider_slug: harvv-com
scheme_count: 1
schemes:
- evidence: 'Send an API key as a bearer token on every request: Authorization: Bearer hv_live_xxxxxxxxxxxx'
  header: Authorization
  how_to_obtain: Create one in the dashboard under Settings, then API keys.
  location: header
  name: API key
  type: http-bearer
slug: harvv-com-authentication
source_filename: harvv-com-authentication.yml
source_heading: Authentication Profile
source_url: https://harvv.com/docs/api
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://harvv.com/docs/api\nsources:\n- https://harvv.com/docs/api\n- https://harvv.com/docs/claude-skill/harvv-setup.skill\ndescription: Authentication methods for Harvv REST API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send an API key as a bearer token on every request: Authorization: Bearer hv_live_xxxxxxxxxxxx'\n  location: header\n  header: Authorization\n  how_to_obtain: Create one in the dashboard under Settings, then API keys.\ndocs: https://harvv.com/docs/api\n"
source_yaml_url: https://artifacts.apis.io/harvv-com/authentication/harvv-com-authentication.yml
summary_line: 1 scheme
tags:
- Behavioral Analytics
- Website Analytics
- Session Analysis
- dead‑click detection
---
