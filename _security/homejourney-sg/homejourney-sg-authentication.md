---
anonymous_access: false
api_key_in: []
api_specs:
- filename: homejourney-sg-openapi-generated.yml
  format: yaml
  label: Homejourney API
  slug: homejourney-sg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homejourney-sg/openapi/_ae-authored/homejourney-sg-openapi-generated.yml
auth_types: []
description: 'Authenticate every request with an API key as a bearer token: Authorization: Bearer <key>. Create keys in the Homejourney developer console.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Homejourney Authentication
name_suffix: Authentication
oauth_flows: []
overview: Homejourney declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Homejourney
provider_slug: homejourney-sg
scheme_count: 1
schemes:
- evidence: 'Authenticate every request with an API key as a bearer token: Authorization: Bearer <key>. Create keys in the Homejourney developer console.'
  header: Authorization
  how_to_obtain: Create keys in the Homejourney developer console.
  location: header
  name: Bearer
  type: http-bearer
slug: homejourney-sg-authentication
source_filename: homejourney-sg-authentication.yml
source_heading: Authentication Profile
source_url: https://www.homejourney.sg/api/platform/v1/docs#tag/onboarding
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.homejourney.sg/api/platform/v1/docs#tag/onboarding\nsources:\n- https://www.homejourney.sg/api/platform/v1/docs#tag/onboarding\n- https://www.homejourney.sg/api/platform/v1/docs\ndescription: 'Authenticate every request with an API key as a bearer token: Authorization: Bearer <key>. Create keys in the Homejourney developer\n  console.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authenticate every request with an API key as a bearer token: Authorization: Bearer <key>. Create keys in the Homejourney developer\n    console.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in the Homejourney developer console.\nnote: No other authentication methods (e.g., OAuth2, apiKey query, etc.) are documented on the provided pages.\ndocs: https://www.homejourney.sg/api/platform/v1/docs#tag/onboarding\n"
source_yaml_url: https://artifacts.apis.io/homejourney-sg/authentication/homejourney-sg-authentication.yml
summary_line: 1 scheme
tags:
- Real Estate
- Mortgage
- Home Services
- Singapore
- Platform
---
