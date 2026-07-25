---
api_key_in: []
api_specs:
- filename: thermo-fisher-scientific-authentication-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Authentication API
  slug: thermo-fisher-scientific-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-authentication-api-openapi.yml
- filename: thermo-fisher-scientific-entities-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Entities API
  slug: thermo-fisher-scientific-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-entities-api-openapi.yml
- filename: thermo-fisher-scientific-export-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Export API
  slug: thermo-fisher-scientific-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-export-api-openapi.yml
- filename: thermo-fisher-scientific-instrument-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Instrument API
  slug: thermo-fisher-scientific-instrument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-instrument-api-openapi.yml
- filename: thermo-fisher-scientific-measurements-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Measurements API
  slug: thermo-fisher-scientific-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-measurements-api-openapi.yml
- filename: thermo-fisher-scientific-methods-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Methods API
  slug: thermo-fisher-scientific-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-methods-api-openapi.yml
- filename: thermo-fisher-scientific-results-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Results API
  slug: thermo-fisher-scientific-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-results-api-openapi.yml
- filename: thermo-fisher-scientific-samples-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Samples API
  slug: thermo-fisher-scientific-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-samples-api-openapi.yml
- filename: thermo-fisher-scientific-workflows-api-openapi.yml
  format: yaml
  label: Thermo Fisher Scientific Workflows API
  slug: thermo-fisher-scientific-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thermo-fisher-scientific/refs/heads/main/openapi/thermo-fisher-scientific-workflows-api-openapi.yml
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
