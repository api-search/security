---
api_key_in: []
api_specs:
- filename: google-quantum-ai-calibrations-api-openapi.yml
  format: yaml
  label: Google Quantum AI Calibrations API
  slug: google-quantum-ai-calibrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/google-quantum-ai-calibrations-api-openapi.yml
- filename: google-quantum-ai-jobs-api-openapi.yml
  format: yaml
  label: Google Quantum AI Jobs API
  slug: google-quantum-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/google-quantum-ai-jobs-api-openapi.yml
- filename: google-quantum-ai-processors-api-openapi.yml
  format: yaml
  label: Google Quantum AI Processors API
  slug: google-quantum-ai-processors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/google-quantum-ai-processors-api-openapi.yml
- filename: google-quantum-ai-programs-api-openapi.yml
  format: yaml
  label: Google Quantum AI Programs API
  slug: google-quantum-ai-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/google-quantum-ai-programs-api-openapi.yml
- filename: google-quantum-ai-reservations-api-openapi.yml
  format: yaml
  label: Google Quantum AI Reservations API
  slug: google-quantum-ai-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/google-quantum-ai-reservations-api-openapi.yml
- filename: google-quantum-ai-results-api-openapi.yml
  format: yaml
  label: Google Quantum AI Results API
  slug: google-quantum-ai-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-quantum-ai/refs/heads/main/openapi/google-quantum-ai-results-api-openapi.yml
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
