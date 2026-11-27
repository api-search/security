---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fintechstudios-com-openapi-generated.yml
  format: yaml
  label: FinTech Studios API
  slug: fintechstudios-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fintechstudios-com/openapi/_ae-authored/fintechstudios-com-openapi-generated.yml
auth_types: []
description: Authentication methods as published on FinTech Studios documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FinTech Studios Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinTech Studios declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FinTech Studios
provider_slug: fintechstudios-com
scheme_count: 2
schemes:
- evidence: Keys are provided by adding an x-api-key header to your request, with your key as the value.
  header: x-api-key
  how_to_obtain: Contact your account manager or sales representative to receive a 36‑character UUID access key.
  location: header
  name: FTS API Key
  type: apiKey
- evidence: 'To authorize API requests using the token, simply add the JWT as a bearer token to the Authorization header in each request: authorization : Bearer eyJhbGciOiJSUzI1NiIsIn...'
  header: Authorization
  how_to_obtain: 'Make a POST request to the /auth/login endpoint with JSON body { "email": "string", "password": "string" } to receive a JWT in the "token" field of the response.'
  location: header
  name: JWT Access Token
  type: http-bearer
slug: fintechstudios-com-authentication
source_filename: fintechstudios-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fintechstudios.com/en/latest/api/authentication/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fintechstudios.com/en/latest/api/authentication/\nsources:\n- https://docs.fintechstudios.com/en/latest/api/authentication/\n- https://docs.fintechstudios.com/en/latest/api/vibe-coding/authentication-instructions/\n- https://docs.fintechstudios.com/en/latest/lrcm/getting-set-up/\n- https://docs.fintechstudios.com/en/latest/api/vibe-coding/reglens-api-setup/\ndescription: Authentication methods as published on FinTech Studios documentation\nschemes:\n- type: apiKey\n  name: FTS API Key\n  evidence: Keys are provided by adding an x-api-key header to your request, with your key as the value.\n  location: header\n  header: x-api-key\n  how_to_obtain: Contact your account manager or sales representative to receive a 36‑character UUID access key.\n- type: http-bearer\n  name: JWT Access Token\n  evidence: 'To authorize API requests using the token, simply add the JWT as a\
  \ bearer token to the Authorization header in each request: authorization\n    : Bearer eyJhbGciOiJSUzI1NiIsIn...'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Make a POST request to the /auth/login endpoint with JSON body { \"email\": \"string\", \"password\": \"string\" } to receive a JWT\n    in the \"token\" field of the response.'\nnote: No OAuth2 flows, scopes, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.fintechstudios.com/en/latest/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/fintechstudios-com/authentication/fintechstudios-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Intelligence
- Real-Time
- News
- Data
---
