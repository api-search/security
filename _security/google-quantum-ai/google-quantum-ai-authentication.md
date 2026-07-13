---
api_key_in: []
api_specs:
- filename: quantum-engine-api-openapi.yml
  format: yaml
  label: Google Quantum Engine API
  slug: quantum-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/quantum-engine-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Quantum Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Quantum AI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Quantum AI
provider_slug: google-quantum-ai
scheme_count: 1
schemes:
- description: OAuth 2.0 via Google Cloud Application Default Credentials.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  sources:
  - openapi/quantum-engine-api-openapi.yml
  type: oauth2
slug: google-quantum-ai-authentication
source_filename: google-quantum-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quantum-engine-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: googleOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  description: OAuth 2.0 via Google Cloud Application Default Credentials.\n  sources:\n  - openapi/quantum-engine-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/authentication/google-quantum-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Quantum Computing
- Quantum
- Hardware
- NISQ
- Error Correction
- Willow
- Sycamore
- Cirq
- Quantum Engine
- Superconducting Qubits
- Google Cloud
---
