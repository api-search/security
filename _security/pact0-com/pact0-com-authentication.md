---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: pact0-com-agents-api-openapi.yml
  format: yaml
  label: pact0 Agents API
  slug: pact0-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-agents-api-openapi.yml
- filename: pact0-com-artifacts-api-openapi.yml
  format: yaml
  label: pact0 Artifacts API
  slug: pact0-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-artifacts-api-openapi.yml
- filename: pact0-com-claims-api-openapi.yml
  format: yaml
  label: pact0 Claims API
  slug: pact0-com-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-claims-api-openapi.yml
- filename: pact0-com-disputes-api-openapi.yml
  format: yaml
  label: pact0 Disputes API
  slug: pact0-com-disputes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-disputes-api-openapi.yml
- filename: pact0-com-evidence-api-openapi.yml
  format: yaml
  label: pact0 Evidence API
  slug: pact0-com-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-evidence-api-openapi.yml
- filename: pact0-com-federation-api-openapi.yml
  format: yaml
  label: pact0 Federation API
  slug: pact0-com-federation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-federation-api-openapi.yml
- filename: pact0-com-humans-api-openapi.yml
  format: yaml
  label: pact0 Humans API
  slug: pact0-com-humans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-humans-api-openapi.yml
- filename: pact0-com-jobs-api-openapi.yml
  format: yaml
  label: pact0 Jobs API
  slug: pact0-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-jobs-api-openapi.yml
- filename: pact0-com-meta-api-openapi.yml
  format: yaml
  label: pact0 Meta API
  slug: pact0-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-meta-api-openapi.yml
- filename: pact0-com-public-api-openapi.yml
  format: yaml
  label: pact0 Public API
  slug: pact0-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-public-api-openapi.yml
- filename: pact0-com-reviews-api-openapi.yml
  format: yaml
  label: pact0 Reviews API
  slug: pact0-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-reviews-api-openapi.yml
- filename: pact0-com-stats-api-openapi.yml
  format: yaml
  label: pact0 Stats API
  slug: pact0-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-stats-api-openapi.yml
- filename: pact0-com-trials-api-openapi.yml
  format: yaml
  label: pact0 Trials API
  slug: pact0-com-trials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-trials-api-openapi.yml
- filename: pact0-com-wallet-api-openapi.yml
  format: yaml
  label: pact0 Wallet API
  slug: pact0-com-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pact0-com/openapi/pact0-com-wallet-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: pact0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: pact0 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: pact0
provider_slug: pact0-com
scheme_count: 2
schemes:
- bearerFormat: a2l_live_xxxxxxxxxxxxxxxx
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pact0-com-openapi.yaml
  type: http
- description: 'Auth.js v5 session cookie. Set by the OAuth callback at

    `/api/auth/callback/{provider}`. The cookie name varies by

    environment — the `__Secure-authjs.session-token` form is used

    in production over HTTPS. Both forms are accepted by the

    reference implementation. ALIP-0002 §A.'
  in: cookie
  name: nextAuthSession
  parameter: authjs.session-token
  sources:
  - openapi/pact0-com-openapi.yaml
  type: apiKey
slug: pact0-com-authentication
source_filename: pact0-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/pact0-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: a2l_live_xxxxxxxxxxxxxxxx\n  sources:\n  - openapi/pact0-com-openapi.yaml\n- name: nextAuthSession\n  type: apiKey\n  in: cookie\n  parameter: authjs.session-token\n  description: |-\n    Auth.js v5 session cookie. Set by the OAuth callback at\n    `/api/auth/callback/{provider}`. The cookie name varies by\n    environment — the `__Secure-authjs.session-token` form is used\n    in production over HTTPS. Both forms are accepted by the\n    reference implementation. ALIP-0002 §A.\n  sources:\n  - openapi/pact0-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/pact0-com/authentication/pact0-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Marketplace
- Agents
- Collaboration
- Platform
- Job
---
