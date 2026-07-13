---
api_key_in: []
api_specs:
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Subjects API
  slug: vivalink-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Devices API
  slug: vivalink-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Vital Signs Data API
  slug: vivalink-vital-signs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Webhooks API
  slug: vivalink-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK FHIR API
  slug: vivalink-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vivalink Authentication
name_suffix: Authentication
oauth_flows: []
overview: VivaLNK secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VivaLNK
provider_slug: vivalink
scheme_count: 1
schemes:
- description: Modeled as an OAuth2/bearer access token issued to Developer Program partners for machine-to-machine access. Confirm the exact scheme (API key vs. OAuth2 client credentials) against VivaLNK's licensed docs.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vivalink-openapi.yml
  type: http
slug: vivalink-authentication
source_filename: vivalink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vivalink-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Modeled as an OAuth2/bearer access token issued to Developer Program partners\n    for machine-to-machine access. Confirm the exact scheme (API key vs. OAuth2 client credentials)\n    against VivaLNK's licensed docs.\n  sources:\n  - openapi/vivalink-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/authentication/vivalink-authentication.yml
summary_line: http · 1 scheme
tags:
- Connected Health
- Remote Patient Monitoring
- RPM
- Wearables
- Biosensors
- Biometrics
- ECG
- Vital Signs
- Digital Health
- IoT
- Clinical Trials
---
