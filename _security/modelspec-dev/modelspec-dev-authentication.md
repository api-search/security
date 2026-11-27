---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: modelspec-dev-auth-check-api-openapi.yml
  format: yaml
  label: modelspec-dev Auth Check API
  slug: modelspec-dev-auth-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-auth-check-api-openapi.yml
- filename: modelspec-dev-billing-api-openapi.yml
  format: yaml
  label: modelspec-dev Billing API
  slug: modelspec-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-billing-api-openapi.yml
- filename: modelspec-dev-compare-api-openapi.yml
  format: yaml
  label: modelspec-dev Compare API
  slug: modelspec-dev-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-compare-api-openapi.yml
- filename: modelspec-dev-compare-models-api-openapi.yml
  format: yaml
  label: modelspec-dev Compare Models API
  slug: modelspec-dev-compare-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-compare-models-api-openapi.yml
- filename: modelspec-dev-credits-api-openapi.yml
  format: yaml
  label: modelspec-dev Credits API
  slug: modelspec-dev-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-credits-api-openapi.yml
- filename: modelspec-dev-decide-api-openapi.yml
  format: yaml
  label: modelspec-dev Decide API
  slug: modelspec-dev-decide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-decide-api-openapi.yml
- filename: modelspec-dev-feedback-api-openapi.yml
  format: yaml
  label: modelspec-dev Feedback API
  slug: modelspec-dev-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-feedback-api-openapi.yml
- filename: modelspec-dev-hardware-fit-api-openapi.yml
  format: yaml
  label: modelspec-dev Hardware Fit API
  slug: modelspec-dev-hardware-fit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-hardware-fit-api-openapi.yml
- filename: modelspec-dev-health-api-openapi.yml
  format: yaml
  label: modelspec-dev Health API
  slug: modelspec-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-health-api-openapi.yml
- filename: modelspec-dev-human-status-api-openapi.yml
  format: yaml
  label: modelspec-dev Human Status API
  slug: modelspec-dev-human-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-human-status-api-openapi.yml
- filename: modelspec-dev-policy-check-api-openapi.yml
  format: yaml
  label: modelspec-dev Policy Check API
  slug: modelspec-dev-policy-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-policy-check-api-openapi.yml
- filename: modelspec-dev-rank-api-openapi.yml
  format: yaml
  label: modelspec-dev Rank API
  slug: modelspec-dev-rank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-rank-api-openapi.yml
- filename: modelspec-dev-signals-api-openapi.yml
  format: yaml
  label: modelspec-dev Signals API
  slug: modelspec-dev-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-signals-api-openapi.yml
- filename: modelspec-dev-visit-token-api-openapi.yml
  format: yaml
  label: modelspec-dev Visit Token API
  slug: modelspec-dev-visit-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-visit-token-api-openapi.yml
- filename: modelspec-dev-vocabulary-api-openapi.yml
  format: yaml
  label: modelspec-dev Vocabulary API
  slug: modelspec-dev-vocabulary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modelspec-dev/openapi/modelspec-dev-vocabulary-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: modelspec-dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: modelspec-dev secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: modelspec-dev
provider_slug: modelspec-dev
scheme_count: 4
schemes:
- description: 'Authorization: Bearer <key>. Takes precedence.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/modelspec-dev-openapi.yaml
  type: http
- description: 'X-API-Key: <key>. Never in the query string.'
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/modelspec-dev-openapi.yaml
  type: apiKey
- description: sha256=<HMAC-SHA256 of the exact request bytes>.
  in: header
  name: signalHmac
  parameter: X-ModelSpec-Signature
  sources:
  - openapi/modelspec-dev-openapi.yaml
  type: apiKey
- description: Human browser credential from the Turnstile-verified visit gate. Bound to the visitor and allowed site origin; admits only decide and vocabulary. Machine callers use an API key.
  in: header
  name: visitToken
  parameter: X-ModelSpec-Visit-Token
  sources:
  - openapi/modelspec-dev-openapi.yaml
  type: apiKey
slug: modelspec-dev-authentication
source_filename: modelspec-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/modelspec-dev-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <key>. Takes precedence.'\n  sources:\n  - openapi/modelspec-dev-openapi.yaml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'X-API-Key: <key>. Never in the query string.'\n  sources:\n  - openapi/modelspec-dev-openapi.yaml\n- name: signalHmac\n  type: apiKey\n  in: header\n  parameter: X-ModelSpec-Signature\n  description: sha256=<HMAC-SHA256 of the exact request bytes>.\n  sources:\n  - openapi/modelspec-dev-openapi.yaml\n- name: visitToken\n  type: apiKey\n  in: header\n  parameter: X-ModelSpec-Visit-Token\n  description: Human browser credential from the Turnstile-verified visit gate. Bound to the\n    visitor and allowed site origin; admits only decide and vocabulary. Machine callers\
  \ use\n    an API key.\n  sources:\n  - openapi/modelspec-dev-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/modelspec-dev/authentication/modelspec-dev-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- AI Model Selection
- Cost Analysis
---
