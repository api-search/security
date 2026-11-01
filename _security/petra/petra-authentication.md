---
anonymous_access: false
api_key_in: []
api_specs:
- filename: petra-openapi.json
  format: json
  label: Petra Security API
  slug: petra-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/petra/openapi/petra-openapi.json
auth_types: []
description: The Petra Security API uses Bearer token authentication. Every request to the API must include a valid API key in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Petra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Petra declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Petra
provider_slug: petra
scheme_count: 1
schemes:
- evidence: The Petra Security API uses Bearer token authentication. Every request to the API must include a valid API key in the Authorization header.
  header: Authorization
  how_to_obtain: API keys are managed in Settings → API Keys. Admins can create keys via the app.petrasecurity.com UI.
  location: header
  name: Bearer
  type: http-bearer
slug: petra-authentication
source_filename: petra-authentication.yml
source_heading: Authentication Profile
source_url: https://www.petrasecurity.com/docs/api-reference/authentication
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.petrasecurity.com/docs/api-reference/authentication\nsources:\n- https://www.petrasecurity.com/docs/api-reference/authentication\ndescription: The Petra Security API uses Bearer token authentication. Every request to the API must include a valid API key in the Authorization\n  header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: The Petra Security API uses Bearer token authentication. Every request to the API must include a valid API key in the Authorization\n    header.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are managed in Settings → API Keys. Admins can create keys via the app.petrasecurity.com UI.\ndocs: https://www.petrasecurity.com/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/petra/authentication/petra-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- ITDR
- Software-as-a-Service
- Threat Detection
---
