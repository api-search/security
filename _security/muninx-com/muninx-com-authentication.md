---
anonymous_access: false
api_key_in: []
api_specs:
- filename: muninx-com-openapi-generated.yml
  format: yaml
  label: Muninx API
  slug: muninx-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/muninx-com/openapi/_ae-authored/muninx-com-openapi-generated.yml
auth_types: []
description: Authentication methods as published on Muninx documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Muninx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Muninx declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Muninx
provider_slug: muninx-com
scheme_count: 1
schemes:
- evidence: Most Muninx API endpoints require a bearer token.
  header: Authorization
  how_to_obtain: Create a personal API token in Settings > API Tokens, then send the token in the Authorization header as "Bearer <token>".
  location: header
  name: Bearer
  type: http-bearer
slug: muninx-com-authentication
source_filename: muninx-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.muninx.com/api/authentication/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.muninx.com/api/authentication/\nsources:\n- https://docs.muninx.com/api/authentication/\n- https://docs.muninx.com/api/reference/operations/tags/oauth/\n- https://docs.muninx.com/api/reference/operations/authoauthauthorizationservermetadata/\n- https://docs.muninx.com/api/reference/operations/authopenidconfiguration/\ndescription: Authentication methods as published on Muninx documentation.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Most Muninx API endpoints require a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal API token in Settings > API Tokens, then send the token in the Authorization header as \"Bearer <token>\".\nnote: No other authentication schemes (apiKey, oauth2, http-basic, etc.) are described on the referenced pages.\ndocs: https://docs.muninx.com/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/muninx-com/authentication/muninx-com-authentication.yml
summary_line: 1 scheme
tags:
- Help Desk
- Software-as-a-Service
- Customer Service
- Artificial Intelligence
- Free Tier
---
