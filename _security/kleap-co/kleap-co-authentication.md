---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kleap-co-account-api-openapi.yml
  format: yaml
  label: Kleap Account API
  slug: kleap-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-account-api-openapi.yml
- filename: kleap-co-apps-api-openapi.yml
  format: yaml
  label: Kleap Apps API
  slug: kleap-co-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-apps-api-openapi.yml
- filename: kleap-co-auth-api-openapi.yml
  format: yaml
  label: Kleap Auth API
  slug: kleap-co-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-auth-api-openapi.yml
- filename: kleap-co-tasks-api-openapi.yml
  format: yaml
  label: Kleap Tasks API
  slug: kleap-co-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleap-co/openapi/kleap-co-tasks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kleap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kleap declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kleap
provider_slug: kleap-co
scheme_count: 1
schemes:
- evidence: 'API key obtained from POST /api/v1/auth/keys. Pass as Authorization: Bearer kleap_live_sk_...'
  header: Authorization
  how_to_obtain: POST /api/v1/auth/keys
  location: header
  name: Authorization
  type: apiKey
slug: kleap-co-authentication
source_filename: kleap-co-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.kleap.co/reference#POST/auth/keys
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.kleap.co/reference#POST/auth/keys\nsources:\n- https://developers.kleap.co/reference#POST/auth/keys\n- https://developers.kleap.co/reference#GET/auth/keys\n- https://developers.kleap.co/reference#DELETE/auth/keys/{keyId}\n- https://developers.kleap.co/reference\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'API key obtained from POST /api/v1/auth/keys. Pass as Authorization: Bearer kleap_live_sk_...'\n  location: header\n  header: Authorization\n  how_to_obtain: POST /api/v1/auth/keys\ndocs: https://developers.kleap.co/reference#POST/auth/keys\n"
source_yaml_url: https://artifacts.apis.io/kleap-co/authentication/kleap-co-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Website Builder
- No-Code
- Entrepreneurship
- Software-as-a-Service
---
