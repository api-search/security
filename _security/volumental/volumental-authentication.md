---
anonymous_access: false
api_key_in: []
api_specs:
- filename: volumental-openapi-generated.yml
  format: yaml
  label: Volumental API
  slug: volumental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/openapi/_ae-authored/volumental-openapi-generated.yml
auth_types: []
description: Authentication to Volumental API is performed using a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Volumental Authentication
name_suffix: Authentication
oauth_flows: []
overview: Volumental declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Volumental
provider_slug: volumental
scheme_count: 1
schemes:
- evidence: JWT Authorization header using the Bearer scheme.
  header: Authorization
  how_to_obtain: POST to /v1/auth with JSON body containing client_id and client_secret; the response includes an access_token field.
  location: header
  name: bearerAuth
  token_url: /v1/auth
  type: http-bearer
slug: volumental-authentication
source_filename: volumental-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.volumental.com/reference/welcome-1.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.volumental.com/reference/welcome-1.md\nsources:\n- https://developer.volumental.com/reference/welcome-1.md\n- https://developer.volumental.com/reference/auth.md\n- https://developer.volumental.com/docs/getting-started-recommendations.md\n- https://developer.volumental.com/docs/getting-started-with-measurements-service.md\ndescription: Authentication to Volumental API is performed using a bearer token.\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: JWT Authorization header using the Bearer scheme.\n  location: header\n  header: Authorization\n  token_url: /v1/auth\n  how_to_obtain: POST to /v1/auth with JSON body containing client_id and client_secret; the response includes an access_token field.\ndocs: https://developer.volumental.com/reference/welcome-1.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volumental/refs/heads/main/authentication/volumental-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Retail
- Footwear
- 3DScanning
- AI
---
