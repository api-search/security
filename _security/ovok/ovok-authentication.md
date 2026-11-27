---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ovok-openapi-generated.yml
  format: yaml
  label: Ovok API
  slug: ovok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ovok/openapi/_ae-authored/ovok-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ovok Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ovok declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ovok
provider_slug: ovok
scheme_count: 1
schemes:
- evidence: 'Send the access token as Authorization: Bearer <accessToken> .'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
slug: ovok-authentication
source_filename: ovok-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ovok.com/authentication
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ovok.com/authentication\nsources:\n- https://docs.ovok.com/authentication\n- https://docs.ovok.com/api/wearables/check-a-wearable-webhook-url-with-a-token\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send the access token as Authorization: Bearer <accessToken> .'\n  location: header\n  header: Authorization\ndocs: https://docs.ovok.com/authentication\n"
source_yaml_url: https://artifacts.apis.io/ovok/authentication/ovok-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- FHIR
- Digital Health
- API Platform
---
