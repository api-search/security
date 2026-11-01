---
anonymous_access: false
api_key_in: []
api_specs:
- filename: n0t1fy-dev-health-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Health API
  slug: n0t1fy-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-health-api-openapi.yml
- filename: n0t1fy-dev-keys-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Keys API
  slug: n0t1fy-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-keys-api-openapi.yml
- filename: n0t1fy-dev-messages-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Messages API
  slug: n0t1fy-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-messages-api-openapi.yml
- filename: n0t1fy-dev-verifications-api-openapi.yml
  format: yaml
  label: n0t1fy-dev Verifications API
  slug: n0t1fy-dev-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/n0t1fy-dev/openapi/n0t1fy-dev-verifications-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: N0T1Fy Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: n0t1fy-dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: n0t1fy-dev
provider_slug: n0t1fy-dev
scheme_count: 1
schemes:
- description: 'An API key: `sk_test_…` (fake provider, never sends) or `sk_live_…`. Get a test key from `POST /v1/test-keys`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/n0t1fy-dev-api-openapi.json
  - openapi/n0t1fy-dev-openapi.json
  type: http
slug: n0t1fy-dev-authentication
source_filename: n0t1fy-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/n0t1fy-dev-api-openapi.json, openapi/n0t1fy-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key: `sk_test_…` (fake provider, never sends) or `sk_live_…`. Get a test\n    key from `POST /v1/test-keys`.'\n  sources:\n  - openapi/n0t1fy-dev-api-openapi.json\n  - openapi/n0t1fy-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/n0t1fy-dev/authentication/n0t1fy-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SMS
- Georgia
- Transactional
- Developer-First
---
