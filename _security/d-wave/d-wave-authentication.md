---
api_key_in:
- header
api_specs:
- filename: d-wave-solvers-api-openapi.yml
  format: yaml
  label: D-Wave Solver API (SAPI) - Solvers
  slug: d-wave-solver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-solvers-api-openapi.yml
- filename: d-wave-problems-api-openapi.yml
  format: yaml
  label: D-Wave Solver API (SAPI) - Problems
  slug: d-wave-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-problems-api-openapi.yml
- filename: d-wave-metadata-api-openapi.yml
  format: yaml
  label: D-Wave Metadata API - Regions
  slug: d-wave-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-metadata-api-openapi.yml
- filename: d-wave-leap-account-api-openapi.yml
  format: yaml
  label: D-Wave Leap Account API
  slug: d-wave-leap-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-leap-account-api-openapi.yml
- filename: d-wave-hybrid-solvers-openapi.yml
  format: yaml
  label: D-Wave Leap Hybrid Solvers
  slug: d-wave-hybrid-solvers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-hybrid-solvers-openapi.yml
- filename: d-wave-qpu-samplers-openapi.yml
  format: yaml
  label: D-Wave QPU Samplers (Advantage / Advantage2)
  slug: d-wave-qpu-samplers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-qpu-samplers-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: D Wave Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: D-Wave secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: D-Wave
provider_slug: d-wave
scheme_count: 2
schemes:
- in: header
  name: SapiToken
  parameter: X-Auth-Token
  sources:
  - openapi/d-wave-hybrid-solvers-openapi.yml
  - openapi/d-wave-metadata-api-openapi.yml
  - openapi/d-wave-problems-api-openapi.yml
  - openapi/d-wave-qpu-samplers-openapi.yml
  - openapi/d-wave-solvers-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://cloud.dwavesys.com/leap/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://cloud.dwavesys.com/leap/oauth/token
  name: LeapOAuth
  sources:
  - openapi/d-wave-leap-account-api-openapi.yml
  type: oauth2
slug: d-wave-authentication
source_filename: d-wave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/d-wave-hybrid-solvers-openapi.yml, openapi/d-wave-leap-account-api-openapi.yml,\n  openapi/d-wave-metadata-api-openapi.yml, openapi/d-wave-problems-api-openapi.yml, openapi/d-wave-qpu-samplers-openapi.yml,\n  openapi/d-wave-solvers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: SapiToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/d-wave-hybrid-solvers-openapi.yml\n  - openapi/d-wave-metadata-api-openapi.yml\n  - openapi/d-wave-problems-api-openapi.yml\n  - openapi/d-wave-qpu-samplers-openapi.yml\n  - openapi/d-wave-solvers-api-openapi.yml\n- name: LeapOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.dwavesys.com/leap/oauth/authorize\n    tokenUrl: https://cloud.dwavesys.com/leap/oauth/token\n    scopes: 1\n  sources:\n  - openapi/d-wave-leap-account-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/authentication/d-wave-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Quantum Computing
- Quantum Annealing
- Optimization
- Hybrid Quantum-Classical
- Ising
- QUBO
- Industrial Optimization
- Sampling
- Leap
- Ocean SDK
- SAPI
---
