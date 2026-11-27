---
anonymous_access: false
api_key_in: []
api_specs:
- filename: day3-app-openapi-generated.yml
  format: yaml
  label: day3 API
  slug: day3-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/day3-app/openapi/_ae-authored/day3-app-openapi-generated.yml
auth_types: []
description: Authentication schemes for day3 API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: day3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: day3 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: day3
provider_slug: day3-app
scheme_count: 1
schemes:
- evidence: 'Every request carries an API key as a bearer token: Authorization: Bearer day3_live_x7Kj9mP2...'
  header: Authorization
  how_to_obtain: Admins create and revoke keys in the app under API keys.
  location: header
  name: Bearer
  scopes:
  - campaigns:send
  - automations:enroll
  - webhooks:manage
  type: http-bearer
slug: day3-app-authentication
source_filename: day3-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.day3.app/authentication
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.day3.app/authentication\nsources:\n- https://docs.day3.app/authentication\n- https://docs.day3.app/quickstart\ndescription: Authentication schemes for day3 API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request carries an API key as a bearer token: Authorization: Bearer day3_live_x7Kj9mP2...'\n  location: header\n  header: Authorization\n  scopes:\n  - campaigns:send\n  - automations:enroll\n  - webhooks:manage\n  how_to_obtain: Admins create and revoke keys in the app under API keys.\nnote: No other authentication methods (e.g., OAuth2, apiKey in query, etc.) are documented.\ndocs: https://docs.day3.app/authentication\n"
source_yaml_url: https://artifacts.apis.io/day3-app/authentication/day3-app-authentication.yml
summary_line: 1 scheme
tags:
- Email Marketing
- Transactional Email
- Software-as-a-Service
- Startup Tools
---
