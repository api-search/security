---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aircube-openapi-generated.yml
  format: yaml
  label: AirCube API
  slug: aircube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aircube/refs/heads/main/openapi/_ae-authored/aircube-openapi-generated.yml
auth_types: []
description: Authentication via API keys
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aircube Authentication
name_suffix: Authentication
oauth_flows: []
overview: AirCube declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AirCube
provider_slug: aircube
scheme_count: 1
schemes:
- evidence: All AirCube API requests require authentication via an API key passed as a Bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the AirCube dashboard (API Keys page) after signing up; the key starts with the prefix sk- and is provided only once.
  location: header
  name: Authorization
  type: apiKey
slug: aircube-authentication
source_filename: aircube-authentication.yml
source_heading: Authentication Profile
source_url: https://aircube.ai/docs/getting-started/authentication
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aircube.ai/docs/getting-started/authentication\nsources:\n- https://aircube.ai/docs/getting-started/authentication\n- https://aircube.ai/docs/getting-started/overview\n- https://aircube.ai/docs/getting-started/quickstart\ndescription: Authentication via API keys\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: All AirCube API requests require authentication via an API key passed as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the AirCube dashboard (API Keys page) after signing up; the key starts with the prefix sk- and is provided\n    only once.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://aircube.ai/docs/getting-started/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircube/refs/heads/main/authentication/aircube-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Platform
- API
- MediaGeneration
- UnifiedAPI
---
