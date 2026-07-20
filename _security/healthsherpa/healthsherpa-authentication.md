---
api_key_in:
- header
api_specs:
- filename: healthsherpa-one-openapi.json
  format: json
  label: HealthSherpa Public API (ONE)
  slug: healthsherpa-public-api-one
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/openapi/healthsherpa-one-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Healthsherpa Authentication
name_suffix: Authentication
oauth_flows: []
overview: HealthSherpa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HealthSherpa
provider_slug: healthsherpa
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/healthsherpa-one-openapi.json
  type: apiKey
slug: healthsherpa-authentication
source_filename: healthsherpa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/healthsherpa-one-openapi.json\ndocs: https://one.healthsherpa.com/docs.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Single scheme on the public ONE API. Keys are issued at onboarding and revealed once in the\n    passwordless developer portal; server-side use only. No OAuth, sessions, or HMAC signing on ONE.\n    (Separately, the HealthSherpa Medicare Partner API offers v1 API keys and a v2 OAuth flow, and\n    the ICHRA Partner API also uses x-api-key — those surfaces publish no OpenAPI.)\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/healthsherpa-one-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthsherpa/refs/heads/main/authentication/healthsherpa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Health Insurance
- Healthcare
- ACA
- Enrollment
- Quoting
- Insurance
- Enhanced Direct Enrollment
- ICHRA
---
