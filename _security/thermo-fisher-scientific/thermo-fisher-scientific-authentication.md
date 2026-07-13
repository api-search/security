---
api_key_in: []
api_specs:
- filename: thermo-fisher-samplemanager-openapi.yml
  format: yaml
  label: Thermo Fisher SampleManager LIMS REST API
  slug: samplemanager-lims
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-samplemanager-openapi.yml
- filename: thermo-fisher-nanodrop-openapi.yml
  format: yaml
  label: Thermo Fisher NanoDrop Ultra Web API
  slug: nanodrop-ultra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-nanodrop-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Thermo Fisher Scientific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thermo Fisher Scientific secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thermo Fisher Scientific
provider_slug: thermo-fisher-scientific
scheme_count: 1
schemes:
- description: Session token obtained from the /mobile/login endpoint. Pass as "Bearer {token}" in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/thermo-fisher-samplemanager-openapi.yml
  type: http
slug: thermo-fisher-scientific-authentication
source_filename: thermo-fisher-scientific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thermo-fisher-samplemanager-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Session token obtained from the /mobile/login endpoint. Pass as \"Bearer {token}\"\n    in the Authorization header.\n  sources:\n  - openapi/thermo-fisher-samplemanager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/authentication/thermo-fisher-scientific-authentication.yml
summary_line: http · 1 scheme
tags:
- Life Sciences
- Laboratory
- Scientific Instruments
- LIMS
- Diagnostics
- Biosciences
- Fortune 500
---
